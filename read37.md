1. Why choose Redux instead of the Context API for global state?
*Redux is the industry standard for managing the state of large applications. It is more optimized for larger projects because the context API re-renders more often*

2. What is the purpose of a reducer?
*A reducer is a function that determines changes to an application's state. It uses the action it receives to determine this change. We have tools, like Redux, that help manage an application's state changes in a single store so that they behave consistently*

3. What does an action contain?
*An action contains a action type and whatever payload you want it to have*

4. Why do we need to copy the state in a reducer?
*The reducer needs to be a pure function without any side-effects. It should only take in an action and return the new state*

### immutable state:
*State cannot be modified, reducers must make copies of existing state to make updates*

### time travel in redux:
*l debugging refers to the ability step forward and backward through the state of you application, empowering the developer understand exactly what is happening at any point in the app's lifecycle*

### action creator:
*is merely a function that returns an action object. Redux includes a utility function called bindActionCreators for binding one or more action creators to the store's dispatch() function*

### reducer:
*Functions that take current state and an action as arguments, and return a new state result, (state, action) => newState*

### dispatch:
*store holds the whole state tree of the application, the only way to change the state inside it is to dispatch an action on it*

## combineReducers
*helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore . The resulting reducer calls every child reducer, and gathers their results into a single state object*

- *As your app grows more complex, you'll want to split your reducing function into separate functions, each managing independent parts of the state*

- *The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore*

- *The resulting reducer calls every child reducer, and gathers their results into a single state object. The state produced by combineReducers() namespaces the states of each reducer under their keys as passed to combineReducers()*
