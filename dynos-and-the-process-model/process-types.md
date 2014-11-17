# Processes types

  There are two process types you can define: **web** and _anything else_.

## Web process types  
  A web process listens to requests and responds with results, just as a web server or application server would.

  All request sent to your application are routed through to the dyno's you have running.  So the more dynos you run, the more requests you application can process.  


## Setting a PORT variable 

  You cannot specify the port number your application listens to, as Heroku may need to change this to provide you a consistent compute resources for your app.  Instead you can use the environment variable PORT to ask Heroku for the current port number.
  
  This PORT variable is usually used in either the Procfile when defining your process or in the configuration file for your application.
  
  See the [Java process examples](java-process-examples.html) section to see how this is used in the Procfile.

