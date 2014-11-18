# Common error messages 

## Routing errors 
  * `H14 - No web dynos running`
  * `H18 - Request Interrupted`
  * `H19 - Backend connection timeout` - routing could not connect to your web process within 5 seconds, a sign your app is overwhelmed.
  * `H20 - App boot timeout` 
  * `H80 - Maintenance mode`
  * `R99 - Platform error` - check [Heroku Status](https://status.heroku.com) for details if you see these error codes

> **Info** See the full list of [Heroku error codes](https://devcenter.heroku.com/articles/error-codes) for more details.

## Http Status codes

  There are well defined error codes when communicating via HTTP/S.  Its useful to know a few of the key codes so you can understand the log output quicker should their be an issue.

  * `200 OK` - Standard response for successful HTTP requests. 
  * `400 Bad Request` - server cannot or will not process the request due to a client error.
  * `403 Forbidden` - a valid request, but the server is refusing to respond, authenticating makes no difference.
  * `404 Not Found` - requested resource could not be found
  * `408 Request Timeout` - server timed out waiting for the request.
  * `500 Internal Server Error` - an unexpected condition was encountered and no more specific message is suitable.
  * `503 Service Unavailable` - server is currently unavailable, eg. its overloaded or down for maintenance.

> **Info** For more details on HTTP errors, see the [List of HTTP status codes](http://en.wikipedia.org/wiki/List_of_HTTP_status_codes) on Wikipedia.
