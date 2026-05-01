# Part 09 — Events

## addEventListener()

Listen for user actions and run code when they happen.

```js
let btn = document.getElementById("btn")

btn.addEventListener("click", function() {
  console.log("Button clicked!") ✅
})
```

addEventListener takes 2 things:
- Event name — "click"
- Function to run when it fires

---

## Mouse Events

```js
btn.addEventListener("click",     function() { console.log("clicked") })
btn.addEventListener("mouseover", function() { console.log("hovered") })
btn.addEventListener("mouseout",  function() { console.log("left") })
btn.addEventListener("dblclick",  function() { console.log("double clicked") })
```

---

## Keyboard Events

```js
document.addEventListener("keydown",  function() { console.log("key pressed") })
document.addEventListener("keypress", function() { console.log("key held") })
```

---

## Input Events

```js
let input = document.getElementById("inp")

input.addEventListener("input",  function() { console.log("user is typing") })
input.addEventListener("change", function() { console.log("value changed") })
```

---

## Quick Reference

| Event | When it fires |
|-------|--------------|
| click | Mouse click |
| dblclick | Double click |
| mouseover | Mouse enters element |
| mouseout | Mouse leaves element |
| keydown | Key is pressed |
| keypress | Key is held down |
| input | User is typing |
| change | Input value changed |

> JavaScript DOM Series
