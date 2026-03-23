---
theme: apple-basic
# background: https://cover.sli.dev

# force color schema for the slides, can be 'auto', 'light', or 'dark'
colorSchema: light

# favicon, can be a local file path or URL
favicon: "https://garthtuck.com/images/favicon.ico"

title: Using CodePen in Intro to JavaScript
class: hero-slide text-center
layout: center

# author field for exported PDF or PPTX
author: Garth Tuck

# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left

download: true
exportFilename: CodePen-JS-Presentation
---

<style>
:root {
  --deck-accent: #6f3fa0;
  --deck-accent-soft: #f3edf8;
  --deck-border: #ddd0ea;
  --deck-text-soft: #5d4b73;
}

.slidev-layout {
  padding: 2.2rem 2.6rem;
}

.slidev-layout.two-cols-header {
  column-gap: 1.5rem;
}

.slidev-layout h1 {
  margin-bottom: 0.35rem;
  line-height: 1.05;
}

.slidev-layout h2,
.slidev-layout h3 {
  line-height: 1.15;
}

.slidev-layout ul,
.slidev-layout ol {
  margin-top: 0.85rem;
}

.slidev-layout li + li {
  margin-top: 0.45rem;
}

.slidev-layout blockquote {
  margin-top: 1rem;
  border-left: 4px solid var(--deck-accent);
  background: var(--deck-accent-soft);
  color: var(--deck-text-soft);
  border-radius: 0.9rem;
  padding: 0.75rem 1rem;
  font-style: normal;
}

.slidev-layout pre {
  font-size: 0.84rem;
  line-height: 1.35;
}

.hero-slide h1 {
  background-color: #492365;
  background-image: linear-gradient(45deg, #814d9d 10%, #a275b3 20%, #492365 90%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
  font-size: 2.65rem;
}

.kicker {
  margin-bottom: 0.75rem;
  color: var(--deck-accent);
  font-size: 0.78rem;
  font-weight: 700;
  letter-spacing: 0.18em;
  text-transform: uppercase;
}

.subtitle {
  margin-top: 0.85rem;
  font-size: 1.15rem;
  color: var(--deck-text-soft);
}

.presenter {
  margin-top: 1.5rem;
  font-size: 0.95rem;
  color: #3d3250;
  line-height: 1.6;
}

.section-slide h1 {
  margin-bottom: 0.75rem;
  font-size: 2.3rem;
}

.link-card {
  display: inline-block;
  margin-top: 1.5rem;
  padding: 0.9rem 1.35rem;
  border: 1px solid var(--deck-border);
  border-radius: 1rem;
  background: #faf7fc;
  box-shadow: 0 12px 30px rgba(73, 35, 101, 0.08);
  font-size: 1.2rem;
  font-weight: 600;
}

.link-card a {
  color: #492365;
  text-decoration: none;
}

.callout {
  margin-top: 1rem;
  padding: 1.1rem 1.15rem;
  border: 1px solid var(--deck-border);
  border-radius: 1rem;
  background: linear-gradient(180deg, #faf7fc 0%, #f3edf8 100%);
}

.callout h3 {
  margin-top: 0;
  margin-bottom: 0.45rem;
  color: #492365;
}

.callout p {
  margin: 0;
  color: #4d4060;
  line-height: 1.5;
}

.activity-slide h1 {
  margin-bottom: 0.25rem;
}

.activity-slide h2 {
  margin-top: 0;
  margin-bottom: 0.9rem;
  color: #5d4b73;
  font-size: 1.1rem;
  font-weight: 500;
}

.activity-slide h3 {
  margin-top: 0.2rem;
  margin-bottom: 0.4rem;
}
</style>

# Using CodePen.io to Introduce JavaScript

### Fast feedback. Zero setup. Maximum engagement.  

<p class="presenter">
  Garth Tuck<br>
  Weber State University
</p>

---

# The Problem

### Intro students often hit friction before they ever reach the JavaScript concept itself:

- **Environment setup** derails momentum
- **"Nothing works" frustration** appears early
- **Slow feedback loops** make experimentation feel risky
- **Fear of breaking things** discourages exploration

> Cognitive overload shows up before real JavaScript learning begins.

---
layout: two-cols-header
---
# Why CodePen?

### Remove setup friction and keep the focus on JavaScript.

::left::

- ✅ No install
- ✅ Instant feedback
- ✅ Visual learning
- ✅ The console is always visible
- ✅ Share work by URL

::right::

<div class="callout">
  <h3>Instructional payoff</h3>
  <p>Students spend class time learning JavaScript instead of troubleshooting local tooling.</p>
</div>

---

# The No-Fear Setup

### Tips for the non-CS teacher

- **No account needed:** Students can start coding immediately. They only need an account to save.
- **Show the Console button:** It becomes the hub for debugging conversations.
- **Lean into copy/paste:** Examples run without extra `<script>` ceremony.
- **Use collections:** Keep the semester organized in public folders.

---

# My Typical Flow

- Open my playground pen.
- Model the concept live during lecture.
- Students follow along in their own pen.
- Students submit their pen URL.

> The workflow stays lightweight for you and low-stakes for students.

---
layout: center
class: section-slide text-center
---
<div class="kicker">Live Demo</div>

# Let's See It in Action

<div class="link-card">
  <a href="https://codepen.io" target="_blank">https://codepen.io</a>
</div>

---
layout: two-cols-header
class: activity-slide
---
# Activity 1

### Click to Change Color

Use one button click to update the page background.

::left::

### HTML

```html
<button>Click Me</button>
```

::right::

### JavaScript

```js
document.querySelector("button").onclick = function () {
  document.body.style.backgroundColor = "yellow";
};
```

---
layout: two-cols-header
class: activity-slide
---
# Activity 2

### Counter App

Track a value in JavaScript and reflect it in the DOM.

::left::

### HTML

```html
<button id="btn">Click</button>
<p id="count">0</p>
```

::right::

### JavaScript

```js
let count = 0;

document.getElementById("btn").onclick = () => {
  count++;
  document.getElementById("count").textContent = count;
};
```

---
layout: two-cols-header
class: activity-slide
---
# Activity 3

### Change Text

Respond to a click by replacing page text.

::left::

### HTML

```html
<h1 id="title">Hello</h1>
<button>Button</button>
```

::right::

### JavaScript

```js
document.querySelector("button").onclick = () => {
  document.getElementById("title").textContent = "Button was clicked!";
};
```

---
layout: center
class: section-slide text-center
---
<div class="kicker">Discussion</div>

# Questions?

<p class="subtitle">CodePen makes it easier to teach JavaScript before setup becomes the lesson.</p>
