<div align="center">
  <a href="http://github.com/flyjs/fly">
    <img width=200px  src="https://cloud.githubusercontent.com/assets/8317250/8733685/0be81080-2c40-11e5-98d2-c634f076ccd7.png">
  </a>
</div>

> Use [XO](https://github.com/sindresorhus/xo)'s shareable config for [fly-eslint][fly-eslint]

[![][fly-badge]][fly]
[![npm package][npm-ver-link]][releases]
[![][dl-badge]][npm-pkg-link]
[![][travis-badge]][travis-link]
[![][mit-badge]][mit]

## Install

This package depends on [fly-eslint][fly-eslint]. It must be installed before (or with) `fly-eslint-xo`.

```a
npm install -D fly-eslint fly-eslint-xo
```

Then create a `.eslintrc` file in your project root.

For ES5 linting:

```json
{
  "extends": "xo"
}
```

For ES2015 (or "ES6") linting: 

```json
{
  "extends": "xo/esnext"
}
```

Check out [XO's Documentation](https://github.com/sindresorhus/eslint-config-xo#usage) for information on usage and configuration.

## Usage

Follow the normal `fly-eslint` usage:

```js
export function* linter () {
  yield this.source("src/**/*.js").eslint()
}
```

## License

[MIT][mit] © [Luke Edwards][author] et [al][contributors]


[fly-eslint]:   https://github.com/bucaran/fly-eslint
[mit]:          http://opensource.org/licenses/MIT
[author]:       https://lukeed.com
[contributors]: https://github.com/lukeed/fly-eslint-xo/graphs/contributors
[releases]:     https://github.com/lukeed/fly-eslint-xo/releases
[fly]:          https://www.github.com/flyjs/fly
[fly-badge]:    https://img.shields.io/badge/fly-JS-05B3E1.svg?style=flat-square
[mit-badge]:    https://img.shields.io/badge/license-MIT-444444.svg?style=flat-square
[npm-pkg-link]: https://www.npmjs.org/package/fly-eslint-xo
[npm-ver-link]: https://img.shields.io/npm/v/fly-eslint-xo.svg?style=flat-square
[dl-badge]:     http://img.shields.io/npm/dm/fly-eslint-xo.svg?style=flat-square
[travis-link]:  https://travis-ci.org/lukeed/fly-eslint-xo
[travis-badge]: http://img.shields.io/travis/lukeed/fly-eslint-xo.svg?style=flat-square
