# JavaScript Methods

Here is a collection of JavaScript Methods that available or can be made available with the help of polyfills.

##Array

####Array.prototype ([here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/prototype))

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
console.log(x.length);

```

####Array.from() ([here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/from))

It creates a new Array instance from an array-like or iterable object.

***Syntax:***<br>
&nbsp;&nbsp;&nbsp;Array.from(arrayObject[, mapFunction[, thisArgument]])

***Parameters:***<br>
&nbsp;&nbsp;&nbsp;arrayObject - An array-like or iterable object to convert to an array.<br>
&nbsp;&nbsp;&nbsp;mapFunction - Optional. Map function (function(element, index) {}) to call on every element of the array.<br>
&nbsp;&nbsp;&nbsp;thisArgument - Optional. Value to use as this when executing mapFn.<br>

***Browser compatibility:***<br>
&nbsp;&nbsp;&nbsp; It supports in fewer browsers but can be used with [polyfill](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/from#Polyfill).




