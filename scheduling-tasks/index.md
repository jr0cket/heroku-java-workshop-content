# Scheduling Tasks

> **TODO** work in progress

  Sometimes you want to run a task or script just once rather than continually running.  Heroku provides several ways to do this.
  
  * One-time tasks - using `heroku run` command
  * Using Scheduler, Temo, etc addons to set up a CRON-like regular task 
  * Worker dynos for long running tasks 

  If you are running a short task then you can use `Heroku run` or one of the scheduling addons.  If you have a longer running task you should use a **worker** dyno.
  
  
