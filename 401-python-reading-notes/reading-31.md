[Conditional Rendering](https://reactjs.org/docs/conditional-rendering.html)

In React, you can create distinct components that encapsulate behavior you need. Then, you can render only some of them, depending on the state of your application.

Element Variables
You can use variables to store elements. This can help you conditionally render a part of the component while the rest of the output doesn’t change.

Preventing Component from Rendering
In rare cases you might want a component to hide itself even though it was rendered by another component. To do this return null instead of its render output.

In the example below, the <WarningBanner /> is rendered depending on the value of the prop called warn. If the value of the prop is false, then the component does not render:

[Lists & Keys](https://reactjs.org/docs/lists-and-keys.html)

Given the code below, we use the map() function to take an array of numbers and double their values. We assign the new array returned by map() to the variable doubled and log it:

const numbers = [1, 2, 3, 4, 5];
const doubled = numbers.map((number) => number * 2);
console.log(doubled);


Basic List Component
Usually you would render lists inside a component.

We can refactor the previous example into a component that accepts an array of numbers and outputs a list of elements.

function NumberList(props) {
  const numbers = props.numbers;
  const listItems = numbers.map((number) =>
    <li>{number}</li>
  );
  return (
    <ul>{listItems}</ul>
  );
}

const numbers = [1, 2, 3, 4, 5];
ReactDOM.render(
  <NumberList numbers={numbers} />,
  document.getElementById('root')
);

[Forms](https://reactjs.org/docs/forms.html)

Controlled Components
In HTML, form elements such as <input>, <textarea>, and <select> typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState().

We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”.

The textarea Tag
In HTML, a <textarea> element defines its text by its children:

<textarea>
  Hello there, this is some text in a text area
</textarea>
In React, a <textarea> uses a value attribute instead. This way, a form using a <textarea> can be written very similarly to a form that uses a single-line input:



[Lifting State](https://reactjs.org/docs/lifting-state-up.html)

Often, several components need to reflect the same changing data. We recommend lifting the shared state up to their closest common ancestor. Let’s see how this works in action.

see article, very indepth example

[Composition vs Inheritance](https://reactjs.org/docs/composition-vs-inheritance.html)

React has a powerful composition model, and we recommend using composition instead of inheritance to reuse code between components.

Specialization
Sometimes we think about components as being “special cases” of other components. For example, we might say that a WelcomeDialog is a special case of Dialog.

In React, this is also achieved by composition, where a more “specific” component renders a more “generic” one and configures it with props:

[Thinking in React](https://reactjs.org/docs/thinking-in-react.html)

React is, in our opinion, the premier way to build big, fast Web apps with JavaScript. It has scaled very well for us at Facebook and Instagram.

Step 1: Break The UI Into A Component Hierarchy

FilterableProductTable (orange): contains the entirety of the example
SearchBar (blue): receives all user input
ProductTable (green): displays and filters the data collection based on user input
ProductCategoryRow (turquoise): displays a heading for each category
ProductRow (red): displays a row for each product

Step 2: Build A Static Version in React

Step 3: Identify The Minimal (but complete) Representation Of UI State

Step 4: Identify Where Your State Should Live

Step 5: Add Inverse Data Flow

And That’s It
Hopefully, this gives you an idea of how to think about building components and applications with React. While it may be a little more typing than you’re used to, remember that code is read far more than it’s written, and it’s less difficult to read this modular, explicit code. As you start to build large libraries of components, you’ll appreciate this explicitness and modularity, and with code reuse, your lines of code will start to shrink. :)

[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)