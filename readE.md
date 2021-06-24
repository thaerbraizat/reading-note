## React Docs - thinking in React
![react](https://ms314006.github.io/static/b7a8f321b0bbc07ca9b9d22a7a505ed5/97b31/React.jpg)

1. How would you break a mock into a component heirarchy?
The first thing you’ll want to do is to draw boxes around every component (and subcomponent) in the mock and give them all names
2. What is the single responsibility principle and how does it apply to components?
a component should ideally only do one thing.Separate your UI into components, where each component matches one piece of your data model.
3. What does it mean to build a ‘static’ version of your application?
The easiest way is to build a version that takes your data model and renders the UI but has no interactivity. To build a static version of your app that renders your data model, you'll want to build components that reuse other components and pass data using props.
4. Once you have a static application, what do you need to add?
build components that reuse other components and pass data using props. props are a way of passing data from parent to child, don’t use state at all to build this static version. State is reserved only for interactivity,
5.  What are the three questions you can ask to determine if something is state?
* The search text and the checkbox seem to be state since **they change over time**
* if data come from user
* State is reserved only for interactivity
6. How can you identify where state needs to live?
whenever the user changes the form, we update the state to reflect the user input. Since components should only update their own state, FilterableProductTable will pass callbacks to SearchBar that will fire whenever the state should be updated. We can use the onChange event on the inputs to be notified of it. The callbacks passed by FilterableProductTable will call setState(), and the app will be updated.

## Things I want to know more about