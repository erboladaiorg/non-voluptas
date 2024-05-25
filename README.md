# @erboladaiorg/non-voluptas <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

For use with React PropTypes. Will error on any prop not explicitly specified.

## Usage

```jsx
import PropTypes from 'prop-types';
import exact from '@erboladaiorg/non-voluptas';

function Foo({ foo, bar }) {
  return <div>{foo}{bar}</div>
}
Foo.propTypes = exact({
  foo: PropTypes.string,
  bar: PropTypes.number,
});

<Foo foo="hi" bar={3} /> // no warnings

<Foo foo="hi" bar={3} baz="extra" /> // propTypes warning!
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@erboladaiorg/non-voluptas
[npm-version-svg]: http://versionbadg.es/ljharb/@erboladaiorg/non-voluptas.svg
[deps-svg]: https://david-dm.org/ljharb/@erboladaiorg/non-voluptas.svg
[deps-url]: https://david-dm.org/ljharb/@erboladaiorg/non-voluptas
[dev-deps-svg]: https://david-dm.org/ljharb/@erboladaiorg/non-voluptas/dev-status.svg
[dev-deps-url]: https://david-dm.org/ljharb/@erboladaiorg/non-voluptas#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@erboladaiorg/non-voluptas.png?downloads=true&stars=true
[license-image]: http://img.shields.io/npm/l/@erboladaiorg/non-voluptas.svg
[license-url]: LICENSE
[downloads-image]: http://img.shields.io/npm/dm/@erboladaiorg/non-voluptas.svg
[downloads-url]: http://npm-stat.com/charts.html?package=@erboladaiorg/non-voluptas
[codecov-image]: https://codecov.io/gh/ljharb/@erboladaiorg/non-voluptas/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/ljharb/@erboladaiorg/non-voluptas/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/ljharb/@erboladaiorg/non-voluptas
[actions-url]: https://github.com/erboladaiorg/non-voluptas/actions
