## Expalin React Lifecycle


## What is React Hooks? & What problems do React Hooks solve?
==> React Hooks is a function that lets you use state and other React features without writing a class.React hooks are functions that enable functional components to use state and lifecycle features that were previously only available in class components. 

==> React Hooks solves the problems of sharing the stateful logic between components in a more modular and reusable way than class component.

## How does useState work?
==> The useState Hook enables you to add state to your functional components. It returns a stateful value and a function that can be used to update that value. By using Hooks, you can extract stateful logic from your component

## Reconsilation in react??
==> React uses a reconciliation algorithm to compare a new tree with the most recent tree to determine how to update the user interface. reconsilation akta react er algorithm jeta behind the scene "virtual dom" name known.

## React fiber?
==> React Fiber is a reconciliation algorithm in React 16 that allows for incremental rendering of the virtual DOM. This enables smoother UI updates and better performance for complex applications

## ReactJS State vs Props
==> A state is a variable that exists inside a component, that cannot be accessed and modified outside the component, and can only be used inside the component. Works very similarly to a variable that is declared inside a function that cannot be accessed outside the scope of the function in normal javascript.

==> React allows us to pass information to a Component using something called props (which stands for properties). Props are objects which can be used inside a component.

## Difference between state & props

==> props: 
1/ The Data is passed from one component to another.
2/ It is Immutable (cannot be modified).
3/ Props can be used with state and functional components.
4/ Props are read-only.

==> State:
1/ The Data is passed within the component only.
2/ It is Mutable ( can be modified).
3/ The state is both read and write.

## what is lifting the state up?
==> 

## What is event bubbling in React?
==> In event bubbling, the event starts at the most deeply nestd element,then bubbling up, triggering handlers on its parent elements upward till each reaches the top of the dom trees.

## How do you resolve event bubbling?
==> In event object there are a function called stoppropagation(), when it called inside an event handler then it stops prevent the event from bubbling up to any other elements.

## What is useEffect Hooks?
==> useEffect Hooks is used to connect component to an external system. In this the depenedeny array specifies when the effect should run based on changes in its dependencies and when the dependency array is absent in useEffect, the effect will run after every render.

When you provide dependencies in the dependency array of useEffect, the effect will run:

Initially after the first render.
Whenever any of the dependencies change between renders.
If the dependencies are an empty array ( [] ), the effect will only run once after the initial render, similar to componentDidMount in class components.

## When would you use useRef?
useRef is used in React functional components when you need to keep a mutable value around across renders without triggering a re-render. It's commonly used for accessing DOM elements, caching values, or storing mutable variables. You can use useRef to manage focus within your components, such as focusing on a specific input element when a condition is met without triggering re-renders.

