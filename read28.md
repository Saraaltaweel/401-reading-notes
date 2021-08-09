1. Why do we not need more .html pages in a multi-page React app?
*A React app consists of a single HTML file index. html . The views are coded in JSX format as components. But we sometimes need to build multi-page websites because a single-page website can not always represent complete information*

2. If we wanted a component to show up on every page, where would we put it and why?
- Outside the `<BrowserRouter/>`
- Inside the `<BrowserRouter />`, outside a `<Route />`
*The `<BrowserRouter>` is the more popular of the two because it uses the HTML5 History API to keep your UI in sync with the URL, whereas the `<HashRouter>` uses the hash portion of the URL (window.location.hash). If you need to support legacy browsers that don’t support the History API, you should use `<HashRouter>`. Otherwise `<BrowserRouter>` is the better choice for most use cases. *

- Inside a `<Route />`
*You can place your `<Route>` component anywhere you want your route to be rendered. Since `<Route>`, `<Link>` and all the other React Router APIs that we’ll be dealing with are just components, you can easily get up and running with routing in React.*

3. What does routing do with the components that were rendered when a new route is requested?
*When you use component, the router uses React. createElement to create a new React element from the given component. That means if you provide an inline function to the component prop, you would create a new component every render*

4. What does props.children contain?
*is that it is used to display whatever you include between the opening and closing tags when invoking a component. This component contains an `<img>`*

5. How do `useState()` and `this.setState()` differ?
- *The setState function is used to handle the state object in a React class component*
- *We import {useState} from React and we are able to simply create a state and a function to set that state (state: value, setState: setValue). The initial state of this component is set when calling useState*

### State Hook:
*is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components*

### Mounting and Un-Mounting:
*The mount command mounts a storage device or filesystem, making it accessible and attaching it to an existing directory structure. The umount command "unmounts" a mounted filesystem, informing the system to complete any pending read or write operations, and safely detaching it*

## Using the Effect Hook:

### Effects Without Cleanup
*Sometimes, we want to run some additional code after React has updated the DOM. Network requests, manual DOM mutations, and logging are common examples of effects that don’t require a cleanup. We say that because we can run them and immediately forget about them. Let’s compare how classes and Hooks let us express such side effects*

### Use Multiple Effects to Separate Concerns
One of the problems we outlined in the Motivation for Hooks is that class lifecycle methods often contain unrelated logic, but related logic gets broken up into several methods:
`class FriendStatusWithCounter extends React.Component {`
  `constructor(props) {`
    `super(props);`
    `this.state = { count: 0, isOnline: null };`
    `this.handleStatusChange = this.handleStatusChange.bind(this);`
  `}`

  `componentDidMount() {`
    `document.title = ``You clicked ${this.state.count} times``;`
    `ChatAPI.subscribeToFriendStatus(`
      `this.props.friend.id,`
      `this.handleStatusChange`
    `);`
  `}`

  `componentDidUpdate() {`
    `document.title = ``You clicked ${this.state.count} times``;`
  }

 ` componentWillUnmount() {`
   ` ChatAPI.unsubscribeFromFriendStatus(`
      `this.props.friend.id,`
      `this.handleStatusChange`
   ` );`
 ` }`

 ` handleStatusChange(status) {`
   ` this.setState({`
      `isOnline: status.isOnline`
    `});`
  `}`




