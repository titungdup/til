Function composition is an approach where the result of one function is passed on to the next function, which is passed to another until the final function is executed for the final result. Function compositions can be composed of any number of functions.

```Javascript
const double = x => x * 2
const square = x => x * x
// Tradition approach
var output1 = double(2);
var output2 = square(output1);
console.log(output2); // Gives 16
// OR
var output_final = square(double(2));
console.log(output_final); // Gives 16
```

Another way is to use Javascript compose and pipe functions.

Source: [Link](https://www.educative.io/answers/function-composition-in-javascript)
