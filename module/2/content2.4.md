---
layout: module
permalink: /module2/content2.4/
---

# Componenet LifeCycle

React component lifecycle executes in four different intervals/phases. These three phases are constructor Mounting, Updating, and Unmounting.Detail explanation about these phases are illustrated below with examples in detail.

### 1. Mounting <br>
Mounting means inserting the element inside the DOM.The methods that are available in this phase are as follow:

	- componentWillMount()
		This method is called exactly before the render() method is called.

	- componentDidMount()	
		This method is called after the render() has been called.

Example:

```js
class LifeCycle extends React.Component {
  componentWillMount() {
      console.log('Component will mount!')
   }
  componentDidMount() {
      console.log('Component did mount!')
   }
  
  render() {
      return (
         <div>
            <h3>Hello mounting methods!</h3>
         </div>
      );
   }
}

```

The output for above code is :
```
Component will mount!
Hello mounting methods!
Component did mount!
```

### 2. Updating <br>

This is the phase when the component gets updated.A component is updated whenever there is a change in the component's state or props.

Various method present at this lifecycle phase is:
- componentWillReceiveProps()
This method is invoked just before the component receives the new props.

- componentWillUpdate()
componentWillUpdate() is invoked just before rendering when new props or state are being received.

Note :You cannot call this.setState() here. If you need to update state in response to a prop change, use componentWillReceiveProps() instead. The reason we do not call this.setState( ) is that the method triggers another componentWillUpdate().

- shouldComponentUpdate()
This method is invoked before re-rendering after new props and/or state are being received. It defaults to true.if shouldComponentUpdate() returns false, then render(), and componentDidMount() will not be invoked

- componentDidUpdate()
componentDidUpdate() is invoked immediately after updating occurs. This method is not called for the initial render.In order words,After the new (updated) component gets updated on the DOM, the ‘componentDidUpdate’ method is executed.

### 3. UnMounting <br>
This is the last phase in component lifecycle.
The methods invloved are:

- componentWillUnmount()
componentWillUnmount() is invoked immediately before a component is unmounted and destroyed.Perform any necessary cleanup in this method, such as invalidating timers, canceling network requests.This method denotes the end of the component’s lifecycle.


Here is a flowchart representation of lifecycle methods
![LifeCycle]({{ site.baseurl }}/images/componentLifeCycle.JPG)


<<[Back](/ReactJs/module2/content2.3)&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; [Next Page](/ReactJs/module2/content2.5/)>>