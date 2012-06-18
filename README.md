timesync
========

A simple library to synchronize time between computers. 

Javascript usage
========
1. Add a reference to dependencies:
Jquery 1.5.* or later

2. Add a reference to the file src\foranyone.timeSync.js:
  <script src="~/Scripts/4n1.timeSync.js" type="text/javascript"></script>

3. Set the timeSync options if necessary. Below is the list of options with their default values:
  // Used to write debug data
  foranyone.timeSync.debug = false;

  // The url that returns the desired computer time
  foranyone.timeSync.url = "";
  
  // The http method used
  foranyone.timeSync.httpMethod = "POST";
  
  // The request content type
  foranyone.timeSync.contentType = "application/json; charset=utf-8";
  
4. Call the foranyone.timeSync.getTimeDifference function. It will return you positive or negative 
difference in milliseconds. It will also set the foranyone.timeSync.timeDifference variable with the value
returned (easier to reference in other scripts):
  var timeDifference = foranyone.timeSync.getTimeDifference()

  