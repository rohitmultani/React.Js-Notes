# useReducer

This is similar to useState but holds good when keeping track of multiple complex logic together.

## Syntax
```
useReducer(<reducer>, <initialState>)
```

1. reducer function contains our custom state logic.
2. initial state can be any value but should be object.
3. The useReducer Hook returns the current stateand a dispatchmethod.

## Declaring 
```
const [todos, dispatch] = useReducer(reducer, initialTodos);
```

## InitialTools
```
const initialTodos = [
  {
    id: 1,
    title: "Todo 1",
    complete: false,
  },
  {
    id: 2,
    title: "Todo 2",
    complete: false,
  },
];
```
## Reducer function
```
const reducer = (state, action) => {
  switch (action.type) {
    case "COMPLETE":
      return state.map((todo) => {
        if (todo.id === action.id) {
          return { ...todo, complete: !todo.complete };
        } else {
          return todo;
        }
      });
    default:
      return state;
  }
};
```
