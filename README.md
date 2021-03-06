## Running

* install `WWW::AdventCalendar`
* write something in `articles/`
* run `advcal -c advent.ini --today=2012-12-25`
* inspect `out/`

## Article Ideas

* intro (done)
  * where to get it
  * basic concept - combination of Bread::Board, Plack, and Path::Router
  * example of a basic OX app
* routebuilders and controllers (done)
  * basic structure - takes an OX::Request + path variables, returns a response
  * go over the default route builders
* routes and path::router (done)
  * overview of Path::Router
  * route syntax
  * validations?
* bread::board::declare (done)
  * overview of usage - attributes
* middleware (done)
  * wraps the application (just Plack middleware)
  * examples
* mounts (done)
  * includes an entirely separate PSGI application under a given path
  * also, inline mounts
* psgi (done)
  * requests
  * responses
* ox::request (done)
  * mostly modeled after Plack::Request
  * differences in parameter handling
  * encodings
  * mappings
* `uri_for` (done)
  * reverse of routing
  * defaults and validations
* HTTP::Throwable (done)
  * HTTPExceptions middleware is applied by default, so this just works
  * examples
* plack and deployment (done)
  * how to write a .psgi file for your app (and what belongs in it)
* roles and inheritance (done)
  * examples
* views (sartak)
  * just normal classes, nothing special at all
  * can also be controllers themselves, to bypass the need for extra logic
* custom routebuilders (doy)
* additional bread::board features (done)
  * subcontainers
  * type inference
  * lifecycles
* without the sugar (doy) (?)
  * `build_app`, `build_router`, etc
  * bread::board (underlying structure)
* roles as plugins
* example of authentication against a model (using middleware, not using middleware) -- or just translate http://www.catalystframework.org/calendar/2011/15 || http://www.catalystframework.org/calendar/2007/5 || http://www.catalystframework.org/calendar/2007/6
* extend authentication example into authorization
* example of q&d "dancer-style" inline app (done)
* simple app: filesystem-based wiki (ala http://www.catalystframework.org/calendar/2009/3 || http://advent.perldancer.org/2010/3 || http://advent.perldancer.org/2010/15 || http://advent.perldancer.org/2011/7)
* input validation example a la http://www.catalystframework.org/calendar/2010/10
* example of converting existing catalyst app to OX, benefits, pitfalls
* external scripts, cronjobs, etc (sartak)
  * here's where Bread::Board puts Catalyst to shame
* config (done)
* composing multiple OX applications
