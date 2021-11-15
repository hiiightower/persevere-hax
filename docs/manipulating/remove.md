---
layout: default
title: Removing Existing Elements from DOM
parent: 3. Manipulating Elements
---


## Removing Existing Elements from DOM
Similarly, you can use the removeChild() method to remove a child node from the DOM. 


---


### Definition and Usage
{: .no_toc }
The `removeChild` method removes an element from the DOM structure. 

<!-- First, select the last list item using the querySelector() method.
Then, select the parent element of the list item using the parentElement and call the removeChild() method on the parent element.
The `childNode` is the child node of the `parentNode` that you want to remove. If the `childNode` is not the child node of the `parentNode`, the method throws an exception. -->

<!-- The `removeChild()` returns the removed child node from the DOM tree but keeps it in the memory, which can be used later. -->

### Syntax
{: .no_toc }
<!-- parent - Parent node whose child is to be removed
child - Node which will be removed
{: .bg-grey-dk-250 .code-example .text-grey-dk-000} -->

```js
parent.removeChild(child)
```


### Example
{: .no_toc }

The following example uses the removeChild() to remove the last list item:
{: .bg-grey-dk-250 .code-example .text-grey-dk-000}

```js
<ul id="menu">
    <li>Home</li>
    <li>Products</li>
    <li>About Us</li>
</ul>

let menu = document.getElementById('menu');
menu.removeChild(menu.lastElementChild);
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
The following example uses the removeChild() to remove the last list item:
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
