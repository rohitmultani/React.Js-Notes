# useState

The React useState Hook allows us to track state in a function component.

## Importing useState
To use the useState Hook, we first need to import it into our component.
```
import { useState } from "react";
```
 ## Initialising
 useState accepts an initial value/state and return two value:
 1. Value of current state
 2. A function that updates that state

 ```
 const [color, setColor] = useState("orange");
 ```

 In the above code when react code renders very first time it sets color=orange,
 setColor is the state updating function

 useState can be used to give values like string, number, boolean, arrays, objects.
 

 ## Example to demonstrate working useState Hook

 ```
 import React, { useState } from 'react';

function App() {
const [click, setClick] = useState(0);
const onClickHandler=()=>{
    setClick(click+1);
};
return (
	<div>
<p>You clicked {click} times</p>
	<button onClick={onClickHandler}>
		Click me
	</button>
	</div>
);
}

export default App;

```