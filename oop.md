### JS Classes and OOP

**Prototypes are the mechanism by which JavaScript objects inherit features from one another**

What is \__proto\__ in any JS object?

#### MDN definition:

The \__proto\__ property is a simple accessor property on Object. prototype consisting of a getter and setter function. A property access for __proto__ that eventually consults Object. prototype will find this property, but an access that does not consult Object.

In another word, it reference to the prototype of the object which may contains some methods or values that the current object have access to:

For example:

```
const newArray = []

newArray.__proto__.push
```

because the Array object has "push" method inside/defined, so any object created would have acceess to it

So if you use **newArray.push()** JS will look to see if there's method defined within the newArray object and if it can't find it, it will look up the property defined in \__proto\__

```
length: 0
__proto__: Array(0)
concat: ƒ concat()
constructor: ƒ Array()
copyWithin: ƒ copyWithin()
entries: ƒ entries()
every: ƒ every()
fill: ƒ fill()
filter: ƒ filter()
find: ƒ find()
findIndex: ƒ findIndex()
flat: ƒ flat()
flatMap: ƒ flatMap()
forEach: ƒ 
```
