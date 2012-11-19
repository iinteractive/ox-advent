## Running

* install `WWW::AdventCalendar`
* write something in `articles/`
* run `advcal -c advent.ini --today=2012-12-25`
* inspect `out/`

## Article Ideas

* intro
  * where to get it
  * basic concept - combination of Bread::Board, Plack, and Path::Router
  * example of a basic OX app
* routes and path::router
  * overview of Path::Router
  * route syntax
  * validations?
* routebuilders and controllers
  * basic structure - takes an OX::Request + path variables, returns a response
  * go over the default route builders
* views
  * just normal classes, nothing special at all
  * can also be controllers themselves, to bypass the need for extra logic
* mounts
  * includes an entirely separate PSGI application under a given path
  * also, inline mounts
* middleware
  * wraps the application (just Plack middleware)
  * give examples?
* HTTP::Throwable
  * HTTPExceptions middleware is applied by default, so this just works
  * examples
* bread::board::declare
  * overview of usage - attributes
* dependencies
  * explicit dependencies
  * infer => 1
* ox::request
  * mostly modeled after Plack::Request
  * differences in parameter handling
  * encodings
  * mappings
* `uri_for`
  * reverse of routing
  * defaults and validations
* roles and inheritance
  * examples
* psgi
  * how to write a .psgi file for your app (and what belongs in it)
  * ???
* bread::board (underlying structure)
* without the sugar
* external scripts, cronjobs, etc (basically: here's where Bread::Board puts Catalyst to shame)
* custom routebuilders
* external routers
* roles as plugins
* example of authentication against a model (using middleware, not using middleware) -- or just translate http://www.catalystframework.org/calendar/2011/15 || http://www.catalystframework.org/calendar/2007/5 || http://www.catalystframework.org/calendar/2007/6
* extend authentication example into authorization
* example of q&d "dancer-style" inline app
* config (I'm not in love with what I did for Appfarm, would love to see more ideas -- shawn)
* simple app: filesystem-based wiki (ala http://www.catalystframework.org/calendar/2009/3 || http://advent.perldancer.org/2010/3 || http://advent.perldancer.org/2010/15 || http://advent.perldancer.org/2011/7)
* input validation example a la http://www.catalystframework.org/calendar/2010/10
* example of converting existing catalyst app to OX, benefits, pitfalls
