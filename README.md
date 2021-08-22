<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->

# Arcvercosine

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] [![dependencies][dependencies-image]][dependencies-url]

> Compute the [inverse versed cosine][inverse-versed-cosine].

<section class="intro">

The [inverse versed cosine][inverse-versed-cosine] is defined as

<!-- <equation class="equation" label="eq:arcvercosine" align="center" raw="\operatorname{avercos}(\theta) = \arccos(1+\theta)" alt="Inverse versed cosine."> -->

<div class="equation" align="center" data-raw-text="\operatorname{avercos}(\theta) = \arccos(1+\theta)" data-equation="eq:arcvercosine">
    <img src="https://cdn.jsdelivr.net/gh/stdlib-js/stdlib@bb29798906e119fcb2af99e94b60407a270c9b32/lib/node_modules/@stdlib/math/base/special/avercos/docs/img/equation_arcvercosine.svg" alt="Inverse versed cosine.">
    <br>
</div>

<!-- </equation> -->

</section>

<!-- /.intro -->

<section class="installation">

## Installation

```bash
npm install @stdlib/math-base-special-avercos
```

</section>

<section class="usage">

## Usage

```javascript
var avercos = require( '@stdlib/math-base-special-avercos' );
```

#### avercos( x )

Computes the [inverse versed cosine][inverse-versed-cosine].

```javascript
var v = avercos( 0.0 );
// returns 0.0

v = avercos( -3.141592653589793/2.0 );
// returns ~2.1783

v = avercos( -3.141592653589793/6.0 );
// returns ~1.0742
```

If `x < -2`, `x > 0`, or `x` is `NaN`, the function returns `NaN`.

```javascript
var v = avercos( 1.0 );
// returns NaN

v = avercos( -3.14 );
// returns NaN

v = avercos( NaN );
// returns NaN
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```javascript
var linspace = require( '@stdlib/array-linspace' );
var avercos = require( '@stdlib/math-base-special-avercos' );

var x = linspace( -2.0, 0.0, 100 );
var i;

for ( i = 0; i < x.length; i++ ) {
    console.log( avercos( x[ i ] ) );
}
```

</section>

<!-- /.examples -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2021. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/math-base-special-avercos.svg
[npm-url]: https://npmjs.org/package/@stdlib/math-base-special-avercos

[test-image]: https://github.com/stdlib-js/math-base-special-avercos/actions/workflows/test.yml/badge.svg
[test-url]: https://github.com/stdlib-js/math-base-special-avercos/actions/workflows/test.yml

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/math-base-special-avercos/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/math-base-special-avercos?branch=main

[dependencies-image]: https://img.shields.io/david/stdlib-js/math-base-special-avercos.svg
[dependencies-url]: https://david-dm.org/stdlib-js/math-base-special-avercos/main

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/math-base-special-avercos/main/LICENSE

[inverse-versed-cosine]: https://en.wikipedia.org/wiki/Versine

</section>

<!-- /.links -->
