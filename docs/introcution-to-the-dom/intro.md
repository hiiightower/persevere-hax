---
layout: default
title: a. Introduction to the DOM
parent: 1. Understanding the DOM
---


# Introduction to the DOM
Remove an element from the DOM tree and insert a new one in its place.

---

### Prerequisites
In order to effectively understand the DOM and how it relates to working with the web, it is necessary to have an existing knowledge of HTML and CSS. It is also beneficial to have familiarity with fundamental JavaScript syntax and code structure.


### Intro
The Document Object Model, usually referred to as the DOM, is an essential part of making websites interactive. It is an interface that allows a programming language to manipulate the content, structure, and style of a website. JavaScript is the client-side scripting language that connects to the DOM in an internet browser.

Almost any time a website performs an action, such as rotating between a slideshow of images, displaying an error when a user attempts to submit an incomplete form, or toggling a navigation menu, it is the result of JavaScript accessing and manipulating the DOM. In this article, we will learn what the DOM is, how to work with the document object, and the difference between HTML source code and the DOM.

### What is the DOM?
At the most basic level, a website consists of an HTML document. The browser that you use to view the website is a program that interprets HTML and CSS and renders the style, content, and structure into the page that you see.

In addition to parsing the style and structure of the HTML and CSS, the browser creates a representation of the document known as the Document Object Model. This model allows JavaScript to access the text content and elements of the website document as objects.

```html
<!DOCTYPE html>
<html lang="en">

  <head>
    <title>Learning the DOM</title>
  </head>

  <body>
    <h1>Document Object Model</h1>
  </body>

</html>
```

This code is the familiar HTML source of a new website skeleton. It contains the absolute most essential aspects of a website document — a doctype, and an html tag with the head and body nested inside.

For our purposes, we’ll be using the Chrome browser, but you can receive similar output from other modern browser. Within Chrome, open up index.html. You’ll see a plain website with our heading saying “Document Object Model”. Right click anywhere on the page and select “Inspect”. This will open up Developer Tools.

##### What is the Difference Between the DOM and HTML Source Code?
Currently, with this example, it seems that HTML source code and the DOM are the exact same thing. There are two instances in which the browser-generated DOM will be different than HTML source code:

    The DOM is modified by client-side JavaScript
    The browser automatically fixes errors in the source code

Let’s demonstrate how the DOM can be modified by client-side JavaScript. Type the following into the console:

```js
document.body;
```
The console will respond with this output:
```hbs
<!-- Output -->
<body>
  <h1>Document Object Model</h1>
</body>
```