# What triggers a new release

  It is important to understand what triggers a new release on Heroku.  As well as using `git push to` to upload new commits, the following actions also create a new release.
  
* Updating environment variables, `heroku config:add DB_URL=https://postgres.heroku.com/ofipie8ufdhh`

* Provisioning an Heroku add-on `heroku addon:postgres`


> TODO: anything else that triggers a release ?

