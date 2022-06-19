# React Animations
In React, we can add animation using an explicit group of components known as the React Transition Group.
React Transition Group is an add-on component for managing component states and useful for defining entering and exiting transitions. 
React Transition group has mainly two APIs to create transitions.

# Installation
` npm install react-transition-group --save `

React Transition Group API provides three main components. These are:

1. Transition
2. CSSTransition
3. Transition Group

# Transition

It has a simple component API to describe a transition from one component state to another over time. It is mainly used to animate the mounting and unmounting of a component. It can also be used for in-place transition states as well.
We can access the Transition component into four states:

1. entering
2. entered
3. exiting
4. exited

# CSSTransition

The CSSTransition component uses CSS stylesheet classes to write the transition and create animations. It is inspired by the ng-animate library. It can also inherit all the props of the transition component. We can divide the "CSSTransition" into three states.
1. Appear
2. Enter
3. Exit

CSSTransition component must be applied in a pair of class names to the child components. The first class is in the form of name-stage and the second class is in the name-stage-active. For example, you provide the name fade, and when it applies to the 'enter' stage, the two classes will be fade-enter and fade-enter-active. It may also take a prop as Timeout which defines the maximum time to animate.

# TransitionGroup

This component is used to manage a set of transition components (Transition and CSSTransition) in a list.
It is a state machine that controls the mounting and unmounting of components over time. 