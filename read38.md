1. How granular should your reducers be?
*The concept of a Reducer became popular in JavaScript with the rise of Redux as state management solution for React. ... Basically reducers are there to manage state in an application. For instance, if a user writes something in an HTML input field, the application has to manage this UI state (e.g. controlled components)*

2. Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched
*Not always we need to fire all reducer in one action dispatch*

3. Name a strategy for preventing the above
*Using Redux middleware thunk, allows for evaluating the actions*

### store:
*Holds the whole state tree of the application, only way to change the state inside is to dispatch an action on it*

### combined reducers:
*helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore . The resulting reducer calls every child reducer, and gathers their results into a single state object*

## Redux Thunk
*is a middleware that lets you call action creators that return a function instead of an action object. That function receives the store's dispatch method, which is then used to dispatch regular synchronous actions inside the function's body once the asynchronous operations have been completed*

### what is the additional with thunk?
*With a plain basic Redux store, you can only do simple synchronous updates by dispatching an action. Middleware extends the store's abilities, and lets you write async logic that interacts with the store.*

### Using Redux Thunk in a Sample Application
*The most common use case for Redux Thunk is for communicating asynchronously with an external API to retrieve or save data. Redux Thunk makes it easy to dispatch actions that follow the lifecycle of a request to an external API*

- *install thunk npm install redux-thunk then import it*