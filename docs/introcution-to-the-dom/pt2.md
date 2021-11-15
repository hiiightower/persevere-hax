---
layout: default
title: b. The DOM Part 2
parent: 1. Understanding the DOM
---


# Document Object Model Part 2
Remove an element from the DOM tree and insert a new one in its place.

---

### Introduction
The DOM is often referred to as the DOM tree, and consists of a tree of objects called nodes. In the Introduction to the DOM, we went over what the Document Object Model (DOM) is, how to access the document object and modify its properties with the console, and the difference between HTML source code and the DOM.

### HTML Terminology
Understanding HTML and JavaScript terminology is essential to understanding how to work with the DOM. Let’s briefly review some HTML terminology.

To begin, let’s take a look at this HTML element.
```html
<a href="index.html">Home</a>
```
Here we have an anchor element, which is a link to index.html.

- a is the tag
- href is the attribute
- index.html is the attribute value
- Home is the text.
- Everything between the opening and closing tag combined make the entire HTML element.

### The DOM Tree and Nodes
All items in the DOM are defined as nodes. There are many types of nodes, but there are three main ones that we work with most often:

- Element nodes
- Text nodes
- Comment nodes

When an HTML element is an item in the DOM, it is referred to as an element node. Any lone text outside of an element is a text node, and an HTML comment is a comment node. In addition to these three node types, the document itself is a document node, which is the root of all other nodes.

The DOM consists of a tree structure of nested nodes, which is often referred to as the DOM tree. You may be familiar with an ancestral family tree, which consists of parents, children, and siblings. The nodes in the DOM are also referred to as parents, children, and siblings, depending on their relation to other nodes.

```html
<!DOCTYPE html>
<html>

  <head>
    <title>Learning About Nodes</title>
  </head>

  <body>
    <h1>An element node</h1>
    <!-- a comment node -->
    A text node.
  </body>

</html>
```
The html element node is the parent node. head and body are siblings, children of html. body contains three child nodes, which are all siblings — the type of node does not change the level at which it is nested.




