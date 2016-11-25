# CoreWebApp
This demonstrates an issue with dotnetcore where a PreFlight (OPTIONS) request returns a 401 from dotnetcore if using Windows Authentication
<br>
<br>Issue described here:
<br>http://stackoverflow.com/questions/15734031/why-does-the-preflight-options-request-of-an-authenticated-cors-request-work-in

<br>To replicate the issue:
<br>1) Change the launchSettings.json to use your servername - don't use localhost as that complicates it further.
<br>2) Build and run this solution. 
<br>3) Do a put or post ajax call from a different domain (works in IE, fails in Chrome)
<br>
<br>You can use this jsFiddle for the ajax calls:
<br>http://jsfiddle.net/enricosaunders/o2u3yete/
