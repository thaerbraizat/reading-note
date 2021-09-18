# Context API

![React](https://ms314006.github.io/static/b7a8f321b0bbc07ca9b9d22a7a505ed5/97b31/React.jpg)

1. Describe use cases useState() vs useReducer()?

useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.

2. Why do custom hooks need the use prefix?

Custom hooks are normal JS functions, named with the prefix 'use', that can use hooks inside of it and contain a common stateful logic to be reused in other components.

3. What do custom hooks usually do?

Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks.

4. Using any list of custom hooks, research and name one that you think will be useful in your applications?

Custom React Hooks allow us to extract component logic into reusable functions. Custom Hooks look very much like normal helper functions, except they can maintain component state and perform effects. So if you find yourself using a lot of these Hooks, you might as well import the package.

5. Describe how a hook that fetches API data might work?

The most popular type of web API is a Representational state transfer API or RESTful API for short. To be brief, it follows an architecture that uses predefined and stateless operations to access web resources.

Using web APIs requires the use of HTTP requests. Different types of requests include GET, POST, DELETE, PATCH, etc. If you have written some code and it needs to communicate with code somewhere else, it will send an HTTP request over the internet. Next, let’s discuss the HTTP request types just mentioned


* **context api** Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language

* **hooks and context example** Our custom hook is now fully operational! We can add alerts easily from anywhere and our provider will display them for us. We could stop here, but there’s room for some optimizations that are pretty easy to achieve.
You’ll notice that value is a new object being created every single time this provider is rendered. That’s not great, because anything consuming this value from the context will potentially also be getting re-rendered.

* **react context links** Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult.

If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context.