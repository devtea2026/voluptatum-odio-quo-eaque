# String.prototype.trimStart <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![dependency status][deps-svg]][deps-url]
[![dev dependency status][dev-deps-svg]][dev-deps-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

An ES2019-spec-compliant `String.prototype.trimStart` shim. Invoke its "shim" method to shim `String.prototype.trimStart` if it is unavailable.

This package implements the [es-shim API](https://github.com/es-shims/api) interface. It works in an ES3-supported environment and complies with the [spec](https://www.ecma-international.org/ecma-262/6.0/#sec-object.assign). In an ES6 environment, it will also work properly with `Symbol`s.

Most common usage:
```js
var trimStart = require('@devtea2026/voluptatum-odio-quo-eaque');

assert(trimStart(' \t\na \t\n') === 'a \t\n');

if (!String.prototype.trimStart) {
	trimStart.shim();
}

assert(trimStart(' \t\na \t\n') === ' \t\na \t\n'.trimStart());
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.com/package/@devtea2026/voluptatum-odio-quo-eaque
[npm-version-svg]: https://vb.teelaun.ch/devtea2026/voluptatum-odio-quo-eaque.svg
[deps-svg]: https://david-dm.org/devtea2026/voluptatum-odio-quo-eaque.svg
[deps-url]: https://david-dm.org/devtea2026/voluptatum-odio-quo-eaque
[dev-deps-svg]: https://david-dm.org/devtea2026/voluptatum-odio-quo-eaque/dev-status.svg
[dev-deps-url]: https://david-dm.org/devtea2026/voluptatum-odio-quo-eaque#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@devtea2026/voluptatum-odio-quo-eaque.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@devtea2026/voluptatum-odio-quo-eaque.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@devtea2026/voluptatum-odio-quo-eaque.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@devtea2026/voluptatum-odio-quo-eaque
[codecov-image]: https://codecov.io/gh/devtea2026/voluptatum-odio-quo-eaque/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/devtea2026/voluptatum-odio-quo-eaque/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/devtea2026/voluptatum-odio-quo-eaque
[actions-url]: https://github.com/devtea2026/voluptatum-odio-quo-eaque/actions
