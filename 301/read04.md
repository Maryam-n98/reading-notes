# Read04: Readings: React and Forms:

### Forms:
This form has the default HTML form behavior of browsing to a new page when the user submits the form. If you want this behavior in React, it just works. But in most cases, it’s convenient to have a JavaScript function that handles the submission of the form and has access to the data that the user entered into the form. The standard way to achieve this is with a technique called “controlled components”.

##### Controlled Components
We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”.

#### Handling Multiple Inputs
When you need to handle multiple controlled input elements, you can add a name attribute to each element and let the handler function choose what to do based on the value of event.target.name.

#### Controlled Input Null Value
Specifying the value prop on a controlled component prevents the user from changing the input unless you desire so. If you’ve specified a value but the input is still editable, you may have accidentally set value to undefined or null.

##### Starting With the Basics — The if statement
Using a conditional, like an if statement, allows us to specify that a certain block of code should be executed if a certain condition is met.

#### Conditional Rendering
In React, you can create distinct components that encapsulate behavior you need. Then, you can render only some of them, depending on the state of your application.

Conditional rendering in React works the same way conditions work in JavaScript. Use JavaScript operators like if or the conditional operator to create elements representing the current state, and let React update the UI to match them.

### Element Variables
You can use variables to store elements. This can help you conditionally render a part of the component while the rest of the output doesn’t change.

###### Preventing Component from Rendering
In rare cases you might want a component to hide itself even though it was rendered by another component. To do this return null instead of its render output.

