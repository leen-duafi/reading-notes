**What does .map() return?**

new array which will be different than the orginal depending in the code 

**If I want to loop through an array and display each value in JSX, how do I do that in React?**

JSX allows embedding any expression in curly braces so we could inline the map() result

**Each list item needs a unique ____.**

key 

**What is the purpose of a key?**

Keys help React identify which items have changed, are added, or are removed.
special string attribute you need to include when creating lists of elements
Keys used within arrays should be unique among their siblings





**What is the spread operator?**

InJavaScript, spread syntax refers to the use of an ellipsis of three dots (β¦) to expand an iterable object into the list of arguments.

The spread operator was added to JavaScript in ES6 (ES2015), just like the rest parameters, which have the same syntax: three magic dots β¦.




**List 4 things that the spread operator can do.**

* Copying an array
* Concatenating or combining arrays
* Using Math functions
* Using an array as arguments
* Adding an item to a list
* Adding to state in React
* Combining objects
* Converting NodeList to an array




**Give an example of using the spread operator to combine two arrays.**

const myArray = ['π','π','π']

const yourArray = ['π','π','π']

const ourArray = [β¦myArray,β¦yourArray]

console.log(β¦ourArray) // [π π π  π π π]




**Give an example of using the spread operator to add a new item to an array.**

const fruits = ['π','π','π','π','π']
const moreFruits = [...fruits];
console.log(moreFruits) // Array(5) [ "π", "π", "π", "π", "π" ]
fruits[0] = 'π'
console.log(...[...fruits,'...',...moreFruits]) //  π π π π π ... π π π π π





**Give an example of using the spread operator to combine two objects into one.**

const objectOne = {hello: βπ€ͺβ}

const objectTwo = {world: βπ»β}

const objectThree = {β¦objectOne, β¦objectTwo, laugh: βπβ}

console.log(objectThree) // Object { hello: βπ€ͺβ, world: βπ»β, laugh: βπβ }





**In the video, what is the first step that the developer does to pass functions between components?**

create a function wherever the state is the  state  is that we are going to change 



**In your own words, what does the increment function do?**

It takes a variable and increments (changes) its value, and also returns this value. The increment can be a positive or negative number. 



**How can you pass a method from a parent component into a child component?**

 props argument inside  render method which will receive data from  parent component and afterward  passed the event and data using this.props

 

**How does the child component invoke a method that was passed to it from a parent component?**

this state value using setState
