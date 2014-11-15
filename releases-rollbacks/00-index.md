# Releases & Rollbacks

  As its so quick and easy to deploy to heroku it is a great platform for agile development and continuous deployment.  With a simple git push you can new features, change the way the application looks as well as add more features.
  
  As typically there are many releases of a application, Heroku gives you a very easy way to see what releases have been made.  As software development is still a human activity then errors are inevitable, so Heroku provides an effective way carry out rollbacks to keep your site live.


## Working with releases

  To see your current list of releases for your application, use the following command within your project folder:

    heroku releases

  You should already have several release for your application, even if you have only done one or two pushes.  When you created your application uisng `heroku create` then several releases took place automatically.

  Your release history should look similar to the following:
  
> TODO: pictures of the new activity log
  
  Notice that each relase is related to a commit number used in Git.  This commit number gives you traceabitliy between your version control system and your deployed appliations.
  
  You can also dig deeper and see more details about latest release or any specific release using the following commands: 

    heroku releases:info
    heroku releases:info v24

