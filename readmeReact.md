## Expalin React Lifecycle


## What is React Hooks? & What problems do React Hooks solve?
==> React Hooks is a function that lets you use state and other React features without writing a class.React hooks are functions that enable functional components to use state and lifecycle features that were previously only available in class components. 

==> React Hooks solves the problems of sharing the stateful logic between components in a more modular and reusable way than class component.

## How does useState work?
==> The useState Hook enables you to add state to your functional components. It returns a stateful value and a function that can be used to update that value. By using Hooks, you can extract stateful logic from your component

## Reconsilation in react??
==> React uses a reconciliation algorithm(diffing algorithm) to compare a new tree with the most recent tree to determine how to update the user interface. reconsilation akta react er algorithm jeta behind the scene "virtual dom" name known.

## React fiber?
==> React Fiber is a reconciliation algorithm in React 16 that allows for incremental rendering of the virtual DOM. This enables smoother UI updates and better performance for complex applications

## ReactJS State vs Props
==> A state is a variable that exists inside a component, that cannot be accessed and modified outside the component, and can only be used inside the component. Works very similarly to a variable that is declared inside a function that cannot be accessed outside the scope of the function in normal javascript.

==> React allows us to pass information to a Component using something called props (which stands for properties). Props are objects which can be used inside a component. props basically data pass korar way parent to child component e.

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

## babel in react?
==> babel is a transpiler , jeta jsx code k traslate kroe pure js code e then browser k send kore code.

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


## usememo hook in react?
==> useMemo hook is used to get the memoized value of a function in react components. It works on the concept of memoization which refers to caching the output of a function for a given argument to save the computation time. Hence, it improves the application performance.

The useMemo Hook returns a memoized value and prevents the application from unnecessary re-renders. It is useful in heavy computations and processes when using functional components. The useMemo hook helps optimize performance by memoizing expensive calculations.

```
const memoizedValue = useMemo(functionThatReturnsValue, arrayDependencies)
```
useMemo hook is used to enchance the performance in react applications. It stores the output for given arguments as cache and directly return it for same values, preventing unnecessary rerenders and computations.

## React useCallback Hook?

==> React useCallback hook returns a memoized function to reduce unnecessary callbacks. This useCallback hook is used when you have a component in which the child is rerendering again and again without need.

```
const memoizedCallback = useCallback(
    () => {
        doSomething(a, b);
    },    [a, b],
);
```

## React useCallback Hook Usage
This is useful when passing callbacks to optimized child components that rely on reference equality to prevent unnecessary renders.
It improves the performance by reducing the unnecessary computations and providing already stored callback.
It is similar to React useMemo Hook, the difference is it returns a callback and useMemo returns a value.

## ReactJS useContext Hook?
==> Create Context , create provider, pass value, usecontext

React Context is a way to manage state globally.Context provides a way to pass data or state through the component tree without having props drilling.

useContext Consumes context values in functional components.
Helps avoid prop drilling by allowing components to access global or shared state directly.
Commonly used with React’s Context API to manage application-wide states like themes or user authentication.

## What is the Context API?
The Context API is a mechanism that allows you to share specific information (like state or functions) with multiple components, eliminating the need for prop drilling.

## What is the Context API?
The Context API is a mechanism that allows you to share specific information (like state or functions) with multiple components, eliminating the need for prop drilling.

## What is the Context API?
The Context API is a mechanism that allows you to share specific information (like state or functions) with multiple components, eliminating the need for prop drilling.


### React
## What is React?

React is a JavaScript library for building user interfaces, primarily for single-page applications. It allows developers to create reusable UI components and efficiently update the UI using a virtual DOM.

## What is JSX in React?

JSX (JavaScript XML) is a syntax extension that allows writing HTML structures in JavaScript code. React components often use JSX to render elements.

```jsx
Copy
const element = <h1>Hello, world!</h1>;
```
## What are components in React?

Components are the building blocks of React applications. They can be either class-based or function-based and return JSX to define the UI.

## What is the difference between state and props in React?

State: Data that is local to a component and can be changed within the component.
Props: Data passed from parent to child components, which is immutable within the child component.

## What is the use of useState in React?

useState is a Hook that allows you to add state to function components. It returns a pair: the current state and a function to update it.

```jsx
Copy
const [count, setCount] = useState(0);
```
## What is the purpose of useEffect in React?

useEffect is a Hook that allows you to perform side effects (such as data fetching or DOM manipulation) in function components. It runs after every render unless you specify dependencies.

```jsx
Copy
useEffect(() => {
    // side effect code here
}, [dependencies]);
```
## What are React lifecycle methods?

Lifecycle methods are special methods that get called at different stages of a component’s life (like mounting, updating, and unmounting). In function components, useEffect can replace many lifecycle methods.

## What is the difference between functional components and class components?

Functional components: Simpler components that are written as JavaScript functions. They can use Hooks for state and side effects.
Class components: More complex components that are defined using ES6 classes and can have lifecycle methods and state.

## What is a Virtual DOM in React?

The Virtual DOM is a lightweight in-memory representation of the actual DOM. React updates the Virtual DOM first, and then efficiently updates the real DOM, improving performance.

## What is the key prop in React?

The key prop is used to uniquely identify elements in a list, helping React efficiently update and re-render lists of items.

```jsx
Copy
{items.map(item => <li key={item.id}>{item.name}</li>)}
```
## What is React Router?

React Router is a library that enables navigation and routing in React applications. It allows users to move between different views or pages of the application.

## What is context in React?

React's Context API is used to pass data deeply through the component tree without having to explicitly pass props at every level.

## What are hooks in React?

Hooks are functions that allow you to "hook into" React's state and lifecycle features from function components. Examples include useState, useEffect, useContext, etc.

## What is useRef in React?

useRef is a Hook that can store a mutable value that persists across re-renders. It can be used to reference a DOM element or store a value without causing a re-render.

## What is the useMemo hook in React?

useMemo is a Hook that memorizes a calculated value and only recalculates it when one of its dependencies changes. It's useful for optimizing performance.

## What is the useCallback hook in React?

useCallback returns a memoized version of a callback function that only changes if one of the dependencies has changed. It helps to prevent unnecessary re-renders of child components.

## What is prop drilling in React?

Prop drilling refers to the process of passing data through multiple layers of components via props. This can be simplified by using React's Context API.

## What is React.Fragment?

React.Fragment allows you to group multiple elements without adding extra nodes to the DOM.

```jsx
Copy
return (
    <React.Fragment>
        <h1>Title</h1>
        <p>Some content</p>
    </React.Fragment>
);
```

## What is dangerouslySetInnerHTML in React?

dangerouslySetInnerHTML is a property that lets you insert HTML directly into the DOM. It should be used with caution to avoid security risks (e.g., XSS attacks).

## What are controlled and uncontrolled components in React?

Controlled components: Components that use state to control form elements (input, textarea, etc.).
Uncontrolled components: Components that rely on the DOM itself to manage their state.




