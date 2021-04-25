## React 
React is  a declarative, efficient, and flexible JavaScript library for building user interfaces. It lets you compose complex UIs from small and isolated pieces of code called “components”.

A **component** takes in parameters, called props (short for “properties”), and returns a hierarchy of views to display via the render method.
The render method returns a _description_ of what you want to see on the screen. React takes the description and displays the result. In particular, render returns a **React element**, which is a lightweight description of what to render.

**JSX** is a syntax extension to JavaScript, it looks like this:
```const element = <h1>Hello, world!</h1>;```

Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called “components” that contain both.

After compilation, JSX expressions become regular JavaScript function calls and evaluate to JavaScript objects.

Since JSX is closer to JavaScript than to HTML, React DOM uses camelCase property naming convention instead of HTML attribute names.
For example, `class` becomes `className` in JSX, and `tabindex` becomes `tabIndex`.


### Rendering an Element into the DOM

if we have a <div> somewhere in our HTML file:

`<div id="root"></div>`

We call this a “root” DOM node because everything inside it will be managed by React DOM.

To render a React element into a root DOM node, pass both to `ReactDOM.render()`:

```
const element = <h1>Hello, world</h1>;
ReactDOM.render(element, document.getElementById('root'));
```

React elements are **immutable**. Once you create an element, you can’t change its children or attributes. 

The only way to update the UI is to create a new element, and pass it to `ReactDOM.render()`.

### Components and Props

Components let you split the UI into independent, reusable pieces, and think about each piece in isolation. They are like JavaScript functions. They accept arbitrary inputs (called “props”) and return React elements describing what should appear on the screen.

We can either use a JavaScript function or ES6 class to define a component.

for example, using ES6 class:
```
class Welcome extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}
```

When React sees an element representing a user-defined component, it passes JSX attributes and children to this component as a single object. We call this object __props__.

For example:

```
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}

const element = <Welcome name="Sara" />;
ReactDOM.render(
  element,
  document.getElementById('root')
);
```

Whether we declare a component as a function or a class, it must never modify its own props, props are __read-only__.