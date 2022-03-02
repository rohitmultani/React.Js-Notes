# useEffect

The useEffect Hook allows you to perform side effects in your components.

## Syntax

useEffect accepts two arguments. The second argument is optional.

useEffect(<function>, <dependency>)

## 3 ways to implement useEffect.
 1. When no dependency passed
 ```
 useEffect(()=>{});
 ```

 2. An empty array
 ```
 useEffect(()=>{},[]);
 ```
 
 3. Having some props or state value
 ```
 useEffect(()=>{},[props]);
 ```
