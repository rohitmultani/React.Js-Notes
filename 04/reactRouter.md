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

- Routes: It’s a new component introduced in the v6 and a upgrade of the component. The main advantages of Routes over Switch are:
Relative s and s
Routes are chosen based on the best match instead of being traversed in order.

- Route: Route is the conditionally shown component that renders some UI when its path matches the current URL.

- Link: Link component is used to create links to different routes and implement navigation around the application. It works like HTML anchor tag.

## Example code
```
import React, { Component } from 'react';
import { BrowserRouter as Router,Routes, Route, Link } from 'react-router-dom';
import Home from './component/home';
import About from './component/about';
import Contact from './component/contact';
import './App.css';

class App extends Component {
render() {
	return (
	<Router>
		<div className="App">
			<ul className="App-header">
			<li>
				<Link to="/">Home</Link>
			</li>
			<li>
				<Link to="/about">About Us</Link>
			</li>
			<li>
				<Link to="/contact">Contact Us</Link>
			</li>
			</ul>
		<Routes>
				<Route exact path='/' element={< Home />}></Route>
				<Route exact path='/about' element={< About />}></Route>
				<Route exact path='/contact' element={< Contact />}></Route>
		</Routes>
		</div>
	</Router>
);
}
}

export default App;
```

## Associated props
1. exact
It is used to match the exact value with the URL. For Eg., exact path=’/about’ will only render the component if it exactly matches the path but if we remove exact from the syntax, then UI will still be rendered even if the strucute is like /about/10. 

2. path: Path specifies a pathname we assign to our component.

3. element: It refers to the component which will render on matching the path.