 # React and Forms

## Controlled Components
*In HTML, form elements such as \<input>, \<textarea>, and \<select> typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState().

We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”.*

## Forms
1. The textarea Tag
    - in React, a \<textarea> uses a value attribute instead.
2. The select Tag
    - React, instead of using this selected attribute, uses a value attribute on the root select tag. 
3. Handling Multiple Inputs
    - When you need to handle multiple controlled input elements, you can add a name attribute to each element and let the handler function choose what to do based on the value of "event.target.name".
4. Controlled Input Null Value
    - Specifying the value prop on a controlled component prevents the user from changing the input unless you desire so. If you’ve specified a value but the input is still editable, you may have accidentally set value to undefined or null


![f](https://borunov.com/wp-content/uploads/2017/01/Screen-Shot-2017-01-05-at-3.48.22-PM.png)

# The Conditional (Ternary) Operator 

The Conditional (Ternary) Operator:  <br>
First, we’ll take a look at the syntax of a typical if statement:<br>
- if ( condition ) { <br>
  value if true; <br>
} else { <br>
  value if false;<br>
} <br>

Now, the ternary operator: <br>
condition ? value if true : value if false <br>
<br>
<br>

1. The condition is what you’re actually testing. The result of your condition should be true or false or at least coerce to either boolean value.
2. A ? separates our conditional from our true value. Anything between the ? and the : is what is executed if the condition evaluates to true.
3. Finally a : colon. If your condition evaluates to false, any code after the colon is executed.