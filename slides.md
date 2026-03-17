---
theme: apple-basic
title: Using CodePen in Intro to JavaScript
author: Garth Tuck
transition: slide-left
download: true
exportFilename: CodePen-JS-Presentation
---

<style>
h1 {
  background: linear-gradient(45deg, #4f46e5, #9333ea);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
.qr {
  width: 180px;
}
</style>

# Using CodePen in Intro to JavaScript

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

> Cognitive overload happens *before* learning JavaScript

---

# Why CodePen?

- ✅ No install
- ✅ Instant feedback
- ✅ Visual learning
- ✅ Share via URL

> Students focus on *learning*, not tooling

---

# Teaching Philosophy

> Remove friction → Increase experimentation → Build confidence

- Start with **play**
- Encourage **trial & error**
- Show **immediate results**

---

# Demo (Pre-Built Pen)

```js
document.querySelector("button").addEventListener("click", () => {
  document.body.style.backgroundColor = "lightblue";
});
```

---

# Lesson Structure

**50-minute class:**

- 5 min → Show working example  
- 10 min → Explain concept  
- 20 min → Student modification  
- 10 min → Challenge  
- 5 min → Share  

---

# Classroom Workflow

1. Create starter Pen  
2. Share link  
3. Students fork  
4. Students experiment  

---

# Activity 1 — Click to Change Color

```html
<button>Click Me</button>
```

```js
document.querySelector("button").onclick = function() {
  document.body.style.backgroundColor = "yellow";
};
```

Scan: https://codepen.io/pen?template=dygNwQX

---

# Activity 2 — Counter App

```html
<button id="btn">Click</button>
<p id="count">0</p>
```

```js
let count = 0;
document.getElementById("btn").onclick = () => {
  count++;
  document.getElementById("count").textContent = count;
};
```

Scan: https://codepen.io/pen?template=abdygZX

---

# Activity 3 — Change Text

```html
<h1 id="title">Hello</h1>
<button>Change</button>
```

```js
document.querySelector("button").onclick = () => {
  document.getElementById("title").textContent = "You clicked!";
};
```

Scan: https://codepen.io/pen?template=GRyXbqV

---

# Final Thought

> “If students can see it change, they believe they can learn it.”

---

# Questions?
