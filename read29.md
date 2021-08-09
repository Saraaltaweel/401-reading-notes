1. How can we ensure that an effect hook runs only once?
*React has a built-in hook called useEffect. Hooks are used in function components. The Class component comparison to useEffect are the methods componentDidMount , componentDidUpdate , and componentWillUnmount*

2. Can useState() update more than one state variable at the same time?
*no*

3. Is useState() synchronous?
*useState and setState both are asynchronous.Even though they are asynchronous, the useState and setState functions do not return promises*

### State Hook:
*is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components*

### Component Lifecycle:
*can be defined as the series of methods that are invoked in different stages of the component's existence*

## useReducer
`const [state, dispatch] = useReducer(reducer, initialArg, init);`

### Note:
*React guarantees that dispatch function identity is stable and won’t change on re-renders. This is why it’s safe to omit from the useEffect or useCallback dependency list*

## useCallback
`const memoizedCallback = useCallback(`
  `() => {`
    `doSomething(a, b);`
  `},`
  `[a, b],`
`);`

*Pass an inline callback and an array of dependencies. useCallback will return a memoized version of the callback that only changes if one of the dependencies has changed. This is useful when passing callbacks to optimized child components that rely on reference equality to prevent unnecessary renders (e.g. shouldComponentUpdate)*
