1. When you have multiple contexts, what component type should you use (class/function) and why?
*React needs to make each context consumer a separate node in the tree. If two or more context values are often used together, you might want to consider creating your own render prop component that provides both*

2. What are some good use cases for using the Context API for global state?
*Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult. If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context*

3. How can you best test context?
- *We can then make use of the ThemeContext in the `<BlogPost />` component*
- *This type of test is available if both the provider and consumer are used within the component that you want to test such as in the case of `<Page />`*

### context:
* the parts of a discourse that surround a word or passage and can throw light on its meaning.the interrelated conditions in which something exists or occurs : environment, setting the historical context of the war*

### useContext():
*“useContext” hook is used to create common data that can be accessed throughout the component hierarchy without passing the props down manually to each level. Context defined will be available to all the child components without involving “props”*

### static context:
*A static method or, block belongs to the class and these will be loaded into the memory along with the class. You can invoke static methods without creating an object*

## When to Use Context?

*Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language*

## Before You Use Context?

*Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult*

### Context.displayName
*Context object accepts a displayName string property. React DevTools uses this string to determine what to display for the context*