# Scalable Apps

![Heroku hightlights](../images/heroku-highlights.png)

  Heroku provides you with a highly scalable platform on which to run all your applications.  You can scale almost instantly by selecting the resources (dyno's) you need and Heroku automatically provisions them for you.
  
![Heroku scaling](../images/heroku-features-scaling-dynos.png)

  You can scale individual dynos (application processes) to create a very effective and highly scalable app, scaling each part up and down as required.  To scale effectively you need to gain understanding of how your application is going to be used and monitor how well it performs under various loads.

> **Warning** Simply throwing more and more resources to handle traffic with your app makes any Paas or IaaS service feel expensive.  [Monitoring App Performance](monitoring-performance.html) helps you get the most value from the Heroku platform.

## Designing scalable apps

  Application design is still your responsibility.  However Heroku share with your their experiences in running their own scalable apps and those of its customers.  
  
  Here are some factors to consider:

  * Break your app into components & [stateless processes](http://12factor.net/processes)
  * [Delivering static assets](https://devcenter.heroku.com/articles/s3)
  * [Scale out via the process model](http://12factor.net/concurrency) and create different types of processes for different workloads, such as [background jobs & queueing](https://devcenter.heroku.com/articles/background-jobs-queueing)
  * [Maximize the robustness of your app with processes]() that startup fast and gracefully shutdown
  * Understand your applications performance 

> **Hint** See the [12 Factor website](http://12factor.net/) for more details on this interesting and challenging topic.

  Of course you also need an appreciation of how your framework and language practices and design patterns help your application scale.

## Constraints

  To make the most of the Heroku platform, you should gain a deeper appreciation of Heroku and its constraints

  * [How Heroku works](https://devcenter.heroku.com/articles/how-heroku-works)
  * [Heroku Limits overview](https://devcenter.heroku.com/articles/limits)
  * [Dyno sizes](https://devcenter.heroku.com/articles/dyno-size) and [optomisation of dyno usage](https://devcenter.heroku.com/articles/optimizing-dyno-usage)
  * [Avoiding request timeouts](https://devcenter.heroku.com/articles/request-timeout) and maintaining sub 500ms response times
  * [Heroku error codes](https://devcenter.heroku.com/articles/error-codes)
  * [Recovering offline applications](https://devcenter.heroku.com/articles/application-offline)
  
  response time limits on processes (web, worker, scheduler plugin)

