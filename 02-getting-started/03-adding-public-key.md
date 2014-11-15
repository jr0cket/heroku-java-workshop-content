# Adding a Public Key to your Heroku account 

> Heroku is beta testing a service called Http Git which removes the need for a public key and enables those users who would otherwise be stuck behind restrictive firewalls.  For more information, see the article [Http Git](https://devcenter.heroku.com/articles/http-git).

  To deploying your code on Heroku you need to securely authenticate yourself, this is done via public key encryption and therefore you need to add an SSH key to your Heroku account.  This same approach taken by services such as Github.

  Adding a public key to your Heroku account avoids having to enter username and password details each time you want to deploy your apps to Heroku.

  The following command authenticates you with Heroku and uploads your public key.  If you do not have a public key then the command will ask if you want to create one:

    heroku login

  You will be prompted for your Heroku account username and password.  Select `y` to generate a public key if you are asked.

> TODO: replace with a picture of the output of the heroku login command, so it looks like output rather than a command you have to run

```
$ heroku login
Enter your Heroku credentials.
Email: java@example.com
Password:
Could not find an existing public key.
Would you like to generate one? [Yn]
Generating new SSH public key.
Uploading ssh public key /Users/java/.ssh/id_rsa.pub
```

## Creating your own key (optional)

  Use the following command if you would prefer to create your key manually, rather than via `heroku login`.  When you create the public key, ensure you add the email address of your Heroku account as a comment:

    ssh-keygen -t rsa -C "email@used-for-heroku-account.com"
    
  To add a new key to Heroku, use the following command:
  
    heroku keys:add 
    
  If you have only one public key, this command will just add it to heroku without prompting.  If you have more than one pubic key then heroku will prompt you as to which key you want to add.

  For more information, see the [Managing SSH Keys](https://devcenter.heroku.com/articles/keys) article on Heroku document center.
  

