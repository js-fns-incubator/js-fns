# js-fns

## Ideas behind js-fns

1. js-fns organization it's natural response to lack of CommonJS-compatible utility belts.
2. js-fns designed to be used in the browser via [webpack](http://webpack.github.io) or [Browserify](http://browserify.org) but with [Node.js](http://nodejs.org/) in mind.
3. js-fns it's a collection of "pick one function at once" libraries (like [lodash-node](https://github.com/lodash/lodash-node/)) but also can be used via bundles (installed via [Bower](http://bower.io) or another concat'n'uglify-compatible package manager).
4. js-fns supposed to be pure functional: immutable (unless user explicitly asks for mutation) & no prototype extensions.
5. js-fns is open to new contributors, repos and functions and only limitation is short guidelines and common sense. [Shoot an issue](https://github.com/js-fns/js-fns/issues) (or send PR) if you want to create a repo or become contributor.
6. js-fns also designed to be used as reference and the source of copy-paste (read it: feel free to "copy-paste" code from js-fns to StackOverflow).
7. js-fns it's not [Underscore.js](http://underscorejs.org/)/[https://lodash.com/](Lo-Dash)/[Sugar.js](http://sugarjs.com/)/[Moment.js](http://momentjs.com/) killer and not aimed to be a fame-generator.
8. js-fns it's not replacement for native functions (avalibale now or planned in the future versions), so we always prefer to use [shims](https://github.com/es-shims).

## FAQ

### What's worng with Sugar.js, it's [proven to be safe](http://sugarjs.com/native), no?

With concat'n'uglify approach it's the best fit, although it has [minor problemms with tests](https://github.com/andrewplummer/Sugar/issues/427). 

But with modular approach it becomes a plague: 

1. Lack of explicit dependencies makes code resistant to change, reuse and library-extraction.
2. Even if you are using 10% of Sugar.js, 100% of code will be served to user.

### Ok, what about [Underscore.js](http://underscorejs.org/) & [https://lodash.com/](Lo-Dash)?

As Sugar.js, both Underscore.js and Lo-Dash are designed to be used (and used widely in the community) as bundles. It means that ever function added bloats size of final application code. js-fns is restistant for that, because unused functions will never be in the final application JS file.

### Where is guidelines?

We have guidelines in our minds, but at the moment there is no list avaliable online aka TODO. [Contact us](https://github.com/js-fns/js-fns/issues) if you need more info.

### Where is `js-fns` package?

In the roadmap. [Shoot an issue](https://github.com/js-fns/js-fns/issues) if you need it ASAP.

### Who is working on it?

Basically it's internal [Toptal](http://www.toptal.com)'s core team project designed to solve our problems and needs.
