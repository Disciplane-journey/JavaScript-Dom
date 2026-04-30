# Part 07 — Creating Elements

## createElement()

Creates a new element — not added to page yet.

```js
let newPara = document.createElement("p")
```

---

## Add content and attributes

```js
newPara.innerText = "I was created by JavaScript"
newPara.classList.add("highlight")
newPara.setAttribute("id", "new-para")
```

---

## appendChild() — add at the end

```js
let parent = document.getElementById("box")
parent.appendChild(newPara) // added at end ✅
```

---

## prepend() — add at the beginning

```js
parent.prepend(newPara) // added at beginning ✅
```

---

## insertBefore() — add at specific position

```js
let reference = document.querySelector("h1")
parent.insertBefore(newPara, reference)
// newPara placed right before h1 ✅
```

---

## Full Example

```js
let li = document.createElement("li")
li.innerText = "New Item"

let ul = document.getElementById("list")
ul.appendChild(li) // new item added to list ✅
```

---

## Quick Reference

| Method | Job |
|--------|-----|
| createElement("tag") | Create new element |
| appendChild(el) | Add at end of parent |
| prepend(el) | Add at beginning of parent |
| insertBefore(el, ref) | Add before a specific element |

>JavaScript DOM Series
