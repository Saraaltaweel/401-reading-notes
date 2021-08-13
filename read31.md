1. Describe use cases useState() vs useReducer()?
*useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks*

2. Why do custom hooks need the use prefix?
*Custom hooks are normal JS functions, named with the prefix 'use', that can use hooks inside of it and contain a common stateful logic to be reused in other components*

3. What do custom hooks usually do?
*Custom Hook is a JavaScript function which we create by ourselves, when we want to share logic between other JavaScript functions. It allows you to reuse some piece of code in several parts of your app*

4. Describe how a hook that fetches API data might work
- *Holding that data that is to be rendered*
- *Page count to make API call*
- *Loading state (show loading screen/component until the data is received from server)*
- *Error state (show error message when something goes wrong while fetching data)*

### reducer:
*The concept of a Reducer became popular in JavaScript with the rise of Redux as state management solution for React. Basically reducers are there to manage state in an application. For instance, if a user writes something in an HTML input field, the application has to manage this UI state (e.g. controlled components)*

## Context

*In a typical React application, data is passed top-down (parent to child) via props, but such usage can be cumbersome for certain types of props (e.g. locale preference, UI theme) that are required by many components within an application*

## Globally Accessible 

*The state of our snackbars (which ones are visible) can be localized to a single centralized component. That same centralized component can be responsible for rendering them. There’s really no need for another component somewhere in the tree to hook into that state (at least not in our use-case)*

## Room for Change

*There’s a lot of buzz around how you can replace a lot of what Redux does with useContext and useReducer. The combination of these two hooks means we can have a global state and use Redux-like reducers, actions, and dispatchers to mutate that global state*