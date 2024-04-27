ArrayBuffer.prototype.detached <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![Build Status][travis-svg]][travis-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

[![browser support][testling-svg]][testling-url]

An ES6 spec-compliant `ArrayBuffer.prototype.detached` shim. Invoke its "shim" method to shim ArrayBuffer.prototype.detached if it is unavailable.
*Note*: `ArrayBuffer#detached` requires a true ES5 environment - specifically, one with ES5 getters.

This package implements the [es-shim API](https://github.com/es-shims/api) interface. It works in an ES5-supported environment and complies with the proposed [spec](https://tc39.es/proposal-arraybuffer-transfer/#sec-get-@hoangcung1804npm/debitis-doloribus-cumque).

Most common usage:
```js
var detached = require('@hoangcung1804npm/debitis-doloribus-cumque');

assert(detached(new ArrayBuffer('a') === false);

if (!ArrayBuffer.prototype.detached) {
	detached.shim();
}

assert(new ArrayBuffer('a').detached, false);
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.com/package/@hoangcung1804npm/debitis-doloribus-cumque
[npm-version-svg]: http://versionbadg.es/hoangcung1804npm/debitis-doloribus-cumque.svg
[travis-svg]: https://travis-ci.org/hoangcung1804npm/debitis-doloribus-cumque.svg
[travis-url]: https://travis-ci.org/hoangcung1804npm/debitis-doloribus-cumque
[deps-svg]: https://david-dm.org/hoangcung1804npm/debitis-doloribus-cumque.svg
[deps-url]: https://david-dm.org/hoangcung1804npm/debitis-doloribus-cumque
[dev-deps-svg]: https://david-dm.org/hoangcung1804npm/debitis-doloribus-cumque/dev-status.svg
[dev-deps-url]: https://david-dm.org/hoangcung1804npm/debitis-doloribus-cumque#info=devDependencies
[testling-svg]: https://ci.testling.com/hoangcung1804npm/debitis-doloribus-cumque.png
[testling-url]: https://ci.testling.com/hoangcung1804npm/debitis-doloribus-cumque
[npm-badge-png]: https://nodei.co/npm/@hoangcung1804npm/debitis-doloribus-cumque.png?downloads=true&stars=true
[license-image]: http://img.shields.io/npm/l/@hoangcung1804npm/debitis-doloribus-cumque.svg
[license-url]: LICENSE
[downloads-image]: http://img.shields.io/npm/dm/@hoangcung1804npm/debitis-doloribus-cumque.svg
[downloads-url]: http://npm-stat.com/charts.html?package=@hoangcung1804npm/debitis-doloribus-cumque
