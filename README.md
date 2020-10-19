# what-i-learned-week-5

## `Mapping` - String Building for Arrays 

The `map`() method creates a new array with the results of calling a function for every array element. The `map`() method calls the provided function once for each element in an array, in order. 

You can see an example below:

```javascript
const myArray = ['Sam', 'Alice', 'Nick', 'Matt'];

// Appends text to each element of the array
const newArray = myArray.map(name => {
	return 'My name is ' + name; 
});
console.log(newArray); // ['My name is Sam', 'My Name is Alice', ...]

// Appends the index of each element with it's value
const anotherArray = myArray.map((value, index) => index + ": " + value);
console.log(anotherArray); // ['0: Sam', '1: Alice', '2: Nick', ...]

// Starting array is unchanged
console.log(myArray); // ['Sam', 'Alice', 'Nick', 'Matt']
```

-----------

## `Filter` 

The `filter`() method creates an array filled with all array elements that pass a test (provided as a function).

```javascript
run.addEventListener("click", function () {
    let array = [];
    people.forEach((elem) => {
      // elem before age to target
      if (elem.age > 18) {
        array.push(elem); // each array elem > 18 is "pushed" inside the new array
        // console.log(array); nope : messes things up
      } else {
        (""); // no need to declare this through console.log
      }
    });
    console.log(array); //and there you have it : filtered array
  });
```
----------
## `For Of Loop`

The JavaScript `for/of` statement loops through the values of an iterable objects.

`for/of` lets you loop over data structures that are iterable such as Arrays, Strings, Maps, NodeLists, and more.

An example of a `for/of`:

```javascript
const array1 = ['a', 'b', 'c'];

for (const element of array1) {
  console.log(element);
}

// expected output: "a"
// expected output: "b"
// expected output: "c"

}
```
----------

## `Data Types`   ---*Examples*  

Week-5 we went over the `object` data type, but wanted to have these examples for ref:

```javascript
//String Data Type
let strSingle = 'John'; //String with single quotes
let strDouble = "Bob"; //String with double quotes
-------------------------------------------------------
//Number Data Type
let num = 25; //Integer
let flo = 80.5; //Floating-point number
let exp = 4.25e+6; //Exponential notation, this equates to 4250000

-------------------------------------------------------
//Boolean Data Type
let isReading = true; //Yes, I'm reading
let isSleeping = false; //No, I'm not sleeping

-------------------------------------------------------
//Undefined Data Type
let undef; //If a value is never assigned, any output will be 'undefined'

-------------------------------------------------------
//Null Data Type
let noValue = null; //Null meaning that it is has no value, not the same as 0 or ""

-------------------------------------------------------
//Object Data Type
let emptyObject = {};
let person = {"name": "Clark", "surname": "Kent", "age": "36"}; //The quotes around the propety name can be omitted if the property name is a valid JS name
let car = { //Same as person but easier to read
	model: "BMW X3", //Example with quotes around property name ommitted
	color: "white",
	doors: 5
}

-------------------------------------------------------
//Array Data Type
let emptyArray = []; //An array can be of any data types (string, number, boolean, etc.)
let array = ["One", "Two"] //String array, note the index of the first element is 0

-------------------------------------------------------
//Function Data Type
let func = function() { //Calling the function: func();
  alert("Code excuted"); //Outputs: Code executed
}
```







