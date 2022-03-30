# React Router
React Router is a standard library for routing in React. It enables the navigation among views of various components in a React Application, allows changing the browser URL, and keeps the UI in sync with the URL.

## Adding router dom
```
npm i --save react-router-dom
```

## Importing components
```
import { BrowserRouter, Routes, Route } from "react-router-dom";
```

## Adding components
- BrowserRouter: BrowserRouter is a router implementation that uses the HTML5 history API(pushState, replaceState and the popstate event) to keep your UI in sync with the URL. It is the parent component that is used to store all of the other components.