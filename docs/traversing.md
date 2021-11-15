---
layout: default
title: 3. Traversing the DOM
nav_order: 5
---

# Traversing the DOM
A good JavaScript developer needs to know how to traverse the DOM—it’s the act of selecting an element from another element. Learning how to traverse/navigate the DOM with parent, child, and sibling properties.


{: .no_toc }


Traversing means going up, down, over etc. When you have an element, you often need to select an element based on it's position. There are lots of properties for that, and they all revolve around node and elements.
{: .fs-4 .fw-300 }

---
### Get the Parent of an Element
Get the parent node of an element by using the `parentNode` property of the element.
```js
const current = document.querySelector('#main');
const parent = current.parentNode;
```
##### How it works:
1. First, select the element with the CSS selector #main
2. , use the parentNode property to get the parent element of the selected element.

---


### Get the Closest Element by Selector
To get the closest element by a selector, you use the `element.closest()` method:
```js
const closestElement = targetElement.closest(selector);
```
The `closest()` method starts with the targetElement and travel up to the DOM tree until it finds the element that matches the selector. The method returns null if no such element exists.
{: .fs-2  }
```html
<ul id="one" class="level-1">
  <li class="top-1">Home</li>
  <li id="ii" class="top-2">Products
    <ul class="level-2">
      <li class="category-1">Clothing</li>
      <li class="category-2">Electronics
        <ul class="level-3">
          <li class="product-1">Camera</li>
          <li class="product-2">Computer</li>
          <li class="product-3">Phone</li>
        </ul>
      </li>
      <li class="category-3">Kitchen</li>
    </ul>
  </li>
  <li class="top-3">About</li>
</ul>
```
{: .fs-1  }

The following code selects the list item with the class category-1 and changes the color of the list item to red:
{: .fs-2  }

```js
// start from the category-1
const e = document.querySelector("li.category-1");
e.style.color = 'red';
```
{: .fs-3  }

The following code selects the closest <ul> element of the selected element and changes the background of the selected element to yellow:
{: .fs-2  }

```js
// highlight the closet element
const closet = e.closest("ul");
closet.style.background = 'yellow';
```
{: .fs-3  }



### Get Siblings of an Element
Provide a helper function that returns all siblings of an element.

### Get the Children of an Element
Get all the child elements of an element