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
 