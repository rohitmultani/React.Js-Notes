# useRef

The useRef Hook is a function that returns a mutable ref object whose .current property is initialized with the passed argument (initialValue). The returned object will persist for the full lifetime of the component.

```
const extractedValue = useRef(initialValue);
```

## When to Use Refs
There are a few good use cases for refs:

1. Managing focus, text selection, or media playback.
2. Triggering imperative animations.
3. Integrating with third-party DOM libraries.

## Why to use Refs
It is mainly use to avoide re-rendering the component, storing the value in useState hooks cause re-renderes everytime, which is not a good way in react.