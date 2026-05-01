# Part 08 — Removing Elements

## remove()

Element removes itself directly.

```js
let para = document.getElementById("para")

para.remove() // gone ✅
```

---

## removeChild()

Parent removes a child element.

```js
let parent = document.getElementById("parent")
let title  = document.getElementById("title")

parent.removeChild(title) // gone ✅
```

---

## Real World Example

```js
btn.addEventListener("click", function() {
  let item = document.getElementById("todo-1")
  item.remove() // removed on click ✅
})
```

---

## Which one to use?

```js
el.remove()           // modern — recommended ✅
parent.removeChild(el) // older — still works
```

---

## Quick Reference

| Method | Who removes | Code needed |
|--------|-------------|-------------|
| remove() | Element itself | Just the element |
| removeChild() | Parent | Parent + child both |

>  JavaScript DOM Series
