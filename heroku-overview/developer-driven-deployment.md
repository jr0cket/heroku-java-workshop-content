# Developer Driven Development

  Heroku uses Git as the main way to deploy your application, so you dont need to spend time learning tools you are not already using.

> **Comment** If you know the basics of Git, you already know how to deploy onto Heroku.  If you do not know Git, we will show you all you need to know in this workshop.

> You can also develop your skills with Git at [try.github.io](https://try.github.io)

  When Heroku recieves your `git push` it works out what langauge and framework you have used and configures, builds and deploys your application automatically.  If your language or framework has a commonly used build tool, then Heroku installs that as well so it builds your application in the same way you do locally.

![Heroku deployment simplified](../images/heroku-push-simple.png)

### The developer workflow

  Heroku enables you to iterate on your app at your own pace, whether that be 1 release a month or many releases every hour.  As the deployment process is automated and triggered by a simple push, that deployment can take place by the development team, operations or via continuous integration tools.

  A typical developer workflow is:
  
* Develop your app, committing changes to your local git repository regularly (eg. several times an hour) creating branches where neccessary.

* Push your changes (commits) to a shared repository or continuous integration server, especially when working on a team project (eg. several times a day and/or overnight)  

* Deploy your app with `git push heroku master` when you want to share your running application with others, eg. to let others test it and give feedback or to deploy a new feature into production.

---

  Here is a [simple team workflow visualised](http://jr0cket.co.uk/developer-guides/heroku-developer-team-workflow-overview.png):
  
![Heroku Team Workflow](../images/heroku-developer-team-workflow-overview.png)

---

  It can be valuable to use a service such as Github or Bitbucket to collaborate on code, as they provide more features in that respect than Heroku.  Here is a [simple team workflow with Github](http://jr0cket.co.uk/developer-guides/heroku-developer-team-workflow-with-github.png):

![Heroku Teams and Github Workflow](../images/heroku-developer-team-workflow-with-github.png)

