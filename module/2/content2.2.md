---
layout: module
permalink: /module2/content2.2/
---

# 2.2 Types of Component in ReactJs

## 2.2.1 Functional Components(StateLess Component)

This type of component only support props.Props is another way of handling component properties.
Props are like function arguments, and you send them into the component as attributes.Learn more about [Props](/ReactJs/module2/content2.3)

Code sample for this component is:
```js
	function Welcome(props) { 
	 return <h1>
	 		Welcome
	 	</h1>;
}
```


## 2.2.2 Class Components(State Component)

This type of component supports both the state as well as the props.State are used to keep various component properties when certain change occurs in the component.During various events like click,hover,onChange we can change the state of component and hence re-render the component again.

Code sample for this component is:
```js
class Welcome extends React.Component {
  constructor() {
    super();
    this.state = {
    	version: "new"
    };
  }
  render() {
    return <h2>Welcome to {this.state.version} Car!</h2>;
  }
}


````

<<[Back](/ReactJs/module2/content2.1)&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; [Next Page](/ReactJs/module2/content2.3)>>
