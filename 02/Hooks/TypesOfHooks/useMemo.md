# useMemo

- It returns a memorized value.

- The useMemo and useCallback Hooks are similar. The main difference is that useMemo returns a memoized value and useCallback returns a memoized function.

## Why useCallBack is not working for objects, function?
 In Javascript 2 function and object are not equal even if they holds same value and functionality, as they hold different address in memory hence useMemo is effective there.

 ## code syntax
 ```
  const calculation = useMemo(() => expensiveCalculation(count), [count]);
  ```