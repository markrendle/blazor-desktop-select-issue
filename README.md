# Bug in WebView2 affecting MAUI Blazor Desktop

There is an [open issue on Microsoft's WebView2](https://github.com/MicrosoftEdge/WebView2Feedback/issues/666)
describing how the HTML `<select>` element does not work: the dropdown items of the `select` control are shown
behind the WebView2 control.

Obviously this affects MAUI's Blazor Desktop model, which uses WebView2 in its WinUI projects.
[Issue on the MAUI repo](https://github.com/dotnet/maui/issues/1353).

This repo contains a fresh Blazor Desktop solution created with .NET 6 Preview 5, with a simple `select` added
to the Index page to demonstrate the problem.