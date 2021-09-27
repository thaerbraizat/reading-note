# Redux - Asynchronous Actions

![React](https://ms314006.github.io/static/b7a8f321b0bbc07ca9b9d22a7a505ed5/97b31/React.jpg)

1. How granular should your reducers be?

It’s very easy to go full-warp with very specific events, dedicated for every change that occurs when a user is editing forms such as CHANGE_NAME, CHANGE_STREET, CHANGE_AGE, etc…

But it is not actually necessary if the logic behind the update is not different for all those fields. For those parts which require different handling in various reducers; dedicated action is the best solution. For others, sometimes a general action might be good enough

2. Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched?

As with state, serializable actions enable several of Redux's defining features, such as time travel debugging, and recording and replaying actions. Using something like a Symbol for the type value or using instanceof checks for actions themselves would break that. Strings are serializable and easily self-descriptive, and so are a better choice. Note that it is okay to use Symbols, Promises, or other non-serializable values in an action if the action is intended for use by middleware. Actions only need to be serializable by the time they actually reach the store and are passed to the reducers.

We can't reliably enforce serializable actions for performance reasons, so Redux only checks that every action is a plain object, and that the type is defined. The rest is up to you, but you might find that keeping everything serializable helps debug and reproduce issues.

Encapsulating and centralizing commonly used pieces of code is a key concept in programming. While it is certainly possible to manually create action objects everywhere, and write each type value by hand, defining reusable constants makes maintaining code easier. If you put constants in a separate file, you can check your import statements against typos so you can't accidentally use the wrong string.


* **Async Logic and Data Fetching**

![Async]( https://miro.medium.com/max/638/1*gzSOKTC2V-mQhAJ-fc0qIA.jpeg)


![middleware](https://miro.medium.com/max/1838/1*vBeR3yXWcukp_yZpNBtHlg.png)

![middleware](https://pbs.twimg.com/media/DlwKz2UUcAA9cg_.png)


With a plain basic Redux store, you can only do simple synchronous updates by dispatching an action. Middleware extends the store's abilities, and lets you write async logic that interacts with the store.

Thunks are the recommended middleware for basic Redux side effects logic, including complex synchronous logic that needs access to the store, and simple async logic like AJAX requests.

