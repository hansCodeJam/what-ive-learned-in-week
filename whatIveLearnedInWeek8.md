# What I've Learend In Week 8

### Javascript Events

HTML events are **"things"** that happen to HTML elements.

When JavaScript is used in HTML pages, JavaScript can **"react"** on these events.

Example

```html
<!DOCTYPE html>
<html>
<body>

<button onclick="document.getElementById('demo').innerText=Date()">The time is?</button>

<p id="demo"></p>

</body>
</html>

<!-- Output on the dom:
Click demo button 
Output on dom: Sun Nov 03 2019 12:13:19 GMT-0500 (Eastern Standard Time) -->

```

Example from [domosour](https://github.com/hansCodeJam/domosaur) 

```Javascript
//querySelector
const feathered = document.querySelector('#feathers');

//AddEventListener
feathered.addEventListener('click', makeTransparent);

//Function
function makeTransparent(event) {
  event.target.style.opacity = 0.5;
}
```

Codewars

Don't Give me Five

```Javascript
function dontGiveMeFive(start, end) {
  let count = 0;
  for (let i = start; i <= end; i++) {
    if (i.toString().includes('5') !== true) {
      count++;
    }
  }
  return count;
}
```
