# useEffect

The useEffect Hook allows you to perform side effects in your components.

## Syntax

useEffect accepts two arguments. The second argument is optional.

useEffect(<function>, <dependency>)

## 3 ways to implement useEffect.
 1. When no dependency passed

 ```
 // here it runs everytime whenever component is rerendered
 useEffect(()=>{});
 ```

 2. An empty array
 ```
 // this will work only at the starting time
 useEffect(()=>{},[]);
 ```

 3. Having some props or state value
 ```
 // this will run whenever 'props' value changes
 useEffect(()=>{},[props]);
 ```
