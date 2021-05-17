# Read 03: Readings: Passing Functions as Props



## React Docs - lists and keys:

### What does .map() return?
The map() method returns an entirely new array with transformed elements and the same amount of data. In the case of forEach() , even if it returns undefined , it will mutate the original array with the callback .

### If I want to loop through an array and display each value in JSX, how do I do that in React?
const elements = [] //..some array const items = [] for (const [index, value] of elements. entries()) { items. ...

render() { const elements = ['one', 'two', 'three']; const items = [] for (const [index, value] of elements. ...

render: function() { const elements = ['one', 'two', 'three']; return ( ul {elements.

#### Each list item needs a unique ____.
variable

### What is the purpose of a key?
Keys
Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity.

## The Spread Operator:

### What is the spread operator?
Spread operator to the rescue! It looks similar to rest parameters, also using ..., but does quite the opposite.

### List 4 things that the spread operator can do.
1. Copying an array
2. Concatenating or combining arrays
3. Using Math functions
4. Using an array as arguments
5. Adding an item to a list

### Give an example of using the spread operator to combine two arrays.
const myArray = [`🤪`,`🐻`,`🎌`]
const yourArray = [`🙂`,`🤗`,`🤩`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩

### Give an example of using the spread operator to add a new item to an array.
const fewFruit = ['🍏','🍊','🍌']
const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌" ]

### Give an example of using the spread operator to combine two objects into one.
const objectOne = {hello: "🤪"}
const objectTwo = {world: "🐻"}
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
objectFour.laugh() // 😂😂😂😂😂

## How to Pass Functions Between Components

### In the video, what is the first step that the developer does to pass functions between components?
Creat an arrow function to Pass Data from Child to Parent using Referenced Action he use state

### In your own words, what does the increment function do?

The increment and decrement operators in JavaScript will add one (+1) .

### How can you pass a method from a parent component into a child component?

By using extends like:
class var extends React.Component {
     constructor(props) {
    super(props);
}

### How does the child component invoke a method that was passed to it from a parent component?

In order to execute a function from a child component, you will need to use Refs. React supports a special attribute that you can attach to any component, that's the ref attribute, it takes a callback function, and you can access the functions of the child component in the parent accessing this.refs.REF_NAME.METHOD_NAME.
 this.refs.child.showAlert();




