# Create a Staging Environment for your App

Lets create a second environment for the app, called Staging.  This environment is typically used to run usability, acceptance and performance testing before deploying a new version to production.

## Create the environment 

    # Check for addons 
    heroku addons:list 
    
    # Provision the staging environment 
    heroku create my-app-staging 


## Pushing to the Staging Environment

  As you have a single code-base for your app, shared between all your environments, you simply push the version you want using Git.
  
    git push my-app-staging master


## Using Git Log to track deployment



> Forking - if its still recommended
