# Readings: Passing Functions as Props

## Lists and keys
1. What does .map() return?
map() function returns a map object(which is an iterator) of the results after applying the given function to each item of a given iterable (list, tuple etc.) ... fun : It is a function to which map passes each element of given iterable.
2. If I want to loop through an array and display each value in JSX, how do I do that in React?
data from the object is passed to each block using the JSX handlebars-like curly brackets.
3. Each list item needs a unique key.
4. What is the purpose of a key?
Keys are used to React to identify which items in the list are changed, updated, or deleted. In other words, we can say that keys are used to give an identity to the elements in the lists.

## The spread operator
1. What is the spread operator?
The Spread operator lets you expand an iterable like an object, string, or array into its elements while the Rest operator does the inverse by reducing a set of elements into one array.
2. List 4 things that the spread operator can do?
* Adding to state in React.
* Converting NodeList to an array.
* Using Math functions.
* Using an array as arguments.

## How to pass functions between components
1. what is the first step that the developer does to pass functions between components?
Passing data from a Parent component to Child, simply use **props** in ReactJs to make the child inherit properties from its parent component.
2. what does the increment function do?
it takes a variable and increments (changes) its value, and also returns this value.
3. How can you pass a method from a parent component into a child component?
Passing method as a prop using the arrow function


## Things I want to know more about
 


### Resource
* [Lists and Keys](https://reactjs.org/docs/lists-and-keys.html)
* [The spread operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)
* [How to Pass Functions between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)


