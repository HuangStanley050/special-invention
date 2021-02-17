### Creating arrays

1. Basic way

```javascript
const array = [1, 2, 3];
```

2. Array constructor

```javascript
const array = new Array(1, 2, 3);
```

3. Spread operator

```javascript
const blah = [1, 2, 3];

const newBlah = [...blah, 4];
```

4. From another array

```javascript
const Animals = new Array("panda", "lion", "pig", "fox");
const copyOfAnimals = Array.from(Animals);
```

5. Form Objects using Object.keys and Object.values

```javascript
const days = {
  1: "Monday",
  2: "Tuesday",
  3: "Wednesday",
  4: "Thursday",
  5: "Friday",
  6: "Saturday",
  7: "Sunday",
};

const keys = Object.keys(days);
const values = Object.values(days);
```

6. Array concat meethod

```javascript
const birds = ["duck", "owl"];
const moreBirds = [].concat(birds, "eagle", ["parrot"]);
```

### Useful array methods

1. concat - merge arrays

2. includes - look for value

3. indexOf - find index of a particular value

4. join - make a string out of an array

5. reverse

6. slice - copy portion of an array

7. splice - remove and replace elements

8. sort
