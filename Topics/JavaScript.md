# JavaScript Basics

[Lecture slides](/_assets/JavaScript-Basics.pdf)

### Location and Data types

1: Script tags in the HTML document, insert either inside `<head></head>`, or after `</body>` tag.
```
<script></script>
<script src="/assets/app.js"></script>
 ```
 
2: [Variables](https://www.w3schools.com/js/js_variables.asp) and common data types (read more on the [MDN page](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures))

```
const, let, var (used when to support older browsers);

numbers, strings, booleans, arrays, objects
```


3: Browser Console:
 Browser > Developer Tools > Console
```
console.log()
```
### Accessing Data
```
const fruits = ["banana", "orange", "grape"]
```
`console.log(fruits[0])` prints "banana"


```
const fruits = [
    {
        "name": "banana",
        "number": 2
    },
    {
        "name": "orange",
        "number": 3
    },
    {
        "name": "grape",
        "number": 18
    }
]
```
`console.log(fruits[0].name)` prints "banana"


### JavaScript Selectors


Select single HTML element: 

- `querySelector()` selects the first element in the HTML document that matches its calling.

```
document.querySelector("p")
document.querySelector(".myclass")
document.querySelector("#myID")
```
- `getElementById`, no "#" before the name.

```
document.getElementById("channelTitle")
```

Select multiple HTML elements and obtain as a [NodeList](https://developer.mozilla.org/en-US/docs/Web/API/NodeList):
- `querySelectorAll()` selects all elements in the HTML document that matches its calling.

```
const pTags = document.querySelectorAll("p")
```
- `getElementsByClassName()` selects all elements under the class name, no "." before the name.

```
document.getElementsByClassName("red test");
```

### Event Listeners


Common JavaScript events: 
```
"click", "dblclick", 
"mouseover", "mouseout", 
"keyup", "keydown", 
"scroll", "resize", 
"play", "pause",
"transitionend", "submit"
```


Attach the listener to the interactive elements or window:
```
window.addEventListener("resize", function (){
    // do something here when the window is getting resized
})
```
```
pTag.addEventListener("click", function(){
    pTag.innerHTML = "the text changed after the click!"
})
```
