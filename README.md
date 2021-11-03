# Net6RegisterForJavaScriptTest

This project is meant to reproduce an issue with Blazor .NET 6 Release Candidate 2 using Dyanamic Root Components


Issue: https://github.com/dotnet/aspnetcore/issues/38044

Live demo: https://corylanza.github.io/Net6RegisterForJavaScriptTest/

Exception message:

`Uncaught (in promise) Error: System.ArgumentException: The type 'WebRendererInteropMethods' does not contain a public invokable method with [JSInvokableAttribute("AddRootComponent")].
   at Microsoft.JSInterop.Infrastructure.DotNetDispatcher.GetCachedMethodInfo(IDotNetObjectReference , String )
   at Microsoft.JSInterop.Infrastructure.DotNetDispatcher.InvokeSynchronously(JSRuntime , DotNetInvocationInfo& , IDotNetObjectReference , String )
   at Microsoft.JSInterop.Infrastructure.DotNetDispatcher.BeginInvokeDotNet(JSRuntime , DotNetInvocationInfo , String )`
