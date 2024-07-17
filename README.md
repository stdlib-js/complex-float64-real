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

# real

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Return the real component of a double-precision complex floating-point number.

<!-- Section to include introductory text. Make sure to keep an empty line after the intro `section` element and another before the `/section` close. -->

<section class="intro">

</section>

<!-- /.intro -->

<!-- Package usage documentation. -->



<section class="usage">

## Usage

To use in Observable,

```javascript
real = require( 'https://cdn.jsdelivr.net/gh/stdlib-js/complex-float64-real@umd/browser.js' )
```

To vendor stdlib functionality and avoid installing dependency trees for Node.js, you can use the UMD server build:

```javascript
var real = require( 'path/to/vendor/umd/complex-float64-real/index.js' )
```

To include the bundle in a webpage,

```html
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/complex-float64-real@umd/browser.js"></script>
```

If no recognized module system is present, access bundle contents via the global scope:

```html
<script type="text/javascript">
(function () {
    window.real;
})();
</script>
```

#### real( z )

Returns the **real** component of a double-precision complex floating-point number.

```javascript
var Complex128 = require( '@stdlib/complex-float64-ctor' );

var z = new Complex128( 5.0, 3.0 );
var re = real( z );
// returns 5.0
```

</section>

<!-- /.usage -->

<!-- Package usage notes. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="notes">

</section>

<!-- /.notes -->

<!-- Package usage examples. -->

<section class="examples">

## Examples

<!-- eslint-disable max-len -->

<!-- eslint no-undef: "error" -->

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/complex-float64-ctor@umd/browser.js"></script>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/random-base-discrete-uniform@umd/browser.js"></script>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/array-filled-by@umd/browser.js"></script>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/complex-float64-real@umd/browser.js"></script>
<script type="text/javascript">
(function () {

function random() {
    return new Complex128( discreteUniform( -10, 10 ), discreteUniform( -10, 10 ) ); // eslint-disable-line max-len
}

// Generate an array of random complex numbers:
var x = filledarrayBy( 100, 'complex128', random );
// returns <Complex128Array>

// Retrieve the real component of each complex number...
var z;
var i;
for ( i = 0; i < x.length; i++ ) {
    z = x.get( i );
    console.log( 'real(%s) = %d', z.toString(), real( z ) );
}

})();
</script>
</body>
</html>
```

</section>

<!-- /.examples -->

<!-- C interface documentation. -->



<!-- Section to include cited references. If references are included, add a horizontal rule *before* the section. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="references">

</section>

<!-- /.references -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/complex-float64/imag`][@stdlib/complex/float64/imag]</span><span class="delimiter">: </span><span class="description">return the imaginary component of a double-precision complex floating-point number.</span>
-   <span class="package-name">[`@stdlib/complex-float64/reim`][@stdlib/complex/float64/reim]</span><span class="delimiter">: </span><span class="description">return the real and imaginary components of a double-precision complex floating-point number.</span>

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


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

Copyright &copy; 2016-2024. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/complex-float64-real.svg
[npm-url]: https://npmjs.org/package/@stdlib/complex-float64-real

[test-image]: https://github.com/stdlib-js/complex-float64-real/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/complex-float64-real/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/complex-float64-real/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/complex-float64-real?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/complex-float64-real.svg
[dependencies-url]: https://david-dm.org/stdlib-js/complex-float64-real/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/complex-float64-real/tree/deno
[deno-readme]: https://github.com/stdlib-js/complex-float64-real/blob/deno/README.md
[umd-url]: https://github.com/stdlib-js/complex-float64-real/tree/umd
[umd-readme]: https://github.com/stdlib-js/complex-float64-real/blob/umd/README.md
[esm-url]: https://github.com/stdlib-js/complex-float64-real/tree/esm
[esm-readme]: https://github.com/stdlib-js/complex-float64-real/blob/esm/README.md
[branches-url]: https://github.com/stdlib-js/complex-float64-real/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/complex-float64-real/main/LICENSE

<!-- <related-links> -->

[@stdlib/complex/float64/imag]: https://github.com/stdlib-js/complex-float64-imag/tree/umd

[@stdlib/complex/float64/reim]: https://github.com/stdlib-js/complex-float64-reim/tree/umd

<!-- </related-links> -->

</section>

<!-- /.links -->