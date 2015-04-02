# Abstracting Infrastructure

  As a developer you have very little time for the maintenance responsibities of full blown server to run your application.  Even managine virtual machines or DevOps tools such as Chef, Puppet & Vagrant take up considerable time away from development.

  All you really want to do is run your app somewhere other than your laptop or desktop.  So Heroku gives you Dynos to run the processes that make up your application.

![Heroku Dyno](../images/heroku-dyno.png)

## Dynos - a lightweight way to run your apps

  A dyno is the name Heroku uses for a lightweight container, which is an isolated space for your application to run safely and securely.  A container runs on top of an operating system that may be shared with other containers.

  Dyno's are very quick to create and very quick to destroy when no longer needed (compared to virtual machines).  This helps Heroku provide you with a highly scalable infrastructure without passing on the complexity to you.

  When you send your application to Heroku for deployment, a single file is created that represents your application.  This file is called a **Slug**.  We store each version of the Slug that is created for your app and when you want to scale we copy the relevant slug to any new dynos we create for you.

  When you deploy a new version of your app, a new slug file is created.  Then a new set of dynos are created on which this new slug is run, and network traffic is automatically re-routed to these new dynos.  This gives an almost instantaneous upgrade of your app to the new version.  To tidy up, all the dynos running the old versions of your app are shut down and deleted (although their slug is still avaialble for rollbacks).

### Dynos in context of the Infrastructure

  To help you put some context into Dynos and the use of containters, here is a highly simplified logical view of the PaaS infrastructure.

![Paas and IaaS conceptual infrastructure](../images/infrastructure-concept-iaas-paas.png)

  On Heroku, your application process runs in a container (Dyno) which in turn runs inside a virtual machine.  The virtual machines run on the physical computer hardware.

  Should there be an issue with the physical hardware, the virtual machine & its operating sytem, a new container (dyno) can be instantly created on a working part of the infrastructure and your application process started.
