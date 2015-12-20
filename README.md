# JavaScript Methods

Here is a collection of JavaScript Methods that available or can be made available with the help of polyfills.

## Array

#### Array.prototype ([here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/prototype))

It is a property that represents the prototype for the *Array* constructor.

***Features:***<br>
&nbsp;&nbsp;&nbsp; 1) *Array.prototype* itself is an Array.
<br>
&nbsp;&nbsp;&nbsp; 2) *Array.prototype.constructor* specifies the function that creates an object's prototype.
<br>
&nbsp;&nbsp;&nbsp; 3) *Array.prototype.length* reflects the number of elements in an Array which is similar to Array.length.

***Browser compatibility:***<br>
&nbsp;&nbsp;&nbsp; It supports in all browsers including desktop as well as mobile.

***Example:***<br>
```javascript

var x = [1, 2, 3, 4, 5];
console.log(x.length); // 5

```

#### Array.from() ([here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/from))

It creates a new Array instance from an array-like or iterable object.

***Syntax:***<br>
&nbsp;&nbsp;&nbsp;Array.from(arrayObject[, mapFunction[, thisArgument]])

***Parameters:***<br>
&nbsp;&nbsp;&nbsp;arrayObject - An array-like or iterable object to convert to an array.<br>
&nbsp;&nbsp;&nbsp;mapFunction - Optional. Map function (function(element, index) {}) to call on every element of the array.<br>
&nbsp;&nbsp;&nbsp;thisArgument - Optional. Value to use as this when executing mapFn.<br>

***Browser compatibility:***<br>
&nbsp;&nbsp;&nbsp; It supports in fewer browsers but can be used in all browsers with [polyfill](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/from#Polyfill).

***Example:***<br>
```javascript

var x = [1, 2, 3, 4, 5];

var y = Array.from(x);

var z = Array.from(x, function(element, index) {
    return element * index;
});

console.log(y); // [1, 2, 3, 4, 5]
console.log(z); // [0, 2, 6, 12, 20]

```













# License ([MIT](https://opensource.org/licenses/MIT))

Copyright (c) 2015

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
