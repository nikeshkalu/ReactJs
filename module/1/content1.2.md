---
layout: module
permalink: /module1/content1.2/
---

# 1.2 ReactJs Environmental Setup

ReactJS can be set up in a number of ways, let’s look at a few of them.
- Using Static HTML file
- “Create React App” via npm

In this beginner guide to ReactJS, we will be dealing only with the static HTML file for learning the basic concepts.However, For doing the various projects in ReactJs we will go through the “Create React App” via npm.

## Adding ReactJs to the HTML pages(Using Static HTML file)

```html
<!DOCTYPE html>
<html lang="en">
<title>Add ReactJs to HTML Pages</title>

<!-- Adding ReactJs libray for HTML pages to access the ReactJs libray -->
<!-- Load React API -->
<script src="https://unpkg.com/react@16/umd/react.production.min.js">
</script>
<!-- Load React DOM-->
<script src="https://unpkg.com/react-dom@16/umd/react-dom.production.min.js">
</script>
<!-- Load Babel Compiler -->
<script src="https://unpkg.com/babel-standalone@6.15.0/babel.min.js">
</script>

<body>
<div id="root"></div>

<script type="text/babel">
    //  JSX falls here.
    class App extends React.Component { 
            render( ) { 
                return (
                    <h1>Welcome</h1>
                ); 
            } 
        } 
        ReactDOM.render(<App />, document.getElementById('root'));
</script>

</body>
</html>

```

Later, In this documentaion we will learn more on React DOM,Babel Compiler,JSX.

## “Create React App” via npm

Prerequisite:

Install Node.js and npm globally on your machine.

To create react app using terminal.Go inside the terminal and type
```shell
C:\>npx create-react-app myFirstApp
```

Once the react-app is created, move to the newly created directory and start the project by
```shell
C:\>cd myFirstApp
C:\myFirstApp>npm start
```
Once you run this command. In your browser, a new window will pop up at localhost:3000 with your new React app.

![npmStart]({{ site.baseurl }}/images/npmStart.png)


