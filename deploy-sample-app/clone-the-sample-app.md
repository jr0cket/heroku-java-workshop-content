# Clone the sample app code

  To get all the code for our app onto our computer we use a command called clone.  This takes a complete copy of the Github repository, including all the history of changes.

    git clone github <sample-app-url>

> **Note** The github name can be anything you wish and is used as an alias for the full URL of the repository.  

> You can also specify the name of the directory the repository is copied into: 

>  `git clone github <sample-app-url> play-app`

  When you clone a repository, the orignal repository is linked to your local copy automatically.  You can see this by looking at the _remote_ settings of your local repository:
  
    git remote --verbose

> **TODO** screenshot of sample output

## How to Clone from an existing Heroku App

  If you are a collaborator on an Heroku app (ie. you created the app or someone added you) then you can access that apps code using the Heroku toolbelt.  In the **Code** section of the Heroku dashboard are details on how to _clone the repository_ using the `heroku git` command.  The `-a` option is for specifying the name of the app you wish to clone.  For example:

    heroku git:clone -a sample-play-app
    cd sample-play-app


