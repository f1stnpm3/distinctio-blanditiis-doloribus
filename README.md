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

# Iterators

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Iterator utilities.

<section class="installation">

## Installation

```bash
npm install @f1stnpm3/distinctio-blanditiis-doloribus
```

Alternatively,

-   To load the package in a website via a `script` tag without installation and bundlers, use the [ES Module][es-module] available on the [`esm`][esm-url] branch (see [README][esm-readme]).
-   If you are using Deno, visit the [`deno`][deno-url] branch (see [README][deno-readme] for usage intructions).
-   For use in Observable, or in browser/node environments, use the [Universal Module Definition (UMD)][umd] build available on the [`umd`][umd-url] branch (see [README][umd-readme]).

The [branches.md][branches-url] file summarizes the available branches and displays a diagram illustrating their relationships.

To view installation and usage instructions specific to each branch build, be sure to explicitly navigate to the respective README files on each branch, as linked to above.

</section>

<section class="usage">

## Usage

```javascript
var ns = require( '@f1stnpm3/distinctio-blanditiis-doloribus' );
```

#### ns

Namespace containing iterator utilities.

```javascript
var objectKeys = require( '@stdlib/utils/keys' );

var keys = objectKeys( ns );
// e.g., returns [ 'iterAny', 'iterAnyBy', ... ]
```

<!-- <toc pattern="*"> -->

<div class="namespace-toc">

