# Component Lifecycle / useEffec

![React](https://ms314006.github.io/static/b7a8f321b0bbc07ca9b9d22a7a505ed5/97b31/React.jpg)

1. Why do we not need more .html pages in a multi-page React app?

react is single web app

2. If we wanted a component to show up on every page, where would we put it and why?

Inside the (BrowserRouter /), outside a (Route)

3. What does routing do with the components that were rendered when a new route is requested?

Routing is the ability to move between different parts of an application when a user enters a URL or clicks an element (link, button, icon, image etc) within the application.

4. What does props.children contain?

props. children does is that it is used to display whatever you include between the opening and closing tags when invoking a component.

5. How do useState() and this.setState() differ?

setState() does not immediately mutate this. state but creates a pending state transition. Accessing this. state after calling this method can potentially return the existing value

* What does useEffect do?
 By using this Hook, you tell React that your component needs to do something after render. React will remember the function you passed (we’ll refer to it as our “effect”), and call it later after performing the DOM updates. In this effect, we set the document title, but we could also perform data fetching or call some other imperative API.

* Why is useEffect called inside a component?
Placing useEffect inside the component lets us access the count state variable (or any props) right from the effect. We don’t need a special API to read it — it’s already in the function scope. Hooks embrace JavaScript closures and avoid introducing React-specific APIs where JavaScript already provides a solution.

* Does useEffect run after every render?
 Yes! By default, it runs both after the first render and after every update. (We will later talk about how to customize this.) Instead of thinking in terms of “mounting” and “updating”, you might find it easier to think that effects happen “after render”. React guarantees the DOM has been updated by the time it runs the effects.
