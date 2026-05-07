# Part 06 — Parent & Children

## children

Get all direct child elements.

```js
let parent = document.getElementById("parent")

parent.children          // HTMLCollection [h1, p, span]
parent.firstElementChild // <h1>Title</h1>
parent.lastElementChild  // <span>Span</span>
```

---

## parentElement

Go up to the parent of any element.

```js
let h1 = document.querySelector("h1")

h1.parentElement // <div id="parent"> ✅
```

---

## Siblings

Navigate to the element before or after.

```js
h1.nextElementSibling     // <p>Paragraph</p>
h1.previousElementSibling // null — nothing before h1
```

---

## Real World Example

```js
let parent = document.getElementById("parent")

for (let child of parent.children) {
  console.log(child) // h1, p, span
}
```

---

## Quick Reference

| Property | Returns |
|----------|---------|
| children | All child elements |
| firstElementChild | First child |
| lastElementChild | Last child |
| parentElement | Parent element |
| nextElementSibling | Next sibling |
| previousElementSibling | Previous sibling |

>JavaScript DOM Series
