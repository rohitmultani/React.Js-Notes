# Props
- Props stand for "Properties." They are read-only components. It is an object which stores the value of attributes of a tag and work similar to the HTML attributes. It gives a way to pass data from one component to other components. It is similar to function arguments. Props are passed to the component in the same way as arguments passed in a function.

In Car Compenent we can use it like this.
```
function Car(props) {
  return <h2>I am a { props.brand }!</h2>;
}
```

In App.js we can pass like this.
```
const myelement = <Car brand="Ford" />;
```