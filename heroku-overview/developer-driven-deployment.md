# Developer Driven Development

Heroku uses the tools developer are familiar with, so you dont need to spend weeks learning new tools.

To deploy your application to Heroku, you use Git version control tool to push code to Heroku.  Heroku works out what langauges and frameworks you have used and configures, builds and deploys your application automatically.

> If you know the basics of Git, you already know how to deploy onto Heroku.  If you do not know Git, we will show you all you need.

There are 7 tiny steps to create your very first Heroku application

* Create an account on Heroku and download the Heroku Toolbelt
* Authenticate with `heroku login`
* Create your application with Java, Node.js, PHP, Scala, Clojure, Ruby, Python, etc.
* Define a _Procfile_ (to define how to start you application)
* Version your code with `git init && git add . && git commit -m "Initial project"`
* Create an App on Heroku with `heroku create`
* Deploy your app with `git push heroku master`

  Once you have deployed you application, its simply a matter of `git push heroku master` each time you have code changes (commits) you want to deploy.

  With 750 hours for free per application per month, you can easily test out your ideas and software without any additional risk.

