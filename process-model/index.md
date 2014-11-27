# Dynos and the process model

  Heroku is easy to use as you avoid dealing with all the complexities of a server.  Instead we give you **Dynos** as an abstraction of the compute resources provided.  A dyno is a container that runs an application processes, as defined in the _Procfile_.
  
  Each of the process defined in your Procfile will run on its own dyno.  When you scale, you increase the number of dyno's running that process.
