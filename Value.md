### @@ Array.prototype ([here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/prototype))

It is a property that represents the prototype for the *Array* constructor.

***Syntax:***

```javascript

Array.prototype.length
[].length

```

***Features:***

1) *Array.prototype* itself is an Array.
<br>
2) *Array.prototype.constructor* specifies the function that creates an object's prototype.
<br>
3) *Array.prototype.length* reflects the number of elements in an Array which is similar to Array.length.

***Browser compatibility:***

It supports in all browsers including desktop as well as mobile.

***Example:***

```javascript

var x = [1, 2, 3, 4, 5];
console.log(x.length); // 5

```

### @@ Array() ([here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array))

It is a global object that is used in the construction of arrays; which are high-level, list-like objects.

***Syntax:***

```javascript

[element0, element1, ..., elementN]

new Array(element0, element1[, ...[, elementN]])

new Array(arrayLength)

```

***Parameters:***

elementN - Elements of which to create the array.
<br>
arrayLength - It is the only argument passed to the Array constructor which is an integer between 0 and 2<sup>32</sup>-1 (inclusive) and it serves as the length of the array to be created

***Browser compatibility:***

It supports in all browsers including desktop and mobile.

***Example:***

```javascript

var x = [1, 2, 3, 4, 5];

var y = new Array(1, 2, 3, 4, 5);

var z = new Array(5);

console.log(x);     // [1, 2, 3, 4, 5]
console.log(y);     // [1, 2, 3, 4, 5]
console.log(z);     // an array of 5 empty slots

```

### @@ Array.from() ([here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/from))

It creates a new Array instance from an array-like or iterable object.

***Syntax:***

```javascript

Array.from(arrayObject[, mapFunction[, thisArgument]])

```

***Parameters:***

arrayObject - An array-like or iterable object to convert to an array.
<br>
mapFunction - Optional. Map function (function(element, index) {}) to call on every element of the array.
<br>
thisArgument - Optional. Value to use as this when executing mapFn.

***Browser compatibility:***

It supports in fewer browsers but can be used in all browsers with [polyfill](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/from#Polyfill).

***Example:***

```javascript

var x = [1, 2, 3, 4, 5];

var y = Array.from(x);

var z = Array.from(x, function(element, index) {
    return element * index;
});

console.log(y); // [1, 2, 3, 4, 5]
console.log(z); // [0, 2, 6, 12, 20]

```

### @@ Array.isArray() ([here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/isArray))

It returns true if an object is an array, false if it is not.

***Syntax:***

```javascript

Array.isArray(arrayObject)

```

***Parameters:***

arrayObject - The object to be checked.

***Browser compatibility:***

It supports in all browsers including desktop as well as mobile without [polyfill](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/isArray#Polyfill).

***Example:***

```javascript

Array.isArray([]);                                              // true
Array.isArray([1]);                                             // true
Array.isArray(new Array());                                     // true
Array.isArray(Array.prototype);                                 // true
Array.isArray();                                                // false
Array.isArray({});                                              // false
Array.isArray(null);                                            // false
Array.isArray(undefined);                                       // false
Array.isArray(17);                                              // false
Array.isArray('Array');                                         // false
Array.isArray(Array);                                           // false
Array.isArray(true);                                            // false
Array.isArray(false);                                           // false
Array.isArray({ __proto__: Array.prototype });                  // false
Array.isArray([{a: 1}, {b: 2}]);                                // true
Array.isArray([{a: 1}, {b: 2}, {c: function() { return 1; }}]); // true

```

### @@ Array.of() ([here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/of))

It creates a new Array instance with a variable number of arguments, regardless of number or type of the arguments.

***Syntax:***

```javascript

Array.of(element0[, element1[, ...[, elementN]]])

```

***Parameters:***

elementN - Elements of which to create the array.

***Browser compatibility:***

It supports in fewer browsers but can be used in all browsers with [polyfill](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/of#Polyfill).

***Example:***

```javascript

Array.of(1);            // [ 1 ]
Array.of(1, 2, 3);      // [ 1, 2, 3 ]
Array.of(undefined);    // [ undefined ]
Array.of(true, false);  // [ true, false ]
Array.of(null);         // [ null ]

```

### @@ Array.concat() ([here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/concat))

It returns a new array comprised of the array on which it is called joining the arrays (or values) provided as arguments maintaining the order.

***Syntax:***

```javascript

var newArray = oldArray.concat(array1[, array2[, ...[, arrayN]]])

```

***Parameters:***

arrayN - Arrays (or values) to concatenate into a new array.

***Browser compatibility:***

It supports in all browsers including desktop as well as mobile

***Example:***

```javascript

var num1 = [0],
    num2 = [1, 2, 3],
    num3 = [4, 5],
    num4 = 6;

var nums = num1.concat(num2, num3, num4);

console.log(nums);  // [ 0, 1, 2, 3, 4, 5, 6 ]

```













