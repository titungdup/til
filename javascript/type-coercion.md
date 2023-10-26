Type Coercion is the process of automatic or implicit conversion of values from one data type to another, such as strings to numbers.

Example:

```Javascript
const value1 = "5";
const value2 = 9;
let sum = value1 + value2;

console.log(sum); // 59
```

Here, value2 is coerced from a number to a string and then concatenated with value1 resulting in a string of 59.

Type conversion is similar to type coercion with one key difference — type coercion is implicit whereas type conversion can be either implicit or explicit.
To return the sum you'd have to explicitly convert the string to a number.

`sum = Number(value1) + value2`
