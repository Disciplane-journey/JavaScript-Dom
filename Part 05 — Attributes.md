# Part 05 — Attributes

## getAttribute()

Read the value of any attribute.

```js
let link = document.getElementById("link")

link.getAttribute("href") // "https://google.com"
link.getAttribute("id")   // "link"
```

---

## setAttribute()

Set or change any attribute.

```js
link.setAttribute("href", "https://github.com")
// href updated ✅

let img = document.getElementById("img")
img.setAttribute("src", "dog.jpg")
// image changes instantly ✅
```

---

## removeAttribute()

Delete an attribute completely.

```js
link.removeAttribute("href")
// link no longer goes anywhere ✅
```

---

## hasAttribute()

Check if an attribute exists — returns true or false.

```js
link.hasAttribute("href")  // true
link.hasAttribute("class") // false
```

---

## Quick Reference

| Method | Job |
|--------|-----|
| getAttribute("x") | Read attribute value |
| setAttribute("x", "y") | Set or change attribute |
| removeAttribute("x") | Delete attribute |
| hasAttribute("x") | Check if exists |

>JavaScript DOM Series
