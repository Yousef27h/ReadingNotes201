# Lifting State Up

every component in React has its own state. Because of this sometimes data can be redundant and inconsistent. So, by Lifting up the state we make the state of the parent component as a single source of truth and pass the data of the parent in its children.

__lifting state up__ is the process of moving the sharing state up to the closest common ancestor of the components that need it, and it becomes the "source of truth" for the child components.

There should be a single “source of truth” for any data that changes in a React application. Usually, the state is first added to the component that needs it for rendering. Then, if other components also need it, we can lift it up to their closest common ancestor. Instead of trying to sync the state between different components.

Lifting state involves more writing code than local state approches, but it takes less work to find and locate bugs. since a state lives in some component and only that component can change it, the bugs are greatly reduced. 


# Lists and Keys

In order to render multiple components, we can build collections of elements and include them in JSX using curly braces:

```
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  <li>{number}</li>
);
```

then we include entir `listItems` array inside a _ul_ element :
```
ReactDOM.render(
  <ul>{listItems}</ul>,
  document.getElementById('root')
);
```

__Keys__ help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity:

```
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  <li key={number.toString()}>
    {number}
  </li>
);
```

We should include the key when extracting components:
```
function ListItem(props) {
  // Correct! There is no need to specify the key here:
  return <li>{props.value}</li>;
}

function NumberList(props) {
  const numbers = props.numbers;
  const listItems = numbers.map((number) =>
    // Correct! Key should be specified inside the array.
    <ListItem key={number.toString()} value={number} />
  );
  return (
    <ul>
      {listItems}
    </ul>
  );
}

const numbers = [1, 2, 3, 4, 5];
ReactDOM.render(
  <NumberList numbers={numbers} />,
  document.getElementById('root')
);
```

In the code above, if we extract a `ListItem` component, we should keep the key on the `ListItem` elements in the array rather than on the `li` element in the `ListItem` itself.

Keys have to be unique among their siblings, but they don't have to be globally unique.


## Spread Operator
 
spread syntax refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.

The spread syntax “spreads” the array into separate arguments:

```
Math.max(1,3,5) // 5
Math.max([1,3,5]) // NaN
Math.max(...[1,3,5]) // 5
```

Useful tasks a spread operator can do:

* Copying an array
* Concatenating or combining arrays
* Using Math functions
* Using an array as arguments
* Adding an item to a list
* Adding to state in React
* Combining objects
* Converting NodeList to an array

The spread operator … is useful for working with arrays and objects in JavaScript. It is a convenient feature added in ES6 (ES2015).

