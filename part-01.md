# Part 01 — What is the DOM?

## HTML is just text

```html
<body>
  <h1>Hello</h1>
  <p>World</p>
</body>
```

When you write HTML — you are writing a string. Nothing more.

---

## Browser converts it into a tree

```
document
└── body
    ├── h1 → "Hello"
    └── p  → "World"
```

This tree is called the **DOM — Document Object Model.**

Every HTML element becomes an object with properties that JavaScript can read and change.

---

## JavaScript works on the DOM

```js
document.body          // access the body
document.body.children // HTMLCollection [h1, p]
```

You are not editing the HTML file.

You are changing the DOM — and the browser instantly reflects those changes on screen.

---

## Why it matters

Every time a page updates without reloading — a modal opens, a button changes, a dropdown appears — that is JavaScript changing the DOM.

The DOM is the bridge between your HTML and your JavaScript.

> JavaScript DOM Series
