---
layout: default
title: Replace a DOM element
parent: 3. Manipulating Elements
---


## Replace a DOM element
Remove an element from the DOM tree and insert a new one in its place.

---


### Definition and Usage
{: .no_toc }

You can also replace an element in HTML DOM with another using the `replaceChild()` method. This method accepts two parameters: the node to insert and the node to be replaced. It has the syntax like `parentNode.replaceChild(newChild, oldChild)`;.


### Syntax
{: .no_toc }

```js
parentNode.replaceChild(newChild, oldChild);
// This method also returns the removed node. 
```


### Example
{: .no_toc }

<!-- This method also returns the removed node. 
{: .fs-2 .fw-300 } -->

```js
// select the element that will be replaced
var el = document.querySelector('div');

// <a href="/javascript/manipulation/creating-a-dom-element-51/">create a new element</a> that will take the place of "el"
var newEl = document.createElement('p');
newEl.innerHTML = '<b>Hello World!</b>';

// replace el with newEL
el.parentNode.replaceChild(newEl, el);
```


<!-- ### Example
{: .no_toc }

Use the `createElement()` method for creating a DOM element:
{: .fs-2 .fw-300 }
```js
var el \= document.createElement('div');
```
Fill the new element with any HTML content:
{: .bg-grey-dk-250 .code-example .text-grey-dk-000}

```js
el.innerHTML \= '<p>Hello World!</p>';
```
Alternatively, use DOM methods for creating content nodes and append them to the new element. This approach requires more code, and is in general slower or equally fast as working with innerHTML:
{: .bg-grey-dk-250 .code-example .text-grey-dk-000}

```js
var textnode \= document.createTextNode('Hello World!');

el.appendChild(textnode); 
```
"el" can now be inserted into the DOM tree:
{: .bg-grey-dk-250 .code-example .text-grey-dk-000}

```js
document.body.appendChild(el);
```
 -->
