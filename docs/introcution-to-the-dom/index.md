---
layout: default
title: 1. Understanding the DOM
nav_order: 1
has_children: true
---

# Understanding the DOM — Document Object Model
The Document Object Model, usually referred to as the `DOM`, is an essential part of making websites interactive. It is an interface that allows a programming language to manipulate the content, structure, and style of a website. JavaScript is the client-side scripting language that connects to the DOM in an internet browser.

---

#### Lessons Plan


## Intro to the DOM
The Document Object Model, usually referred to as the DOM, is an essential part of making websites interactive. It is an interface that allows a programming language to manipulate the content, structure, and style of a website. JavaScript is the client-side scripting...

## The DOM pt2
The DOM is often referred to as the DOM tree, and consists of a tree of objects called nodes. In the Introduction to the DOM, we went over what the Document Object Model (DOM) is, how to access...

## How To Access Elements in the DOM
In order to be proficient at accessing elements in the DOM, it is necessary to have a working knowledge of CSS selectors, syntax and terminology as well as an understanding of HTML elements. In this tutorial, we will go over several ways to access elements in the DOM: by ID, class, tag, and query selectors.

## How To Traverse the DOM
This tutorial will go over how to traverse the DOM (also known as walking or navigating the DOM) with parent, child, and sibling properties.

## How To Make Changes to the DOM
In this tutorial, we will go over how to create new nodes and insert them into the DOM, replace existing nodes, and remove nodes.

## How To Modify Attributes, Classes, and Styles in the DOM
In this tutorial, we will learn how to further alter the DOM by modifying styles, classes, and other attributes of HTML element nodes. This will give you a greater understanding of how to manipulate essential elements within the DOM.

<!-- # Understanding the DOM
## Introduction to the DOM
### Understanding the DOM Tree and Nodes
## How To Access Elements in the DOM

## What is the DOM?
The Document Object Model (DOM) is a programming interface for web documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects; that way, programming languages can interact with the page.

DOM stands for Document Object Model. In the world of web, all HTML webpages are referred to as documents. The Document Object Model represents each of these web pages in a tree-like structure to make it easier to access and manage the elements.


### A document as a hierarchy of nodes
{: .no_toc }

The DOM represents an HTML or XML document as a hierarchy of nodes. Consider the following HTML document:

```html
<html>
    <head>
        <title>JavaScript DOM</title>
    </head>
    <body>
        <p>Hello DOM!</p>
    </body>
</html>
```

In this DOM tree, the document is the root node. The root node has one child which is the `<html>` element. The `<html>` element is called the document element.
Each document can have only one document element. In an HTML document, the document element is the `<html>` element. Each markup can be represented by a node in the tree.
The nodes in the `DOM` are also referred to as parents, children, and siblings, depending on their relation to other nodes.


## Understanding the DOM Tree and Nodes
The `DOM` is often referred to as the DOM tree, and consists of a tree of objects called nodes. All items in the DOM are defined as `nodes`. and `nodes` are the name of any type of object in the DOM tree. It could be one of the built-in DOM elements such as the document itself, document.head or document.body. A node could be an HTML tag specified in the HTML such as `<input>, <div>,<h2>, <p>` or it could be a comment node, text node… In fact, a node is any DOM object and every node has a parent, every node is allowed to have one or more children or even zero children.

### What is an element?
An element is a specific type of node, one that can be directly specified in the HTML with an HTML tag and can have properties like an id or a class. can have children, etc. When an HTML `element` is an item in the DOM, it is referred to as an `element` node. You may be familiar with an ancestral family tree, which consists of parents, children, and siblings. 

<iframe height="300" style="width: 100%;" scrolling="no" title="Simple HTML Page (Now with JavaScript!)" src="https://codepen.io/team/turing/embed/kXwjbv?default-tab=js%2Cresult&editable=true" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/team/turing/pen/kXwjbv">
  Simple HTML Page (Now with JavaScript!)</a> by Turing School of Software and Design (<a href="https://codepen.io/team/turing">@turing</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>


---


##### Notes
Any lone text outside of an element is a text node, and an HTML comment is a comment node.
In addition to these three node types, the **document itself is a document node**, which is the root of all other nodes.

##### Vocab
- `HTML Element` A building block that makes up the structure of a web page.
- `CSS Selector` A way to identify a set elements, typically using a tag, class or id.
- `DOM Document Object Model`, the JS interface used to interact with HTML
- `Event` Any event which takes place in the DOM, these can be generated by users or the browser.
- `EventHandler` A function that will run when a specific event occurs

##### Summary
```
    Summary
    What is the DOM?
    How do we get information out of the DOM and into our JS?
    How do we add information to the DOM?
    How can we change the CSS of elements?
    What is the preferred method for updating our CSS using JS?
``` -->