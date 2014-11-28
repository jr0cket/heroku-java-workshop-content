# Configuration Variables in the Procfile 

  You can use configuration variables in the Procfile.  Common examples are database connections or port numbers for listening for web traffic. 


## Setting a PORT variable 

  You cannot specify the port number your application listens to, as Heroku may need to change this to provide you a consistent compute resources for your app.  Instead you can use the environment variable PORT to ask Heroku for the current port number.
  
  This PORT variable is usually used in either the Procfile when defining your process or in the configuration file for your application.
  
  See the [Java process examples](java-process-examples.html) section to see how this is used in the Procfile.

