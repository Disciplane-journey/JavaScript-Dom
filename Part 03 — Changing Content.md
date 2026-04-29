# Part 03 — Changing Content

## innerHTML

Reads and writes HTML including tags.

```js
let el = document.getElementById("box")

el.innerHTML // "Hello <b>World</b>"

el.innerHTML = "<b>New Text</b>"
// renders as bold text ✅
```

---

## innerText

Reads only visible text — ignores HTML tags.

```js
el.innerText // "Hello World"

el.innerText = "<b>New Text</b>"
// shows <b>New Text</b> as plain text ❌
```

---

## textContent

Reads all text — including hidden elements.

```js
el.textContent // "Hello World"
```

```html
<p id="box">Hello <span style="display:none">hidden</span></p>

el.innerText   // "Hello" — ignores hidden
el.textContent // "Hello hidden" — reads everything ✅
```

---

## Quick Reference

| | innerHTML | innerText | textContent |
|---|---|---|---|
| Reads HTML tags | ✅ | ❌ | ❌ |
| Reads hidden text | ✅ | ❌ | ✅ |
| Renders HTML | ✅ | ❌ | ❌ |

---

## Rule

- Need to add HTML? → innerHTML
- Need only visible text? → innerText
- Need all text including hidden? → textContent

> JavaScript DOM Series
