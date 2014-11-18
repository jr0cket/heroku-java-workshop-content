# Monitoring App Performance

If you need your apps to scale then you need to understand as many aspects of your applications performance as you can.

![Heroku Dashboard Metrics for your application](../images/heroku-dashboard-monitoring-example.png)

Heroku provides metrics around your app as well as database queries when using Heroku Postgres database.

![Heroku Dashboard Metrics for Postgres](../images/heroku-dashboard-postgres-dbx-example.png)

---

## Addons for Performance Metrics 

New Relic...



## Advanced stuff

From http://dojo-curriculum.herokuapp.com/modules/running-production-applications.html

> TODO: some advanced aspects of application performance.  Make this a seperate section ?  Elaborate

Explain why it is imperative that a web process responds quickly.

Explain that more than 500ms per response is a cause for concern.

Explain that only the work required to generate the response should be carried out in the web processes. Everything else should be pushed into a background process.

Talk about request queuing when concurrency isn't high enough.

Talk about what causes the H12 error (long running requests, and request queueing).

Explain that once an H12 error has fired, the process is still running (the request is disconnected at the router).

Talk about the compound effect that can occur with slow running requests, that then build into a problem with H12s. Mention that this does not only relate to slow requests, but can affect relatively fast applications under the correct conditions.

Talk about Rack-Timeout for Ruby applications where applicable.
