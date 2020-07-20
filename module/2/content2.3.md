---
layout: module
permalink: /module2/content2.3/
---

# 2.3 Props and State in ReactJs Components

In React Component, Props(short for “properties”)  are the variable passed from one component to another component.In real world sceanrio it is essential for us to pass the value between the components in such scenario we used the props.Most widely, props are passed as attributes from the parent component to child component(similar to function parameters).

Example:

The parent component can pass props as follow:

```js
class ParentComponent extends Component {    
    render() {    
        return (        
            <ChildComponent name="First Child" />    
        );  
    }
}


```
Similarly,Child component can have access to props and use as your wish:

```js
class ChildComponent extends React.Component {
  constructor(props) {
    super(props)
    console.log(props.name)
  }
}
```

`State in Components`:<br>
State is another built-in object in ReactJs, which allows components to create and manage their own data. The behavior of the component at a given moment in time is defined by the state. Components data will be stored in the component’s State. This state can be modified based on user action or other action( onClick,onHover etc).So unlike props, components cannot pass data with state, but they can create and manage it internally.

``When a component state is changed, React will re-render the component to the browser.``

Example:

```js
class Test extends React.Component {    
    constructor() {    
        this.state = {      
            id: 1,      
            name: "demo"    
        };  
    }    
    
    render() {    
        return (      
            <div>        
              <p>{this.state.id}</p>        
              <p>{this.state.name}</p>      
            </div>    
        );  
    }
}

```

``Update the State Component``<br>

State are modified using speical method called setState().

In above example:

```js
this.state.id = “2020”; // wrong

this.setState({         // correct  
    id: "2020"
});

```

Generally,A change in the state happens based on user-input, triggering an event(onClick,onHover,onChange), and so on. Also, React components (with state) are rendered based on the data in the state. State holds the initial information.

``What happens when state is Updated?``<br>

When state gets changed, React re-renders the only the component(not an entire DOM).Thats the main reason why,React is more faster.

In summary, there are 2 important points we need to pay attention to when using state:

- State shouldn’t be modified directly – the setState( ) should be used
- State affects the performance of your app, and therefore it shouldn’t be used unnecessarily

``Does every Component supports state?``

In the early days, state could only be used in class components, not in functional components.

That’s why functional components were also known as stateless components. However, after the introduction of React Hooks, state can now be used both in class and functional components.

If your project is not using React Hooks, then you can only use state in class components.


### State VS Props

- Props are immutable i.e. once set the props cannot be changed, while State is an observable object that is to be used to hold data that may change over time and to control the behavior after each change.

- While Props are set by the parent component, State is generally updated by event handlers

- Components receive data from outside with props, whereas they can create and manage their own data with state





<<[Back](/ReactJs/module2/content2.2)&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; [Next Page](/ReactJs/module2/content2.4)>>
