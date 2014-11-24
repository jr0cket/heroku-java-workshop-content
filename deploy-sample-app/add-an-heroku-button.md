# Add an Heroku Button to the Sample App

Adding a Heroku Button to a your code repository on Github is simple. 


## Fork the project on Github 

  Make a copy of the sample application in your own Github account, so you can make changes to the project.  This is done by viewing the project on Github and pressing the **Fork** button 
  
  
> **TODO** add screenshots of Github project and forking process
  

## Create the app json file 

  Create a file called `app.json` with the following content.
  
> **TODO** add app.json file for sample play project  

  App.json is a way of describing apps and any services they require to be deployed. requirements are. Heroku uses this file to figure out how code in a particular repo should be deployed on the platform. 
  
  Add the following description to a new `app.json` file in the project you previously cloned, substituting the _address of your repository_ on Github in the **"repository"** value
  
    {
      "name": "Play on Heroku Sample",
      "description": "A simple Java app using the Play Framework and Postgres",
      "repository": "https://github.com/github-account/repository-name",
      "logo": "https://node-js-sample.herokuapp.com/node.svg",
      "keywords": ["node", "express", "static"]
    }

  
  
  Now add the app.json file to your local repository 
  
  `git add app.json`


## Add the Heroku Button 

  An Heroku button can live on any web page you like, although its common to simply add it to the `README.md` file in the Github repository that you want people to deploy.

  Edit the `README.md` file of the project and add the following to make an Heroku button appear in the `README.md` file:

```
[![Deploy to Heroku](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)
```

> **Note** The Heroku button code works for any Github repository, its not hard coded to a specific URL. Then means that the Heroku Button will work correctly if the Github repository is forked.  Heroku resolves the repo originating a button click by inspecting the referer header. 


  Add the updated README.md file to local repository and commit both changes

  `git add README.md`
  `git commit -m "adding heroku button to project`


  You can also use HTML code for the Heroku Button, for example if you want to include a button on a seperate web page.  You simply specify the address of the Github repository you want to deploy as a template value.  Here is an example:

```
<a href="https://heroku.com/deploy?template=https://github.com/github-account/repository-name">
  <img src="https://www.herokucdn.com/deploy/button.png" alt="Deploy to Heroku">
</a>
```



## Heroku button Generator

  You can also try an [unofficial Heroku button generator](https://www.expeditedssl.com/heroku-button-maker) for a web form way to create buttons for your own projects.

