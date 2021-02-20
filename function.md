### Functions

#### Ways to declare functions in JS

1. Function declaration

```javascript
function isEven(num) {
  return num % 2 === 0;
}
isEven(24); // => true
isEven(11); // => false
```

2. Funtion expression

```javascript
var myFunction = function () {
  statements;
};

var myFunction = function namedFunction() {
  statements;
};

const newSchoolArrowFunction = () => {
  console.log("new way to declare functions");
};
```

#### Higher order function 

The important thing to know is that functions are objects.

Higher order functios are functions that operate on other functions, either by taking them as arguments or by returning them. In simple words, A Higher-Order function is a function that receives a function as an argument or returns the function as output.


**Example 1**:

```javascript 
function formalGreeting() {
  console.log("How are you?");
}
function casualGreeting() {
  console.log("What's up?");
}
function greet(type, greetFormal, greetCasual) {
  if(type === 'formal') {
    greetFormal();
  } else if(type === 'casual') {
    greetCasual();
  }
}
// prints 'What's up?'
greet('casual', formalGreeting, casualGreeting);
```

**Example 2:**

A practical example involve the array method "map", we pass in an arrow function to "map" like:

```javascript
const arr1 = [1, 2, 3];
const arr2 = arr1.map(item => item * 2);
console.log(arr2);
```
