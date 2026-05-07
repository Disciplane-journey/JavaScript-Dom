# Part 02 — Selecting Elements

## getElementById()

```js
document.getElementById("title")
// <h1 id="title">Hello</h1>
```

Returns a single element. Id is unique — always one result.

---

## getElementsByClassName()

```js
document.getElementsByClassName("text")
// HTMLCollection [p, p]
```

Returns all elements with that class as an HTMLCollection.

---

## querySelector()

```js
document.querySelector("#title")  // by id
document.querySelector(".text")   // by class — first match only
```

Uses CSS selector syntax. Always returns first matching element only.

---

## querySelectorAll()

```js
document.querySelectorAll(".text")
// NodeList [p, p]
```

Returns all matching elements as a NodeList.

---

## Quick Reference

| Method | Returns | Selector |
|--------|---------|----------|
| getElementById() | Single element | id name |
| getElementsByClassName() | HTMLCollection | class name |
| querySelector() | First match | CSS selector |
| querySelectorAll() | NodeList | CSS selector |

---

## Which one to use?

`querySelector` and `querySelectorAll` — they use CSS selectors which you already know.

>
>  JavaScript DOM Series
