---
layout: module
permalink: /module2/content2.5/
---

# Hooks in ReactJS

<hr>

`Why use Hooks in ReactJs?`

The main reason to add Hooks in reactjs is to allows user to use state and other React features, like lifecycle methods, without writing a class i.e we can use fetaures like state, lifecycle in functional component limiting the pain of transforming a component, and all of its UI and business logic, from a stateless functional component to a class for using React Features like state,lifecycle.

### 1. State Hook

useState is the hook which we will use for adding the react state in functional component.

```js
import React, { useState } from 'react';

function Example() {
  // Declare a new state variable, which we'll call "count"
  const [count, setCount] = useState(0);

  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>
        Click me
      </button>
    </div>
  );
}
```

In above example,
we have set state variable named count with the inital value of 0.Here,setCount() is used to alter the state count.

The equivalent example is shown below(in class Component):
```js
class Example extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      count: 0
    };
  }

  render() {
    return (
      <div>
        <p>You clicked {this.state.count} times</p>
        <button onClick={() => this.setState({ count: this.state.count + 1 })}>
          Click me
        </button>
      </div>
    );
  }
}

```

### 2. Effect Hook

useEffect Hook can be compared as componentDidMount, componentDidUpdate, and componentWillUnmount combined in React class lifecycle methods.

Example:

```js
import React, { useState, useEffect } from 'react';

function Example() {
  const [count, setCount] = useState(0);

  useEffect(() => {
    document.title = `You clicked ${count} times`;
  });

  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>
        Click me
      </button>
    </div>
  );
}
```
Here,
After the every render, useEffect() is called.

### Rules of Hook
1. Only call Hooks at the top level. Don’t call Hooks inside loops, conditions, or nested functions.
2. Only call Hooks from React function components. Don’t call Hooks from regular JavaScript functions.


<<[Back](/ReactJs/module2/content2.4)&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; [Next Page](/ReactJs/module3/content3.1/)>>