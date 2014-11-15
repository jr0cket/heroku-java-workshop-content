# Using Heroku Postgres database 
  
  Postgres is a very impressive database and has a very wide range of features. Postgres is also a very active active open source project, with a long history.  Heroku wrapped the same kind of developer focused services around Postgress, making it really easy to use.

  With Heroku Postgres you can use this database along with your application or as a standalone database (Postgress as a Service).

  Read more about [Heroku Postress](http://postgres.heroku.com/) 
  
  
## Add Postgress Driver to the application

  To use Heroku Postgres as the database for our Play application, we need to specify a library that contains the driver used to access the database.

  Add the required driver to the application dependencies in the `project/Build.scala` file (this file may need to be created):

> Read more about [Dependencies managementin the Play framework](http://playframework.com).
   

> TODO: can we push at this stage or should we change the Procfile to include paramters for the app or DB


## Understanding Postgres usage

* Postgres config
* Postgress size 

`heroku pg:info`

Add a follower database and time that with the following command:

`heroku pg:wait`

