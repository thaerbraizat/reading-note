## React and Forms
![react](https://ms314006.github.io/static/b7a8f321b0bbc07ca9b9d22a7a505ed5/97b31/React.jpg)
1. What is a ‘Controlled Component?
We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a **controlled component**.
2. How do we target what the user is entering if we have an event handler on an input field?
handleChange(event) {
    this.setState({value: event.target.value});
  }

3. Why would we use a ternary operator?
Use the ternary operator to simplify your if-else statements that are used to assign values to variables. The ternary operator is commonly used when assigning post data or validating forms.
4. Rewrite the following statement using a ternary statement:

(x===y) ? console.log(true) : console.log(false)

## Things I want to know more about



### Resource
* [React Docs - Forms](https://reactjs.org/docs/forms.html)
* [The Conditional (Ternary) Operator Explained](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)



