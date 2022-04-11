# Uncontrolled components

It is similar to the traditional HTML form inputs. Here, the form data is handled by the DOM itself.
It maintains their own state and will be updated when the input value changes. To write an uncontrolled component, there is no need to write an event handler for every state update, and you can use a ref to access the value of the form from the DOM.