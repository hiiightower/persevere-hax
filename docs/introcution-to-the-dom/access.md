---
layout: default
title: c. Access Elements in the DOM
parent: 1. Understanding the DOM
---


# Accessing and Selecting Elements in the DOM
The first step of making a web page interactive is grabbing ahold of elements you want the user to interact with. This is called selection. In order to be proficient at accessing elements in the DOM, it is necessary to have a working knowledge of CSS selectors, syntax and
terminology as well as an understanding of HTML elements. There are a number of ways to select elements on a web page. Let's explore those you are likely to use most often.

---

# Overview
In order to be proficient at accessing elements in the DOM, it is necessary to have a working knowledge of CSS selectors, syntax and terminology as well as an understanding of HTML elements. In this tutorial, we will go over several ways to access elements in the DOM: by ID, class, tag, and query selectors.


| **Gets**          | **Selector Syntax** | **Method**                 |
| ----------------- | ------------------- | -------------------------- |
| ID                | `#demo`             | `getElementById()`         |
| Class             | `.demo`             | `getElementsByClassName()` |
| Tag               | `demo`              | `getElementsByTagName()`   |
| Selector (single) |                     | `querySelector()`          |
| Selector (all)    |                     | `querySelectorAll()`       |



### Accessing Elements by ID
The easiest way to access a single element in the DOM is by its unique ID. We can grab an element by ID with the getElementById() method of the document object.


### Accessing Elements by Class
The class attribute is used to access one or more specific elements in the DOM. We can get all the elements with a given class name with the getElementsByClassName() method.

### Accessing Elements by Tag
A less specific way to access multiple elements on the page would be by its HTML tag name. We access an element by tag with the getElementsByTagName() method.

### Query Selectors
If you have any experience with the jQuery API, you may be familiar with jQuery’s method of accessing the DOM with CSS selectors.

