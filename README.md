# What I learned Week 8

## "For Of" loop.

The For Of loop is a nice way to clean up some code by shorten it up a bit. For of lets you loop over data structures that are iterable like Arrays, Strings, Maps, etc.

**Example**

for (variable of iterable) {
    statement
}

- The variable inside the brackets on every iteration the value of the property is assigned to the variable.
- The iterable is a object which has enumerable properties and can be iterated upon.

Heres an example of it in action!

---

const iterable = ['mini', 'mani', 'mo'];

for (const value of iterable) {
  console.log(value);
}

// Output:
// mini
// mani
// mo

---

## Filtering

We also went over filtering arrays this week. Which is going through an array and filtering out certain elements and pushing the ones we want into a new array.

There is also a array method called *.filter()* that will also shorten and clean up your code. This method creates a new array with elements that fall under a given criteria from an existing array.

Here are two examples of filtering one without the filter method and one with.

---

const shortNamesOnly = function (names) {
  let result = [];

  for (const shortNames of names) {
    if (shortNames.length < 7) {
      result.push(shortNames)
    }
  }
  return result;
}


const numbers = [1, 3, 6, 8, 11];

let lucky = numbers.filter(function(number) {
  return number > 7;
});

// [ 8, 11 ]

---


## Some methods used this week

- startsWith() - Determines whether a string begins with the characters of a specified string, returning true or false as appropriate.
- includes() - Checks if array includes the item passed in the method.


