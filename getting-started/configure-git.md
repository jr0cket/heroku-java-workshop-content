# Configure Git with name and email

  Git is the main method used to copy source code to Heroku so it can deploy the correct version of your application.  

  The Heroku toolbelt includes a command line Git client.  You may use any git client you prefer, either command line or graphical tool.

> **Note** Identify yourself to Git before you are able to commit changes by configuring your name and email address (preferably the email used to create your Heroku account).

  To add your git name and email, either edit the file `~/.gitconfig` or run the following two commands:

    git config --global user.name "your name"
    git config --global user.email "your.name@domain.com"

  To check if your identity has already been added to Git (some gui clients add information), you can list all the current configuration entries using the command:

    git config --list

> **Hint** Simple graphical tools for Git include [Github for Mac](https://mac.github.com/) or [Github for Windows](https://windows.github.com/).  For a more advanced graphical tool, try [SourceTree](https://windows.github.com/).  All Git clients will used the `~/.gitconfig` file for their configuraiion

> If you are still finding your way with Git, take a look at the seperate [Git tutorial](http://jr0cket.co.uk/git-workshop/) or [try.github.io](http://try.github.io)
  
