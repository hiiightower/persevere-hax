---
layout: default
title: Get and set the HTML content of an element
parent: 3. Manipulating Elements
---


## Get and set the HTML content of an element
You can also get or set the contents of the HTML elements easily with the innerHTML property. This property sets or gets the HTML markup contained within the element i.e. content between its opening and closing tags. 


---


### Definition and Usage
{: .no_toc }
The element property innerHTML is used for getting and setting the HTML content of en element in vanilla JavaScript.


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
const content = element.innerHTML;
element.innerHTML = htmlString;
```


### Example

{: .no_toc }



```hbs
<div id="main">
    <h1 id="title">Hello World!</h1>
    <p id="hint">This is a simple paragraph.</p>
</div>
 
<script>
    // Getting inner HTML conents
    var contents = document.getElementById("main").innerHTML;
    alert(contents); // Outputs inner html contents
    
    // Setting inner HTML contents
    var mainDiv = document.getElementById("main");
    mainDiv.innerHTML = "<p>This is <em>newly inserted</em> paragraph.</p>";
</script>
```
As you can see how easily you can insert new elements into DOM using the innerHTML property, but there is one problem, the innerHTML property replaces all existing content of an element. So if you want to insert the HTML into the document without replacing the existing contents of an element, you can use the insertAdjacentHTML() method.


### Extended Usage

Reading the HTML contents of an element
{: .bg-grey-dk-250 .code-example .text-grey-dk-000}
```js
let contents = myElement.innerHTML;
// HTMLElementObject.innerHTML;
```
Replacing the contents of an element
{: .bg-grey-dk-250 .code-example .text-grey-dk-000}
```js
document.body.innerHTML = "";
// HTMLElementObject.innerHTML = text;
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

