# Putting it all together
## React Docs - thinking in React

*React is the premier way to build big, fast web apps with JavaScript. It makes you think about apps as you build them.
Process for building a searchable product data table using React
Break the UI into a component hierarchy*


## Build a static version in React

*The easiest way is to build a version that takes your data model and renders the UI but has no interactivity.*

*It’s best to decouple these processes because building a static version requires a lot of typing and no thinking, and adding interactivity requires a lot of thinking and not a lot of typing.*


To make your UI interactive, you need to be able to trigger changes to your underlying data model. React does this with state.

Ask three questions about each piece of data to find state:

1. Is it passed in from a parent via props? (If so, it probably isn’t state.)  
2. Does it remain unchanged over time? (If so, it probably isn’t state.)
3.  Can you compute it based on any other state or props in your component? (If so, it isn’t state).

### For each piece of state in your application:

- Identify every component that renders something based on its state

- Find a common owner component (a single component ABOVE all the components that need the state)

- Either the common owner, or another componenet higher up in the hierarchy should own the state.

- If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

- Add inverse data flow



 1. What is the single responsibility principle and how does it apply to components?
    - this principle means that every component should have one function to do, if the component has more than one function then make subcomponents as children to it, every child will do one function.

2. What does it mean to build a ‘static’ version of your application?
    - that is means you will not be able to change your data. in another meaning; you will not use state into your components.

3. Once you have a static application, what do you need to add?
    - you have to make it dynamic, by using states into each component that needs to change its data.

 