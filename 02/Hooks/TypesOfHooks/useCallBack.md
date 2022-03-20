# useCallBack

We know react renders its components whenever any state change happens, now if a parent component re render, all its child components also execute again, but this is not recommended if the props in the children components do not change, hence we use useCallBack hook in react.

The React useCallback Hook returns a memoized callback function.
This allows us to isolate resource intensive functions so that they will not automatically run on every render.
The useCallback Hook only runs when one of its dependencies update.
This can improve performance.