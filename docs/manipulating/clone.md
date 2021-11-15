---
layout: default
title: Clone an element
parent: 3. Manipulating Elements
---


## Clone an element
Create a deep copy of a DOM element.


---


### Definition and Usage
{: .no_toc }
The `cloneNode()` method creates a copy of a node, and returns the clone.

### Syntax
```
let clone = node.cloneNode(deep);
```


<!-- ### Usage Notes
The `cloneNode()` method clones all attributes and their values. -->
#### Parameters
The `cloneNode()` method accepts an optional parameter `deep`:

``` 
var foo = el.cloneNode(deep);
```
- If the deep is `true`, then the original node and all of its descendants are cloned.
- If the deep is `false`, only the original node will be cloned. All the node’s descendants will not be cloned.
{: .fs-2 .fw-400 }

The deep parameter defaults to `false` if you omit it.




<!-- First, select the last list item using the querySelector() method.
Then, select the parent element of the list item using the parentElement and call the removeChild() method on the parent element.
The `childNode` is the child node of the `parentNode` that you want to remove. If the `childNode` is not the child node of the `parentNode`, the method throws an exception. -->

<!-- The `removeChild()` returns the removed child node from the DOM tree but keeps it in the memory, which can be used later. -->

<!-- ### Example
{: .no_toc }
<!-- parent - Parent node whose child is to be removed
child - Node which will be removed
{: .bg-grey-dk-250 .code-example .text-grey-dk-000} -->


### Example
The following example uses the cloneNode() method to copy the <ul> element and place it in the same document.


{: .no_toc }

<!-- Copy a <div> element, including all its attributes and child elements, and append it to the document:
{: .bg-grey-dk-250 .code-example .text-grey-dk-000} -->


```hbs
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <title>JavaScript cloneNode() Demo</title>
</head>
<body>
    <ul id="menu">
        <li>Home</li>
        <li>Services</li>
        <li>About</li>
        <li>Contact</li>
    </ul>
    <script> 
        let menu = document.querySelector('#menu');
        let clonedMenu = menu.cloneNode(true);
        clonedMenu.id = 'menu-mobile';
        document.body.appendChild(clonedMenu);
    </script>
</body>
</html>
```
<!-- 
#### How it works.

    1. First, select the `<ul>` with the id menu by using the `querySelector()` method.
    2. Second, create a deep clone of the `<ul>` element using the `cloneNode()` method.
    3. Third, change the id of the cloned element to avoid duplicate.
    4. Finally, append the cloned element to the child nodes of the document.body using the `appendChild()` method.
{: .fs-2 .fw-400 } -->

#### Example Breakdown

𝟭. Select the <ul> with the id menu by using the `querySelector()` method.
{: .bg-grey-dk-250 .code-example .text-grey-dk-000}
```jsx
let menu = document.querySelector('#menu');
```

𝟐. Create a deep clone of the <ul> element using the `cloneNode()` method.
{: .bg-grey-dk-250 .code-example .text-grey-dk-000}
```jsx
let clonedMenu = menu.cloneNode(true);
```

𝟯. Change the id of the cloned element to avoid duplicate.
{: .bg-grey-dk-250 .code-example .text-grey-dk-000}
```jsx
clonedMenu.id = 'menu-mobile';
```

𝟰. Append the cloned element to the child nodes of the document.body using the `appendChild()` method.
{: .bg-grey-dk-250 .code-example .text-grey-dk-000}
```jsx
document.body.appendChild(clonedMenu);
```

### More Examples
Copy a `<div>` element, including all its attributes and child elements, and append it to the document:

```js
    var elmnt = document.getElementsByTagName("DIV")[0];
    var cln = elmnt.cloneNode(true);
    document.body.appendChild(cln);
```
