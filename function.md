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
