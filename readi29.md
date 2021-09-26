# Redux - Combined Reducers

![React](https://ms314006.github.io/static/b7a8f321b0bbc07ca9b9d22a7a505ed5/97b31/React.jpg)

1. Why choose Redux instead of the Context API for global state?

Context API is easy to is use as it has a short learning curve. It requires less code, and because there's no need of extra libraries, bundle sizes are reduced. Redux on the other hand requires adding more libraries to the application bundle. The syntax is complex and extensive creating unnecessary work and complexity.

2. What is the purpose of a reducer?

A reducer is a function that determines changes to an application's state. It uses the action it receives to determine this change. We have tools, like Redux, that help manage an application's state changes in a single store so that they behave consistently

3. What does an action contain?

Actions are the only source of information for the store as per Redux official documentation. It carries a payload of information from your application to store

4. Why do we need to copy the state in a reducer?

If the new state is different, the reducer must create new object, and making a copy is a way to describe the unchanged part.

* **combineReducers** combineReducers is simply a utility function to simplify the most common use case when writing Redux reducers. You are not required to use it in your own application, and it does not handle every possible scenario

* The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore.

The resulting reducer calls every child reducer, and gathers their results into a single state object. The state produced by combineReducers() namespaces the states of each reducer under their keys as passed to combineReducers()

![combineReducers](https://user-images.githubusercontent.com/6775736/72829182-93b6d480-3c7e-11ea-925b-77d9a57d705f.png)