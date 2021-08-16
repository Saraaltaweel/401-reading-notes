1. Why is the Context API useful?
*Context API is a way to enable components to share some data without explicitly passing via each component manually*

2. Can a component outside of a provider get its context?
*React context is available only when the UI is available. This means that on background tasks you can't access it. But that doesn't mean that you can't access it "outside" of components*

3. What are some common use cases for using the Context API?
*
Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult. If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context*

### global state:
*Image result for global state in react Context provides a way to pass data through the component tree without having to pass props down manually at every level, managing state in multiple components that are not directly connected*

### global context:
*is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language*

### consumer:
*is a person or a group who intends to order, orders, or uses purchased goods, products, or services primarily for personal, social, family, household and similar needs, not directly related to entrepreneurial or business activities*

## Some of the designations in an RBAC tool can include:
- *Management role scope – it limits what objects the role group is allowed to manage*
- *Management role group – you can add and remove members*
- *Management role – these are the types of tasks that can be performed by a specific role group*
- *Management role assignment – this links a role to a role group*

## BENEFITS OF RBAC
- Reducing administrative work and IT support
- Maximizing operational efficiency
- Improving compliance

## react-cookies 
*Install*
- $ npm install react-cookies --save


`import cookie from 'react-cookies'`
 
`componentWillMount() {`
  `this.state =  { token: cookie.load('token') }`
 ` // => 123456789`
`}`

