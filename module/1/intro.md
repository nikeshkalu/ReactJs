---
layout: module
permalink: /module1/content1.1/
---

# Module 1
----
# 1.1 Introduction to ReactJS
ReactJs is frontend JavaScript libray developed by the Facebook for creating the inter- active UIs.ReactJs is not a framework unlike AngularJs.ReactJs can be used as base for development of single web page based application or mobile applications.React also allows us to create reusable UI components.

React Js is widely being used in popular websites like facebook,instagram(web version),Airbnb,Tesla,Netflix and manymore


### Why to use ReactJS?

### Problem:
In traditional web application programming, for even a small change in the webpage, the entire web page needs to be reloaded. This makes the web pages very slower.

### How ReactJS solves this problem?: 
React only updates what’s necessary(necessary components that is to be rendered not an entire webpage).Moreover, React allows developers to create large web applications with complex UIs from small and isolated pieces of code called “components” which can change data, without reloading the entire webpage making it faster solving the above stated problem.

## ReactJS Environmental SetUp
ReactJS can be set up in a number of ways, let’s look at a few of them.
- Using Static HTML file
- “Create React App” via npm

In this beginner guide to ReactJS, we will be dealing only with the static HTML file for learning the basic concepts.However, For doing the various projects in ReactJs we will go through the “Create React App” via npm.

## Adding ReactJs to the HTML pages

```
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
</script>

</body>
</html>

```

Later, In this documentaion we will learn more on React DOM,Babel Compiler,JSX.

 
 <<[Back](/ReactJs/tableOfContent)&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; [Next Page](/ReactJs/module1/content1.2)>>





