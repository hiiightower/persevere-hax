---
layout: default
title: Creating DOM Elements
parent: 3. Manipulating Elements
---


## Create a DOM element
How to create a new element and attach it to the DOM tree.

---

### Definition and Usage
{: .no_toc }

`document.createElement(tagName, [options])` creates a new element of tag type tagName. [options] in this case means you can add some optional parameters to the function. Don’t worry about these at this point.

### Syntax
{: .no_toc }

```js
const div = document.createElement('div');
```
**This function does NOT put your new element into the DOM - it simply creates it in memory.** This is so that you can manipulate the element (by adding styles, classes, ids, text etc.) before placing it on the page. You can place the element into the DOM with one of the following methods.

### Example
{: .no_toc }

Use the `createElement()` method for creating a DOM element:
{: .bg-grey-dk-250 .code-example .text-grey-dk-000}
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

