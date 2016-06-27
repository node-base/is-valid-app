# is-valid-app [![NPM version](https://img.shields.io/npm/v/is-valid-app.svg?style=flat)](https://www.npmjs.com/package/is-valid-app) [![NPM downloads](https://img.shields.io/npm/dm/is-valid-app.svg?style=flat)](https://npmjs.org/package/is-valid-app) [![Build Status](https://img.shields.io/travis/node-base/is-valid-app.svg?style=flat)](https://travis-ci.org/node-base/is-valid-app)

Wrapper around is-valid-instance and is-registered for validating `base` plugins. Returns true if `app` is a valid instance of base and a plugin is not registered yet.

## Install

Install with [npm](https://www.npmjs.com/):

```sh
$ npm install --save is-valid-app
```

## Usage

```js
var isValid = require('is-valid-app');

// in your Base plugin
function plugin(app) {
  // plugin name is required as the second argument
  if (!isValid(app, 'my-plugin')) return;
  // do plugin stuff
}
```

Optionally pass an array of instance types as the third argument:

```js
function plugin(app) {
  if (!isValid(app, 'my-plugin', ['view', 'collection'])) return;
  // do plugin stuff
}
```

Visit [base](https://github.com/node-base/base) for more details.

## Related projects

You might also be interested in these projects:

* [base](https://www.npmjs.com/package/base): base is the foundation for creating modular, unit testable and highly pluggable node.js applications, starting… [more](https://github.com/node-base/base) | [homepage](https://github.com/node-base/base "base is the foundation for creating modular, unit testable and highly pluggable node.js applications, starting with a handful of common methods, like `set`, `get`, `del` and `use`.")
* [is-registered](https://www.npmjs.com/package/is-registered): Util for Base that optionally prevents a plugin from being registered more than once on… [more](https://github.com/jonschlinkert/is-registered) | [homepage](https://github.com/jonschlinkert/is-registered "Util for Base that optionally prevents a plugin from being registered more than once on an instance")
* [is-valid-instance](https://www.npmjs.com/package/is-valid-instance): Returns true if a value is a valid instance of Base. | [homepage](https://github.com/jonschlinkert/is-valid-instance "Returns true if a value is a valid instance of Base.")

## Contributing

This document was generated by [verb-readme-generator](https://github.com/verbose/verb-readme-generator) (a [verb](https://github.com/verbose/verb) generator), please don't edit directly. Any changes to the readme must be made in [.verb.md](.verb.md). See [Building Docs](#building-docs).

Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](../../issues/new).

Or visit the [verb-readme-generator](https://github.com/verbose/verb-readme-generator) project to submit bug reports or pull requests for the readme layout template.

## Building docs

_(This document was generated by [verb-readme-generator](https://github.com/verbose/verb-readme-generator) (a [verb](https://github.com/verbose/verb) generator), please don't edit the readme directly. Any changes to the readme must be made in [.verb.md](.verb.md).)_

Generate readme and API documentation with [verb](https://github.com/verbose/verb):

```sh
$ npm install -g verb verb-readme-generator && verb
```

## Running tests

Install dev dependencies:

```sh
$ npm install -d && npm test
```

## Author

**Jon Schlinkert**

* [github/jonschlinkert](https://github.com/jonschlinkert)
* [twitter/jonschlinkert](http://twitter.com/jonschlinkert)

## License

Copyright © 2016, [Jon Schlinkert](https://github.com/jonschlinkert).
Released under the [MIT license](https://github.com/node-base/is-valid-app/blob/master/LICENSE).

***

_This file was generated by [verb](https://github.com/verbose/verb), v0.9.0, on June 27, 2016._