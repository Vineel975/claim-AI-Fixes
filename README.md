Server Error in '/' Application.
A potentially dangerous Request.Form value was detected from the client (hdnCodingEligibilityDesign="<div class="col-sm-1...").
Description: ASP.NET has detected data in the request that is potentially dangerous because it might include HTML markup or script. The data might represent an attempt to compromise the security of your application, such as a cross-site scripting attack. If this type of input is appropriate in your application, you can include code in a web page to explicitly allow it. For more information, see http://go.microsoft.com/fwlink/?LinkID=212874.

Exception Details: System.Web.HttpRequestValidationException: A potentially dangerous Request.Form value was detected from the client (hdnCodingEligibilityDesign="<div class="col-sm-1...").

Source Error:

An unhandled exception was generated during the execution of the current web request. Information regarding the origin and location of the exception can be identified using the exception stack trace below.

Stack Trace:


[HttpRequestValidationException (0x80004005): A potentially dangerous Request.Form value was detected from the client (hdnCodingEligibilityDesign="<div class="col-sm-1...").]
   System.Web.HttpRequest.ValidateString(String value, String collectionKey, RequestValidationSource requestCollection) +417
   System.Web.HttpValueCollection.EnsureKeyValidated(String key) +102
   System.Web.HttpValueCollection.GetValues(Int32 index) +37
   System.Collections.Specialized.NameValueCollection.Add(NameValueCollection c) +8375111
   System.Web.Mvc.FormCollectionModelBinder.BindModel(ControllerContext controllerContext, ModelBindingContext bindingContext) +193
   System.Web.Mvc.ControllerActionInvoker.GetParameterValue(ControllerContext controllerContext, ParameterDescriptor parameterDescriptor) +458
   System.Web.Mvc.ControllerActionInvoker.GetParameterValues(ControllerContext controllerContext, ActionDescriptor actionDescriptor) +137
   System.Web.Mvc.Async.<>c__DisplayClass21.<BeginInvokeAction>b__19(AsyncCallback asyncCallback, Object asyncState) +1151
   System.Web.Mvc.Async.WrappedAsyncResultBase`1.Begin(AsyncCallback callback, Object state, Int32 timeout) +166
   System.Web.Mvc.Async.AsyncControllerActionInvoker.BeginInvokeAction(ControllerContext controllerContext, String actionName, AsyncCallback callback, Object state) +463
   System.Web.Mvc.Controller.<BeginExecuteCore>b__1c(AsyncCallback asyncCallback, Object asyncState, ExecuteCoreState innerState) +51
   System.Web.Mvc.Async.WrappedAsyncVoid`1.CallBeginDelegate(AsyncCallback callback, Object callbackState) +73
   System.Web.Mvc.Async.WrappedAsyncResultBase`1.Begin(AsyncCallback callback, Object state, Int32 timeout) +166
   System.Web.Mvc.Controller.BeginExecuteCore(AsyncCallback callback, Object state) +860
   System.Web.Mvc.Async.WrappedAsyncResultBase`1.Begin(AsyncCallback callback, Object state, Int32 timeout) +166
   System.Web.Mvc.Controller.BeginExecute(RequestContext requestContext, AsyncCallback callback, Object state) +711
   System.Web.Mvc.MvcHandler.<BeginProcessRequest>b__4(AsyncCallback asyncCallback, Object asyncState, ProcessRequestState innerState) +102
   System.Web.Mvc.Async.WrappedAsyncVoid`1.CallBeginDelegate(AsyncCallback callback, Object callbackState) +73
   System.Web.Mvc.Async.WrappedAsyncResultBase`1.Begin(AsyncCallback callback, Object state, Int32 timeout) +166
   System.Web.Mvc.MvcHandler.BeginProcessRequest(HttpContextBase httpContext, AsyncCallback callback, Object state) +502
   System.Web.CallHandlerExecutionStep.System.Web.HttpApplication.IExecutionStep.Execute() +1130
   System.Web.<>c__DisplayClass285_0.<ExecuteStepImpl>b__0() +42
   System.Web.HttpApplication.ExecuteStepImpl(IExecutionStep step) +121
   System.Web.HttpApplication.ExecuteStep(IExecutionStep step, Boolean& completedSynchronously) +140

Version Information: Microsoft .NET Framework Version:4.0.30319; ASP.NET Version:4.8.9319.0
