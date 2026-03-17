---
theme: apple-basic
# background: https://cover.sli.dev

# force color schema for the slides, can be 'auto', 'light', or 'dark'
colorSchema: light

# favicon, can be a local file path or URL
favicon: "https://garthtuck.com/images/favicon.ico"

title: Using CodePen in Intro to JavaScript
class: text-center
layout: center

# author field for exported PDF or PPTX
author: Garth Tuck

# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left

download: true
exportFilename: CodePen-JS-Presentation
---

<style>
h1 {
  background-color: #492365;
  background-image: linear-gradient(45deg, #814d9d 10%, #a275b3 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

# Using CodePen.io to Introduce JavaScript

### Fast Feedback. Zero Setup. Maximum Engagement.

**Garth Tuck**  
Weber State University  

---

# The Problem

Intro students struggle with:

- Environment setup 😬  
- “Nothing works” frustration  
- Slow feedback loops  
- Fear of breaking things  

> Cognitive overload *before* JavaScript learning begins

---

# Why CodePen?

- ✅ No install
- ✅ Instant feedback
- ✅ Visual learning
- ✅ Console is exposed
- ✅ Share via URL

> Students focus on *learning*, not tooling

---

# Typical flow

- Open Playground Pen  
- Lecture with examples  
- Students follow along (in their own pen)  

> Students submit *thier* pen URL

---

# Let's see it in action

## https://codepen.io

---

# Activity 1 — Click to Change Color

### HTML
```html
<button>Click Me</button>
```

### JavaScript
```js
document.querySelector("button").onclick = function() {
  document.body.style.backgroundColor = "yellow";
};
```

---

# Activity 2 — Counter App

### HTML
```html
<button id="btn">Click</button>
<p id="count">0</p>
```

### JavaScript
```js
let count = 0;
document.getElementById("btn").onclick = () => {
  count++;
  document.getElementById("count").textContent = count;
};
```

---

# Activity 3 — Change Text

### HTML
```html
<h1 id="title">Hello</h1>
<button>Button</button>
```

### JavaScript
```js
document.querySelector("button").onclick = () => {
  document.getElementById("title").textContent = "Button was clicked!";
};
```

---

# Questions?