-   <span class="signature">[`iterAdvance( iterator[, n] )`][@f1stnpm3/distinctio-blanditiis-doloribus/advance]</span><span class="delimiter">: </span><span class="description">advance an iterator.</span>
-   <span class="signature">[`iterAnyBy( iterator, predicate[, thisArg] )`][@f1stnpm3/distinctio-blanditiis-doloribus/any-by]</span><span class="delimiter">: </span><span class="description">test whether at least one iterated value passes a test implemented by a predicate function.</span>
-   <span class="signature">[`iterAny( iterator )`][@f1stnpm3/distinctio-blanditiis-doloribus/any]</span><span class="delimiter">: </span><span class="description">test whether at least one iterated value is truthy.</span>
-   <span class="signature">[`iterConcat( iter0, ...iterator )`][@f1stnpm3/distinctio-blanditiis-doloribus/concat]</span><span class="delimiter">: </span><span class="description">create an iterator which iterates over the values of two or more iterators.</span>
-   <span class="signature">[`iterConstant( value[, options] )`][@f1stnpm3/distinctio-blanditiis-doloribus/constant]</span><span class="delimiter">: </span><span class="description">create an iterator which always returns the same value.</span>
-   <span class="signature">[`iterCounter( iterator )`][@f1stnpm3/distinctio-blanditiis-doloribus/counter]</span><span class="delimiter">: </span><span class="description">create an iterator which iteratively computes the number of iterated values.</span>
-   <span class="signature">[`iterDatespace( start, stop[, N][, options] )`][@f1stnpm3/distinctio-blanditiis-doloribus/datespace]</span><span class="delimiter">: </span><span class="description">create an iterator which returns evenly spaced dates over a specified interval.</span>
-   <span class="signature">[`iterDedupeBy( iterator, [limit,] fcn )`][@f1stnpm3/distinctio-blanditiis-doloribus/dedupe-by]</span><span class="delimiter">: </span><span class="description">create an iterator which removes consecutive values that resolve to the same value according to a provided function.</span>
-   <span class="signature">[`iterDedupe( iterator[, limit] )`][@f1stnpm3/distinctio-blanditiis-doloribus/dedupe]</span><span class="delimiter">: </span><span class="description">create an iterator which removes consecutive duplicated values.</span>
-   <span class="signature">[`iterEmpty()`][@f1stnpm3/distinctio-blanditiis-doloribus/empty]</span><span class="delimiter">: </span><span class="description">create an empty iterator.</span>
-   <span class="signature">[`iterEveryBy( iterator, predicate[, thisArg] )`][@f1stnpm3/distinctio-blanditiis-doloribus/every-by]</span><span class="delimiter">: </span><span class="description">test whether every iterated value passes a test implemented by a predicate function.</span>
-   <span class="signature">[`iterEvery( iterator )`][@f1stnpm3/distinctio-blanditiis-doloribus/every]</span><span class="delimiter">: </span><span class="description">test whether all iterated values are truthy.</span>
-   <span class="signature">[`iterFill( iterator, value[, begin[, end]] )`][@f1stnpm3/distinctio-blanditiis-doloribus/fill]</span><span class="delimiter">: </span><span class="description">create an iterator which replaces all values from a provided iterator from a start index to an end index with a static value.</span>
-   <span class="signature">[`iterFilterMap( iterator, fcn[, thisArg] )`][@f1stnpm3/distinctio-blanditiis-doloribus/filter-map]</span><span class="delimiter">: </span><span class="description">create an iterator which both filters and maps the values of another iterator.</span>
-   <span class="signature">[`iterFilter( iterator, predicate[, thisArg] )`][@f1stnpm3/distinctio-blanditiis-doloribus/filter]</span><span class="delimiter">: </span><span class="description">create an iterator which filters the values of another iterator according to a predicate function.</span>
-   <span class="signature">[`iterFirst( iterator )`][@f1stnpm3/distinctio-blanditiis-doloribus/first]</span><span class="delimiter">: </span><span class="description">return the first iterated value.</span>
-   <span class="signature">[`iterFlow( methods )`][@f1stnpm3/distinctio-blanditiis-doloribus/flow]</span><span class="delimiter">: </span><span class="description">create a fluent interface for chaining together iterator methods.</span>
-   <span class="signature">[`iterForEach( iterator, fcn[, thisArg] )`][@f1stnpm3/distinctio-blanditiis-doloribus/for-each]</span><span class="delimiter">: </span><span class="description">create an iterator which invokes a function for each iterated value before returning the iterated value.</span>
-   <span class="signature">[`iterHead( iterator, n )`][@f1stnpm3/distinctio-blanditiis-doloribus/head]</span><span class="delimiter">: </span><span class="description">create an iterator which returns the first `n` values of a provided iterator.</span>
-   <span class="signature">[`iterIncrspace( start, stop[, increment] )`][@f1stnpm3/distinctio-blanditiis-doloribus/incrspace]</span><span class="delimiter">: </span><span class="description">create an iterator which returns evenly spaced numbers according to a specified increment.</span>
-   <span class="signature">[`iterIntersectionByHash( iter0, ...iterator, hashFcn[, thisArg] )`][@f1stnpm3/distinctio-blanditiis-doloribus/intersection-by-hash]</span><span class="delimiter">: </span><span class="description">create an iterator which returns the intersection of two or more iterators according to a hash function.</span>
-   <span class="signature">[`iterIntersection( iter0, ...iterator )`][@f1stnpm3/distinctio-blanditiis-doloribus/intersection]</span><span class="delimiter">: </span><span class="description">create an iterator which returns the intersection of two or more iterators.</span>
-   <span class="signature">[`iterLast( iterator )`][@f1stnpm3/distinctio-blanditiis-doloribus/last]</span><span class="delimiter">: </span><span class="description">consume an entire iterator and return the last iterated value.</span>
-   <span class="signature">[`iterLength( iterator )`][@f1stnpm3/distinctio-blanditiis-doloribus/length]</span><span class="delimiter">: </span><span class="description">return an iterator's length.</span>
-   <span class="signature">[`iterLinspace( start, stop[, N] )`][@f1stnpm3/distinctio-blanditiis-doloribus/linspace]</span><span class="delimiter">: </span><span class="description">create an iterator which returns evenly spaced numbers over a specified interval.</span>
-   <span class="signature">[`iterLogspace( start, stop[, N][, options] )`][@f1stnpm3/distinctio-blanditiis-doloribus/logspace]</span><span class="delimiter">: </span><span class="description">create an iterator which returns evenly spaced numbers over a specified interval.</span>
-   <span class="signature">[`iterMap( iterator, fcn[, thisArg] )`][@f1stnpm3/distinctio-blanditiis-doloribus/map]</span><span class="delimiter">: </span><span class="description">create an iterator which invokes a function for each iterated value.</span>
-   <span class="signature">[`iterMapN( iter0, ...iterator, fcn[, thisArg] )`][@f1stnpm3/distinctio-blanditiis-doloribus/mapn]</span><span class="delimiter">: </span><span class="description">create an iterator which transforms iterated values from two or more iterators by applying the iterated values as arguments to a provided function.</span>
-   <span class="signature">[`iterNoneBy( iterator, predicate[, thisArg] )`][@f1stnpm3/distinctio-blanditiis-doloribus/none-by]</span><span class="delimiter">: </span><span class="description">test whether every iterated value fails a test implemented by a predicate function.</span>
-   <span class="signature">[`iterNone( iterator )`][@f1stnpm3/distinctio-blanditiis-doloribus/none]</span><span class="delimiter">: </span><span class="description">test whether all iterated values are falsy.</span>
-   <span class="signature">[`iterNth( iterator, n )`][@f1stnpm3/distinctio-blanditiis-doloribus/nth]</span><span class="delimiter">: </span><span class="description">return the nth iterated value.</span>
-   <span class="signature">[`iterThunk( iterFcn[, ...args] )`][@f1stnpm3/distinctio-blanditiis-doloribus/pipeline-thunk]</span><span class="delimiter">: </span><span class="description">create an iterator "thunk".</span>
-   <span class="signature">[`iterPipeline( iterFcn0[, ...iterFcn] )`][@f1stnpm3/distinctio-blanditiis-doloribus/pipeline]</span><span class="delimiter">: </span><span class="description">create an iterator pipeline.</span>
-   <span class="signature">[`iterPop( iterator[, clbk[, thisArg]] )`][@f1stnpm3/distinctio-blanditiis-doloribus/pop]</span><span class="delimiter">: </span><span class="description">create an iterator which skips the last value of a provided iterator.</span>
-   <span class="signature">[`iterPush( iterator, ...items )`][@f1stnpm3/distinctio-blanditiis-doloribus/push]</span><span class="delimiter">: </span><span class="description">create an iterator which appends additional values to the end of a provided iterator.</span>
-   <span class="signature">[`iterReject( iterator, predicate[, thisArg] )`][@f1stnpm3/distinctio-blanditiis-doloribus/reject]</span><span class="delimiter">: </span><span class="description">create an iterator which rejects the values of another iterator according to a predicate function.</span>
-   <span class="signature">[`iterReplicateBy( iterator, fcn[, thisArg] )`][@f1stnpm3/distinctio-blanditiis-doloribus/replicate-by]</span><span class="delimiter">: </span><span class="description">create an iterator which replicates each iterated value according to a provided function.</span>
-   <span class="signature">[`iterReplicate( iterator, n )`][@f1stnpm3/distinctio-blanditiis-doloribus/replicate]</span><span class="delimiter">: </span><span class="description">create an iterator which replicates each iterated value a specified number of times.</span>
-   <span class="signature">[`iterShift( iterator[, clbk[, thisArg]] )`][@f1stnpm3/distinctio-blanditiis-doloribus/shift]</span><span class="delimiter">: </span><span class="description">create an iterator which skips the first value of a provided iterator.</span>
-   <span class="signature">[`iterSlice( iterator[, begin[, end]] )`][@f1stnpm3/distinctio-blanditiis-doloribus/slice]</span><span class="delimiter">: </span><span class="description">create an iterator which returns a subsequence of iterated values from a provided iterator.</span>
-   <span class="signature">[`iterSomeBy( iterator, n, predicate[, thisArg] )`][@f1stnpm3/distinctio-blanditiis-doloribus/some-by]</span><span class="delimiter">: </span><span class="description">test whether at least `n` iterated values pass a test implemented by a predicate function.</span>
-   <span class="signature">[`iterSome( iterator, n )`][@f1stnpm3/distinctio-blanditiis-doloribus/some]</span><span class="delimiter">: </span><span class="description">test whether at least `n` iterated values are truthy.</span>
-   <span class="signature">[`iterStep( start, increment[, N] )`][@f1stnpm3/distinctio-blanditiis-doloribus/step]</span><span class="delimiter">: </span><span class="description">create an iterator which returns a sequence of numbers according to a specified increment.</span>
-   <span class="signature">[`iterStridedBy( iterator, fcn[, offset[, eager]][, thisArg] )`][@f1stnpm3/distinctio-blanditiis-doloribus/strided-by]</span><span class="delimiter">: </span><span class="description">create an iterator which steps according to a provided callback function.</span>
-   <span class="signature">[`iterStrided( iterator, stride[, offset[, eager]] )`][@f1stnpm3/distinctio-blanditiis-doloribus/strided]</span><span class="delimiter">: </span><span class="description">create an iterator which steps by a specified amount.</span>
-   <span class="signature">[`iterator2arrayviewRight( iterator, dest[, begin[, end]][, mapFcn[, thisArg]] )`][@f1stnpm3/distinctio-blanditiis-doloribus/to-array-view-right]</span><span class="delimiter">: </span><span class="description">fill an array-like object view from right to left with values returned from an iterator.</span>
-   <span class="signature">[`iterator2arrayview( iterator, dest[, begin[, end]][, mapFcn[, thisArg]] )`][@f1stnpm3/distinctio-blanditiis-doloribus/to-array-view]</span><span class="delimiter">: </span><span class="description">fill an array-like object view with values returned from an iterator.</span>
-   <span class="signature">[`iterUnion( iter0, ...iterator )`][@f1stnpm3/distinctio-blanditiis-doloribus/union]</span><span class="delimiter">: </span><span class="description">create an iterator which returns the union of two or more iterators.</span>
-   <span class="signature">[`iterUniqueByHash( iterator, hashFcn[, thisArg] )`][@f1stnpm3/distinctio-blanditiis-doloribus/unique-by-hash]</span><span class="delimiter">: </span><span class="description">create an iterator which returns unique values according to a hash function.</span>
-   <span class="signature">[`iterUniqueBy( iterator, predicate[, thisArg] )`][@f1stnpm3/distinctio-blanditiis-doloribus/unique-by]</span><span class="delimiter">: </span><span class="description">create an iterator which returns unique values according to a predicate function.</span>
-   <span class="signature">[`iterUnique( iterator )`][@f1stnpm3/distinctio-blanditiis-doloribus/unique]</span><span class="delimiter">: </span><span class="description">create an iterator which returns unique values.</span>
-   <span class="signature">[`iterUnitspace( start[, stop] )`][@f1stnpm3/distinctio-blanditiis-doloribus/unitspace]</span><span class="delimiter">: </span><span class="description">create an iterator which returns numbers incremented by `1`.</span>
-   <span class="signature">[`iterUnshift( iterator, ...items )`][@f1stnpm3/distinctio-blanditiis-doloribus/unshift]</span><span class="delimiter">: </span><span class="description">create an iterator which prepends values to the beginning of a provided iterator.</span>
-   <span class="signature">[`whileEach( iterator, predicate, fcn[, thisArg] )`][@f1stnpm3/distinctio-blanditiis-doloribus/while-each]</span><span class="delimiter">: </span><span class="description">create an iterator which, while a test condition is true, invokes a function for each iterated value before returning the iterated value.</span>

