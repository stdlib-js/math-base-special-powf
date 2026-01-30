<!--

@license Apache-2.0

Copyright (c) 2025 The Stdlib Authors.

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

# Exponential Function

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> [Exponential function][exponential-function] for a single-precision floating-point number.

<section class="intro">

The [exponential function][exponential-function] is defined as

<!-- <equation class="equation" label="eq:exponential_function" align="center" raw="y = b^x" alt="Exponential function"> -->

```math
y = b^x
```

<!-- </equation> -->

where `b` is the **base** and `x` is the **exponent**.

</section>

<!-- /.intro -->



<section class="usage">

## Usage

```javascript
import powf from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-powf@v0.1.0-esm/index.mjs';
```

#### powf( base, exponent )

Evaluates the [exponential function][exponential-function] for a single-precision floating-point number.

```javascript
var v = powf( 2.0, 3.0 );
// returns 8.0

v = powf( 4.0, 0.5 );
// returns 2.0

v = powf( 100.0, 0.0 );
// returns 1.0

v = powf( 3.1415927410125732, 5.0 );
// returns ~306.0197

v = powf( 3.1415927410125732, -0.2 );
// returns ~0.7954

v = powf( NaN, 3.0 );
// returns NaN

v = powf( 5.0, NaN );
// returns NaN

v = powf( NaN, NaN );
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

import discreteUniform from 'https://cdn.jsdelivr.net/gh/stdlib-js/random-array-discrete-uniform@esm/index.mjs';
import logEachMap from 'https://cdn.jsdelivr.net/gh/stdlib-js/console-log-each-map@esm/index.mjs';
import powf from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-powf@v0.1.0-esm/index.mjs';

var opts = {
    'dtype': 'float32'
};
var b = discreteUniform( 100, 0, 10, opts );
var x = discreteUniform( 100, -5, 5, opts );

logEachMap( '%d^%d = %0.4f', b, x, powf );

</script>
</body>
</html>
```

</section>

<!-- /.examples -->

<!-- C interface documentation. -->



<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

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

## Copyright

Copyright &copy; 2016-2026. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/math-base-special-powf.svg
[npm-url]: https://npmjs.org/package/@stdlib/math-base-special-powf

[test-image]: https://github.com/stdlib-js/math-base-special-powf/actions/workflows/test.yml/badge.svg?branch=v0.1.0
[test-url]: https://github.com/stdlib-js/math-base-special-powf/actions/workflows/test.yml?query=branch:v0.1.0

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/math-base-special-powf/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/math-base-special-powf?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/math-base-special-powf.svg
[dependencies-url]: https://david-dm.org/stdlib-js/math-base-special-powf/main

-->

[chat-image]: https://img.shields.io/badge/zulip-join_chat-brightgreen.svg
[chat-url]: https://stdlib.zulipchat.com

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/math-base-special-powf/tree/deno
[deno-readme]: https://github.com/stdlib-js/math-base-special-powf/blob/deno/README.md
[umd-url]: https://github.com/stdlib-js/math-base-special-powf/tree/umd
[umd-readme]: https://github.com/stdlib-js/math-base-special-powf/blob/umd/README.md
[esm-url]: https://github.com/stdlib-js/math-base-special-powf/tree/esm
[esm-readme]: https://github.com/stdlib-js/math-base-special-powf/blob/esm/README.md
[branches-url]: https://github.com/stdlib-js/math-base-special-powf/blob/main/branches.md

[exponential-function]: https://en.wikipedia.org/wiki/Exponential_function

<!-- <related-links> -->

<!-- </related-links> -->

</section>

<!-- /.links -->
