# Part 11 — Event Delegation

## The Problem

Adding a listener to every element is inefficient.

```js
let items = document.querySelectorAll("li")

items.forEach(item => {
  item.addEventListener("click", function() {
    console.log("clicked") // one listener per element ❌
  })
})
```

100 items = 100 listeners. And dynamically added items get no listener at all.

---

## The Solution — Event Delegation

Add one listener to the parent instead.

```js
let list = document.getElementById("list")

list.addEventListener("click", function(e) {
  if(e.target.tagName === "LI") {
    console.log(e.target.innerText) ✅
  }
})
```

Event bubbles up from li → ul — e.target tells you which li was clicked.

---

## Works on Dynamic Elements Too

```js
let newItem = document.createElement("li")
newItem.innerText = "Item 4"
list.appendChild(newItem)

// click works automatically ✅
// no new listener needed
```

---

## Quick Reference

| | Without Delegation | With Delegation |
|---|---|---|
| Listeners | One per element | Just one |
| Dynamic elements | ❌ | ✅ |
| Performance | ❌ Heavy | ✅ Light |
| Code | ❌ Repetitive | ✅ Clean |

> JavaScript DOM Series
