1. What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?
*The most 'redux-like' way of handling the pre-loading of data would be to fire off the asynchronous action in the lifecycle method (probably componentWillMount ) of a Higher Order Component that wraps your app*

2. When using a thunk/async action that dispatches the actual action, which do you export from your reducer?
*Thunk is for communicating asynchronously with an external API to retrieve or save data. Redux Thunk makes it easy to dispatch actions that follow the lifecycle of a request to an external API*


### middleware:
*Code you put in between the framework receiving a request and the framework generating the response*

### thunk:
*Function that wraps an expressio to delay its evaluation*


## Redux Toolkit
*The official, opinionated, batteries-included toolset for efficient Redux development*

## MobX
- *is a simple, scalable and battle tested state management solution. This tutorial will teach you all the important concepts of MobX in ten minutes*
- *MobX is a standalone library, but most people are using it with React and this tutorial focuses on that combination*

## Hookstate
*The simple but incredibly fast and flexible state management that is based on React state hook*