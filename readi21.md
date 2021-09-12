# useState() Hook

![React](https://ms314006.github.io/static/b7a8f321b0bbc07ca9b9d22a7a505ed5/97b31/React.jpg)

1. How does React differ from vanilla JS/HTML/CSS?

React breaks down the UI into smaller and reusable components that can move around data amongst each other. This breaking down of the UI is what gives React an edge over Vanilla JS. ... This is where React comes in with a great feature i.e its own virtual DOM. The virtual DOM is a shortcut to bypass the manual work.

2. What is the primary difference between a function component and a class component?

A functional component is just a plain JavaScript function that accepts props as an argument and returns a React element. A class component requires you to extend from React. Component and create a render function which returns a React element. There is no render method used in functional components.

3. Why Hooks?
We know that components and top-down data flow help us organize a large UI into small, independent, reusable pieces. However, we often can’t break complex components down any further because the logic is stateful and can’t be extracted to a function or another component. Sometimes that’s what people mean when they say React doesn’t let them “separate concerns.”
These cases are very common and include animations, form handling, connecting to external data sources, and many other things we want to do from our components. When we try to solve these use cases with components alone, we usually end up with:
Huge components that are hard to refactor and test.
Duplicated logic between different components and lifecycle methods.
Complex patterns like render props and higher-order components.

4. What is a Hook?
 A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components.

5. When would I use a Hook?
  If you write a function component and realize you need to add some state to it, previously you had to convert it to a class. Now you can use a Hook inside the existing function component.
