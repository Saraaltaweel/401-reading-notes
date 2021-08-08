1. How does React differ from vanilla JS/HTML/CSS?
- *Vanilla JS requires a lot of typing*
- *Vanilla JS is fragile*
- *React JS is for code organization*
- *React JS files are reusable*

2. What is the primary difference between a function component and a class component?
*A functional component is just a plain JavaScript function that accepts props as an argument and returns a React element. A class component requires you to extend from React. Component and create a render function which returns a React element. There is no render method used in functional components*


### Functional Components:
*basic JavaScript functions. These are typically arrow functions but can also be created with the regular function keyword. Sometimes referred to as “dumb” or “stateless” components as they simply accept data and display them in some form; that is they are mainly responsible for rendering UI*

### Children / Child Components:
*My simple explanation of what this.props.children does is that it is used to display whatever you include between the opening and closing tags when invoking a component.*

## Why Hooks?
*We know that components and top-down data flow help us organize a large UI into small, independent, reusable pieces. However, we often can’t break complex components down any further because the logic is stateful and can’t be extracted to a function or another component. Sometimes that’s what people mean when they say React doesn’t let them “separate concerns.”*


## Hook 
*A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components. *

## When would I use a Hook?
*If you write a function component and realize you need to add some state to it, previously you had to convert it to a class. Now you can use a Hook inside the existing function component. *