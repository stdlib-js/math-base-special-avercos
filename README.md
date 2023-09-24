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


<details>
  <summary>
    About stdlib...
  </summary>
  <p>We believe in a future in which the web is a preferred environment for numerical computation. To help realize this future, we've built stdlib. stdlib is a standard library, with an emphasis on numerical and scientific computation, written in JavaScript (and C) for execution in browsers and in Node.js.</p>
  <p>The library is fully decomposable, being architected in such a way that you can swap out and mix and match APIs and functionality to cater to your exact preferences and use cases.</p>
  <p>When you use stdlib, you can be absolutely certain that you are using the most thorough, rigorous, well-written, studied, documented, tested, measured, and high-quality code out there.</p>
  <p>To join us in bringing numerical computing to the web, get started by checking us out on <a href="https://github.com/stdlib-js/stdlib">GitHub</a>, and please consider <a href="https://opencollective.com/stdlib">financially supporting stdlib</a>. We greatly appreciate your continued support!</p>
</details>

# Arcvercosine

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Compute the [inverse versed cosine][inverse-versed-cosine].

<section class="intro">

The [inverse versed cosine][inverse-versed-cosine] is defined as

<!-- <equation class="equation" label="eq:arcvercosine" align="center" raw="\operatorname{avercos}(\theta) = \arccos(1+\theta)" alt="Inverse versed cosine."> -->

```math
\mathop{\mathrm{avercos}}(\theta) = \arccos(1+\theta)
```

<!-- <div class="equation" align="center" data-raw-text="\operatorname{avercos}(\theta) = \arccos(1+\theta)" data-equation="eq:arcvercosine">
    <img src="https://cdn.jsdelivr.net/gh/stdlib-js/stdlib@bb29798906e119fcb2af99e94b60407a270c9b32/lib/node_modules/@stdlib/math/base/special/avercos/docs/img/equation_arcvercosine.svg" alt="Inverse versed cosine.">
    <br>
</div> -->

<!-- </equation> -->

</section>

<!-- /.intro -->



<section class="usage">

## Usage

```javascript
import avercos from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-avercos@esm/index.mjs';
```
The previous example will load the latest bundled code from the esm branch. Alternatively, you may load a specific version by loading the file from one of the [tagged bundles](https://github.com/stdlib-js/math-base-special-avercos/tags). For example,

```javascript
import avercos from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-avercos@v0.1.0-esm/index.mjs';
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

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="module">

import linspace from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-base-linspace@esm/index.mjs';
import avercos from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-avercos@esm/index.mjs';

var x = linspace( -2.0, 0.0, 100 );

var i;
for ( i = 0; i < x.length; i++ ) {
    console.log( avercos( x[ i ] ) );
}

</script>
</body>
</html>
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/math-base/special/aversin`][@stdlib/math/base/special/aversin]</span><span class="delimiter">: </span><span class="description">compute the inverse versed sine.</span>
-   <span class="package-name">[`@stdlib/math-base/special/versin`][@stdlib/math/base/special/versin]</span><span class="delimiter">: </span><span class="description">compute the versed sine.</span>

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2023. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/math-base-special-avercos.svg
[npm-url]: https://npmjs.org/package/@stdlib/math-base-special-avercos

[test-image]: https://github.com/stdlib-js/math-base-special-avercos/actions/workflows/test.yml/badge.svg?branch=v0.1.0
[test-url]: https://github.com/stdlib-js/math-base-special-avercos/actions/workflows/test.yml?query=branch:v0.1.0

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/math-base-special-avercos/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/math-base-special-avercos?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/math-base-special-avercos.svg
[dependencies-url]: https://david-dm.org/stdlib-js/math-base-special-avercos/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/math-base-special-avercos/tree/deno
[umd-url]: https://github.com/stdlib-js/math-base-special-avercos/tree/umd
[esm-url]: https://github.com/stdlib-js/math-base-special-avercos/tree/esm
[branches-url]: https://github.com/stdlib-js/math-base-special-avercos/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/math-base-special-avercos/main/LICENSE

[inverse-versed-cosine]: https://en.wikipedia.org/wiki/Versine

<!-- <related-links> -->

[@stdlib/math/base/special/aversin]: https://github.com/stdlib-js/math-base-special-aversin/tree/esm

[@stdlib/math/base/special/versin]: https://github.com/stdlib-js/math-base-special-versin/tree/esm

<!-- </related-links> -->

</section>

<!-- /.links -->
