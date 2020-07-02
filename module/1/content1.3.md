---
layout: module
permalink: /module1/content1.3/
---

##JSX(JavaScript + XML)

JSX stands for JavaScript XML. JSX is not JavaScript nor HTML.
Eg: const element = <h1>Welcome</h1>

JSX produces React “elements” which we will explore rendering them to the DOM in the next section.

The React Code without using JSX are:
```js
class App extends React.Component {
  render() {
    return (
      React.createElement(
        'div',
        'Welcome'
      )
    );
  }
}
```

Above code creates <div>welcome<div> and returns that value.The code presented above is a bit
difficult to write code.	

To overcome that problem,JSX is used.
JSX looks like regular HTML code in most cases.

#### Using JSX 

```js
import React from 'react';

class App extends React.Component {
   render() {
      return (
         ///This is JSx
         <div>
            Welcome
         </div>
         ///This is JSX
      );
   }
}
export default App;
```

In above code the value returned 
```html
		<div>
            Welcome
         </div>
```
is JSX. 

The JSX is translated to regular JavaScript at runtime using Babel Compiler.Here the above returned value gets translated as (JS Delivered to Browser)
```js
 React.createElement(
        'div',
        'Welcome'
      )
```

and creates the React element of 'div'.

Since, JSX is easier to understand. Most of programmer prefer using JSX.However,React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code. It also allows React to show more useful error and warning messages.