# Part 04 — Changing Styles

## style.property

Directly change one CSS property at a time.

```js
let el = document.getElementById("box")

el.style.color = "red"
el.style.fontSize = "24px"
el.style.backgroundColor = "yellow"
```

CSS uses `font-size` — JavaScript uses `fontSize`. Hyphen becomes camelCase.

---

## classList

Add, remove, or toggle CSS classes.

```js
el.classList.add("active")     // add class
el.classList.remove("active")  // remove class
el.classList.toggle("active")  // add if not there, remove if there
el.classList.contains("active") // true or false
```

---

## Real World Example

```css
.active {
  color: red;
  font-size: 24px;
  background-color: yellow;
}
```

```js
el.classList.toggle("active")
```

Styles stay in CSS — JavaScript just switches the class.

---

## Quick Reference

| | style.property | classList |
|---|---|---|
| Where styles live | JavaScript | CSS |
| Clean code | ❌ | ✅ |
| Reusable | ❌ | ✅ |
| Best for | Quick one-off | Everything else |

---

## Rule

Always prefer classList — styles belong in CSS, not JavaScript.

> JavaScript DOM Series
