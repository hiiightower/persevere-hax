---
layout: default
title: Accessing Elements by ID
parent: 2. Accessing & Selecting DOM Elements
---

# Accessing Elements by ID
The easiest way to access a single element in the DOM is by its unique ID. We can grab an element by ID with the `getElementById()` method of the document object. However, it has drawbacks; an **ID must always be unique to the page,** and therefore you will only ever be able to access a single element at a time with the `getElementById()` method.


## Syntax
{: .fs-4 }
```js
var element = document.getElementById(element-id-here);
```

## Definition and Usage
{: .fs-4 }

The getElementById() method returns the element that has the ID attribute with the specified value.

This method is one of the most common methods in the HTML DOM, and is used almost every time you want to manipulate, or get info from, an element on your document.

Returns null if no elements with the specified ID exists.

An ID should be unique within a page. However, if more than one element with the specified ID exists, the getElementById() method returns the first element in the source code.


#### Important
{: .text-red-300 }
- The `getElementById()` returns a DOM element specified by an id or null if no matching element found.
- If multiple elements share the same id, even though it is invalid, the `getElementById()` returns the first element it encounters.
{: .fs-3 }


---

### Example Code
{: .no_toc .text-gamma .fs-3 }

```html
<html>
    <head>
        <title>JavaScript getElementById() Method</title>
    </head>
    <body>
        <p id="message">A paragraph</p>
    </body>
</html>
```
The document contains a <p> element that has the id attribute with the value message:
{: .fs-2 }

```js
const p = document.getElementById('message');
console.log(p);
```
Output:
{: .fs-2 }
```html
<p id="message">A paragraph</p>
```

---

{: .no_toc }

