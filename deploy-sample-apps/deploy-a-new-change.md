# Deploy a new change 

  Once you have created your application and deployed it on Heroku for the first time, you have a very simple deployment workflow for your projects.  Each time you make a meaningfull change to your project it is commited to your local  git repository.  When you have a one or more commits that you want to deploy, then you push them to the heroku git repository and the new version of your application is deployed.

You get into the following cycle:

    git add file(s)
    git commit -m "message"
    git push heroku master

> **fixme** Diagram of this workflow...

## Modify your project

  To demonstrate this workflow around Git and Heroku, lets make a simple change to the new application.  As its simple you can just use any editor you want, you dont need to set up an IDE as yet (we will do that later).

In the source code file `foobar.java` change the content of the response:

> **fixme** add code example here

## Commit your changes locally

  As you have made a change to your project, commit that change so that its under version control by git.

    git add .
    git commit -m "result returning hello world"

> TODO: another diagram

## Push your changes to Heroku

  Now the change has been commited locally, you can push it up to Heroku so your live application is up to date with your local app.

    git push heroku master

  This time the deployment should be much quicker as the dependencies are cached [TODO: check this is correct] build tool does not need to bring in any additional library dependencies.

> Optionally you can open a second terminal window and run the command `heroku logs --tail` to see what is happening to your app once it succesfully deploys.


  Either refresh your browser that displays you live appliction or use `heroku open` from the command line.
