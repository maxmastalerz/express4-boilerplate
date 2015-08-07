# Express 4.x boilerplate

## About

This boilerplate is a reconstruction of [yanexbo](https://github.com/atufkas/yanexbo). It is simple in nature and updated to compile under express 4.x

Some changes to yanexbo and extra inclusions:

* Uses Express.js 4.x instead of 3.x
* Uses Hogan.js instead of Jade
* Example Hogan.js variables & partials
* Comes with sanitize-html package for simple user input sanitization.

## Installation

### Clone repository and install dependencies

via git and npm:

```
$ git clone git@github.com:meaniostack/express4-boilerplate.git [my-app-name]
$ cd [my-app-name]
$ npm install
```

### Setup database connection

Database and other environment specific application configuration is meant to be stored in `./config.js`.

```
...
development: {
    db: 'mongodb://localhost:27017/developmentDB'
}
...
```

### Run server

```
node servers.js
```

Open `http://localhost:3000` for sample page.

## Structure

```
/public                     Public (static) static files for express http server
/public/javascripts         Public javascript files
/public/javascripts/app.js  Sample javascript file (just a wrapper)
/public/stylesheets         Public stylesheet files
/public/stylesheets/app.js  Sample stylesheet file (minimalistic)
/routes                     Routing modules ("controllers")
/routes/index.js            Example routing module
/routes/hello.js            Example routing module
/views/                     View templates
/views/partials/head.html   Example hogan partial
/views/index.html           Example hogan view template
/views/dump.html            Example hogan view template
/config.js                  Database and application related configuration
/express-routes.js          Express routing definitions
/express-settings.js        Express configuration / settings
/server.js                  Main file for bootstrapping and starting node http server
```

## Contribute

Ideas, suggestions and pull requests are welcome.

## License

[The MIT License](http://opensource.org/licenses/MIT)

Copyright (c) 2015 Max Mastalerz &lt;maxmastalerz@hotmail.com&gt;