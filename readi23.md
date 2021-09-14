# Advanced State with Reducers

![React](https://ms314006.github.io/static/b7a8f321b0bbc07ca9b9d22a7a505ed5/97b31/React.jpg)

1. How can we ensure that an effect hook runs only once?

you can give it an empty array as second argument.

2. Can useState() update more than one state variable at the same time?

You could combine the loading state and data state into one state object and then you could do one setState call and there will only be one render. Note: Unlike the setState in class components, the setState returned from useState doesn't merge objects with existing state, it replaces the object entirely.

3. Is useState() synchronous?

useState and setState both are asynchronous. They do not update the state immediately but have queues that are used to update the state object. This is done to improve the performance of the rendering of React components. Even though they are asynchronous, the useState and setState functions do not return promises.

* useReducer

useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.

useReducer is one of the additional Hooks that shipped with React 16.8. An alternative to the useState Hook, it helps you manage complex state logic in React applications. When combined with other Hooks like useContext, useReducer can be a good alternative to Redux or MobX — indeed, it can sometimes be an outright better option.

How does useReducer work?
useReducer is used to store and update states, just like the useState Hook. It accepts a reducer function as its first parameter and the initial state as the second.

useReducer returns an array that holds the current state value and a dispatch function, to which you can pass an action and later invoke. This is similar to the pattern Redux uses but with a few differences.
