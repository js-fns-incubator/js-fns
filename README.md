# js-fns

## Ideas behind js-fns

1. js-fns foundation is natural response to the lack of CommonJS-compatible utility belts.
2. js-fns is designed to be used in the browser via [webpack](http://webpack.github.io) or [Browserify](http://browserify.org) but with [Node.js](http://nodejs.org/) in mind.
3. js-fns is a collection of "pick one function at once" libraries (like [lodash-node](https://github.com/lodash/lodash-node/)) but also can be used via bundles (installed via [Bower](http://bower.io) or another concat'n'uglify-compatible package manager).
4. js-fns is supposed to be pure functional: immutable (unless user explicitly asks for mutation), no prototype extensions.
5. js-fns is open to new contributors, repos and functions. Only limitations are short guidelines and common sense. [Shoot an issue](https://github.com/js-fns/js-fns/issues) (or send PR) if you want to create a repo or become a contributor.
6. js-fns is also designed to be used as the reference and the copy-paste source (i.e. feel free to "copy-paste" code from js-fns to StackOverflow).
7. js-fns is not [Underscore.js](http://underscorejs.org/)/[Lo-Dash](https://lodash.com/)/[Sugar.js](http://sugarjs.com/)/[Moment.js](http://momentjs.com/) killer and not aimed to be a fame-generator.
8. js-fns is not replacement for native functions (available now or planned in the future versions), so we always prefer to use [shims](https://github.com/es-shims).

## FAQ

### What's wrong with Sugar.js, it is [proven to be safe](http://sugarjs.com/native), isn't it?

With concat'n'uglify approach it's the best fit, although it has [minor problems with tests](https://github.com/andrewplummer/Sugar/issues/427). 

But with modular approach it becomes a plague: 

1. Lack of explicit dependencies makes code resistant to change, reuse and library-extraction.
2. Even if you are using 10% of Sugar.js, 100% of code will be send to user.

### Ok, but what about [Underscore.js](http://underscorejs.org/) or [Lo-Dash](https://lodash.com/)?

Like Sugar.js, both Underscore.js and Lo-Dash are designed to be used (and used widely in the community) as bundles. It means that any added function bloats size of final application code. js-fns is resistant to that, because unused functions will never be in the final application JS file.

### Where are the guidelines?

We have guidelines in our minds, but at the moment there is no TODO list avaliable online. [Contact us](https://github.com/js-fns/js-fns/issues) if you need more info.

### Where is `js-fns` package?

In the roadmap. [Shoot an issue](https://github.com/js-fns/js-fns/issues) if you need it ASAP.

### Who is working on it?

Basically it's internal [Toptal](http://www.toptal.com) core team's project designed to solve our problems and needs.
