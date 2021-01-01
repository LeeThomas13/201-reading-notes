[ES6 Syntax and Feature Overview](https://www.taniarascia.com/es6-syntax-and-feature-overview/)

var x = 0 

let x = 0

ES6 introduced the const keyword, which cannot be redeclared or reassigned, but is not immutable.

The arrow function expression syntax is a shorter way of creating a function expression. Arrow functions do not have their own this, do not have prototypes, cannot be used for constructors, and should not be used as object methods.

Template Literals - let str = `Release Date: ${date}`

multi line strings - let str = `This text
            is on
            multiple lines`

The return keyword is implied and can be omitted if using arrow functions without a block body.

The function keyword can be omitted when assigning methods on an object.

Use curly brackets to assign properties of an object to their own variable.

iterate through an array - 
for (let i of arr) {
  console.log(i)
}

Functions can be initialized with default parameters, which will be used only if an argument is not invoked through the function.

you can use classes in es6

the extends keyword creates a subclass

you can import and export code between files (like python)

Promises represent the completion of an asynchronous function. They can be used as an alternative to chaining functions.



[React - Hello World](https://reactjs.org/docs/hello-world.html)

ReactDOM.render(
  <h1>Hello, world!</h1>,
  document.getElementById('root')
);

It displays a heading saying “Hello, world!” on the page.

[React - JSX](https://reactjs.org/docs/introducing-jsx.html)

const element = <h1>Hello, world!</h1>;
This funny tag syntax is neither a string nor HTML.

It is called JSX, and it is a syntax extension to JavaScript. We recommend using it with React to describe what the UI should look like. JSX may remind you of a template language, but it comes with the full power of JavaScript.

You may use quotes to specify string literals as attributes:

const element = <\div tabIndex="0"></\div>;

JSX prevents user injection - 
It is safe to embed user input in JSX:

const title = response.potentiallyMaliciousInput;
// This is safe:
const element = <h1>{title}</h1>;
By default, React DOM escapes any values embedded in JSX before rendering them. Thus it ensures that you can never inject anything that’s not explicitly written in your application. Everything is converted to a string before being rendered. This helps prevent XSS (cross-site-scripting) attacks.



[React - Rendering Elements](https://reactjs.org/docs/rendering-elements.html)

To render a React element into a root DOM node, pass both to ReactDOM.render():

example:
const element = <h1>Hello, world</h1>;
ReactDOM.render(element, document.getElementById('root'));

React elements are immutable. Once you create an element, you can’t change its children or attributes. An element is like a single frame in a movie: it represents the UI at a certain point in time.

React Only Updates What’s Necessary
React DOM compares the element and its children to the previous one, and only applies the DOM updates necessary to bring the DOM to the desired state.




[React - Components & Props](https://reactjs.org/docs/components-and-props.html)

Components let you split the UI into independent, reusable pieces, and think about each piece in isolation. This page provides an introduction to the idea of components. You can find a detailed component API reference here.

The simplest way to define a component is to write a JavaScript function:

function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}

Extracting Components
Don’t be afraid to split components into smaller components.

For example, consider this Comment component:

function Comment(props) {
  return (
    <div className="Comment">
      <div className="UserInfo">
        <img className="Avatar"
          src={props.author.avatarUrl}
          alt={props.author.name}
        />
        <div className="UserInfo-name">
          {props.author.name}
        </div>
      </div>
      <div className="Comment-text">
        {props.text}
      </div>
      <div className="Comment-date">
        {formatDate(props.date)}
      </div>
    </div>
  );
}

[React - State & Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html)

Consider the ticking clock example from one of the previous sections. In Rendering Elements, we have only learned one way to update the UI. We call ReactDOM.render() to change the rendered output:

However, it misses a crucial requirement: the fact that the Clock sets up a timer and updates the UI every second should be an implementation detail of the Clock.

Ideally we want to write this once and have the Clock update itself:

ReactDOM.render(
  <Clock />,
  document.getElementById('root')
);
To implement this, we need to add “state” to the Clock component.

In applications with many components, it’s very important to free up resources taken by the components when they are destroyed.

We want to set up a timer whenever the Clock is rendered to the DOM for the first time. This is called “mounting” in React.

[React - Handling Events](https://reactjs.org/docs/handling-events.html)

React events are named using camelCase, rather than lowercase.
With JSX you pass a function as the event handler, rather than a string.

When you define a component using an ES6 class, a common pattern is for an event handler to be a method on the class. For example, this Toggle component renders a button that lets the user toggle between “ON” and “OFF” states:

[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)