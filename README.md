# Syntax Glossary

> Vanilla syntax for various theories

## Overview

One of the hardest tasks when learning your first programming language is learning how to communicate ideas using this weird new vocabulary.

Inevitably, we learn theories but we struggle writing down the cryptic language constructs.  This repository is an attempt to flush out the vanilla (basic) syntax to help ease development.

---

### Objects

There are two ways to create an object.

**Object Literal**

```js
const something = {}
```

**Class**

```js
class Dog {
  constructor(name) {
    this.name = name
  }
}
```

---

### Functions

There are two types of ways to define functions.  The most common way to create a function is:

**Arrow Function**

```js
() => {}
```

**Class Function**

We can use the object function syntax when we want a function inside of a class or object literal

```js
class Dog {
  bark() {
    // Do something here
  }
}

const dog = new Dog();
dog.bark();

const cat = {
  meow() {
    // Do something here
  }
}
cat.meow();
```

### Arrays

Arrays are collections of values.

**Array of simple types**

```js
const numbers = [1,2,3]
```

**Array of object types**

```js
const people = [
  {
    name: 'Bob',
    age: 20
  },
  {
    name: 'Billy',
    age: 20
  }, 
]
```

We get values out of arrays using an index.  To retrieve billy from above we'd use the following code:

```js
const billy = people[1]
```