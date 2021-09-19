# Context API - Behaviors

![React](https://ms314006.github.io/static/b7a8f321b0bbc07ca9b9d22a7a505ed5/97b31/React.jpg)

1. When you have multiple contexts, what component type should you use (class/function) and why?

The static contextType property won't work if you need more than one, so instead you need to use a context consumer.\

2. What are some good use cases for using the Context API for global state?

Notice what all of the example use cases have in common? None of those cases should change value frequently during a single session. Recognizing that brings us a bit closer to the more specific recommendation – use the Context API to store the data that does not change frequently. If the requirements of your project meet that criteria, you’re good to go. If you’re not sure, let’s dig deeper into this and find out why the frequency of updates matters so much.

3. How can you best test context?

The best way to test Context is to make our tests unaware of its existence and avoiding mocks. We want to test our components in the same way that developers would use them (behavioral testing) and mimic the way they would run in our applications (integration testing).


* **context api** Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language

* **hooks and context example** Our custom hook is now fully operational! We can add alerts easily from anywhere and our provider will display them for us. We could stop here, but there’s room for some optimizations that are pretty easy to achieve.
You’ll notice that value is a new object being created every single time this provider is rendered. That’s not great, because anything consuming this value from the context will potentially also be getting re-rendered.

* **react context links** Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult.

If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context.