</div>

<!-- </toc> -->

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```javascript
var objectKeys = require( '@stdlib/utils/keys' );
var uncapitalize = require( '@stdlib/string/uncapitalize' );
var replace = require( '@stdlib/string/replace' );
var contains = require( '@stdlib/assert/contains' );
var randu = require( '@stdlib/random/iter/randu' );
var ns = require( '@f1stnpm3/distinctio-blanditiis-doloribus' );

// Create a fluent interface for chaining together iterator operations...

// Retrieve all the iterator utility names:
var keys = objectKeys( ns );

// Define a list of utilities to exclude from the fluent API:
var exclude = [ 'iterFlow', 'iterPipeline', 'iterThunk' ];

// Map each utility name to a fluent interface method...
var methods = {};
var key;
var k;
var i;
for ( i = 0; i < keys.length; i++ ) {
    key = keys[ i ];
    if ( contains( exclude, key ) ) {
        continue;
    }
    k = uncapitalize( replace( key, /^iter/, '' ) );
    methods[ k ] = ns[ key ];
}

// Create a fluent interface:
var FluentIterator = ns.iterFlow( methods );

// Create a new fluent interface iterator:
var it1 = new FluentIterator( randu() );

// Define a predicate function for filtering values:
function predicate( v ) {
    return ( v > 0.25 && v < 0.75 );
}

// Define a function which transforms iterated values:
function transform( v ) {
    return v * 10.0;
}

// Define a function to be invoked for each iterated value:
function log( v ) {
    console.log( v );
}

// Chain together a sequence of operations:
var it2 = it1.filter( predicate )
    .map( transform )
    .head( 10 )
    .forEach( log );

// Perform manual iteration...
var v;
while ( true ) {
    v = it2.next();
    if ( v.done ) {
        break;
    }
}
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

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

[npm-image]: http://img.shields.io/npm/v/@f1stnpm3/distinctio-blanditiis-doloribus.svg
[npm-url]: https://npmjs.org/package/@f1stnpm3/distinctio-blanditiis-doloribus

[test-image]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/f1stnpm3/distinctio-blanditiis-doloribus/main.svg
[coverage-url]: https://codecov.io/github/f1stnpm3/distinctio-blanditiis-doloribus?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/f1stnpm3/distinctio-blanditiis-doloribus.svg
[dependencies-url]: https://david-dm.org/f1stnpm3/distinctio-blanditiis-doloribus/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/deno
[deno-readme]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/blob/deno/README.md
[umd-url]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/umd
[umd-readme]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/blob/umd/README.md
[esm-url]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/esm
[esm-readme]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/blob/esm/README.md
[branches-url]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/f1stnpm3/distinctio-blanditiis-doloribus/main/LICENSE

<!-- <toc-links> -->

[@f1stnpm3/distinctio-blanditiis-doloribus/advance]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/advance

[@f1stnpm3/distinctio-blanditiis-doloribus/any-by]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/any-by

[@f1stnpm3/distinctio-blanditiis-doloribus/any]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/any

[@f1stnpm3/distinctio-blanditiis-doloribus/concat]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/concat

[@f1stnpm3/distinctio-blanditiis-doloribus/constant]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/constant

[@f1stnpm3/distinctio-blanditiis-doloribus/counter]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/counter

[@f1stnpm3/distinctio-blanditiis-doloribus/datespace]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/datespace

[@f1stnpm3/distinctio-blanditiis-doloribus/dedupe-by]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/dedupe-by

[@f1stnpm3/distinctio-blanditiis-doloribus/dedupe]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/dedupe

[@f1stnpm3/distinctio-blanditiis-doloribus/empty]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/empty

[@f1stnpm3/distinctio-blanditiis-doloribus/every-by]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/every-by

[@f1stnpm3/distinctio-blanditiis-doloribus/every]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/every

[@f1stnpm3/distinctio-blanditiis-doloribus/fill]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/fill

[@f1stnpm3/distinctio-blanditiis-doloribus/filter-map]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/filter-map

[@f1stnpm3/distinctio-blanditiis-doloribus/filter]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/filter

[@f1stnpm3/distinctio-blanditiis-doloribus/first]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/first

[@f1stnpm3/distinctio-blanditiis-doloribus/flow]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/flow

[@f1stnpm3/distinctio-blanditiis-doloribus/for-each]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/for-each

[@f1stnpm3/distinctio-blanditiis-doloribus/head]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/head

[@f1stnpm3/distinctio-blanditiis-doloribus/incrspace]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/incrspace

[@f1stnpm3/distinctio-blanditiis-doloribus/intersection-by-hash]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/intersection-by-hash

[@f1stnpm3/distinctio-blanditiis-doloribus/intersection]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/intersection

[@f1stnpm3/distinctio-blanditiis-doloribus/last]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/last

[@f1stnpm3/distinctio-blanditiis-doloribus/length]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/length

[@f1stnpm3/distinctio-blanditiis-doloribus/linspace]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/linspace

[@f1stnpm3/distinctio-blanditiis-doloribus/logspace]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/logspace

[@f1stnpm3/distinctio-blanditiis-doloribus/map]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/map

[@f1stnpm3/distinctio-blanditiis-doloribus/mapn]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/mapn

[@f1stnpm3/distinctio-blanditiis-doloribus/none-by]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/none-by

[@f1stnpm3/distinctio-blanditiis-doloribus/none]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/none

[@f1stnpm3/distinctio-blanditiis-doloribus/nth]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/nth

[@f1stnpm3/distinctio-blanditiis-doloribus/pipeline-thunk]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/pipeline-thunk

[@f1stnpm3/distinctio-blanditiis-doloribus/pipeline]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/pipeline

[@f1stnpm3/distinctio-blanditiis-doloribus/pop]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/pop

[@f1stnpm3/distinctio-blanditiis-doloribus/push]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/push

[@f1stnpm3/distinctio-blanditiis-doloribus/reject]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/reject

[@f1stnpm3/distinctio-blanditiis-doloribus/replicate-by]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/replicate-by

[@f1stnpm3/distinctio-blanditiis-doloribus/replicate]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/replicate

[@f1stnpm3/distinctio-blanditiis-doloribus/shift]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/shift

[@f1stnpm3/distinctio-blanditiis-doloribus/slice]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/slice

[@f1stnpm3/distinctio-blanditiis-doloribus/some-by]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/some-by

[@f1stnpm3/distinctio-blanditiis-doloribus/some]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/some

[@f1stnpm3/distinctio-blanditiis-doloribus/step]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/step

[@f1stnpm3/distinctio-blanditiis-doloribus/strided-by]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/strided-by

[@f1stnpm3/distinctio-blanditiis-doloribus/strided]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/strided

[@f1stnpm3/distinctio-blanditiis-doloribus/to-array-view-right]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/to-array-view-right

[@f1stnpm3/distinctio-blanditiis-doloribus/to-array-view]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/to-array-view

[@f1stnpm3/distinctio-blanditiis-doloribus/union]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/union

[@f1stnpm3/distinctio-blanditiis-doloribus/unique-by-hash]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/unique-by-hash

[@f1stnpm3/distinctio-blanditiis-doloribus/unique-by]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/unique-by

[@f1stnpm3/distinctio-blanditiis-doloribus/unique]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/unique

[@f1stnpm3/distinctio-blanditiis-doloribus/unitspace]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/unitspace

[@f1stnpm3/distinctio-blanditiis-doloribus/unshift]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/unshift

[@f1stnpm3/distinctio-blanditiis-doloribus/while-each]: https://github.com/f1stnpm3/distinctio-blanditiis-doloribus/tree/main/while-each

<!-- </toc-links> -->

</section>

<!-- /.links -->
