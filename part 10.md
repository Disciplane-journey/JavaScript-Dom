# Part 10 — Event Object

## What is the event object?

Every event automatically passes an object to your function.

```js
btn.addEventListener("click", function(e) {
  console.log(e)        // full event object
  console.log(e.target) // element that fired the event
  console.log(e.type)   // "click"
})
```

---

## e.preventDefault()

Stops the default behavior of an element.

```js
let link = document.querySelector("a")

link.addEventListener("click", function(e) {
  e.preventDefault()
  // page does NOT navigate ✅
})

let form = document.querySelector("form")

form.addEventListener("submit", function(e) {
  e.preventDefault()
  // page does NOT reload ✅
})
```

---

## e.stopPropagation()

Stops the event from bubbling up to parent elements.

```js
document.getElementById("btn").addEventListener("click", function(e) {
  e.stopPropagation()
  console.log("btn clicked") // only this runs ✅
})

document.getElementById("parent").addEventListener("click", function() {
  console.log("parent clicked") // never runs ✅
})
```

---

## Quick Reference

| Property / Method | Job |
|-------------------|-----|
| e.target | Element that fired the event |
| e.type | Type of event |
| e.preventDefault() | Stop default behavior |
| e.stopPropagation() | Stop event bubbling |

> JavaScript DOM Series
