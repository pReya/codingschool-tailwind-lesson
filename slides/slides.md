---
title: "Utility-first CSS frameworks"
---
# Utility-first CSS frameworks

Moritz Stückler<br/> 
<span style="font-size: 1.4rem;">[Twitter (@MoStueck)](https://twitter.com/MoStueck)<br/>
[Mastodon (@preya@mastodon.social)](https://mastodon.social/@preya)<br/>
[GitHub (pReya)](https://github.com/pReya)</span>

Note:


---
# HELLO 👋
### Who are you?

Note:
- Introductions (How much do you know about HTML/CSS/JS?)
- Repeat all names

---
<figure>
<img src="images/tailwind_girlfriend_meme.jpg" />
<figcaption>Source: <a href="https://twitter.com/vicvijayakumar/status/1204198443184463873">Twitter @vicvijayakumar</a></figcaption>
</figure>

Note:
- Goal is to understand this meme at the end of the lesson

---

## Why should we learn this?
<figure>
<img src="images/npm_trends_tailwind.png" />
<figcaption>Source: <a href="https://npmtrends.com/tailwindcss">npmtrends.com/tailwindcss</a></figcaption>
</figure>

but mostly: It makes our life <span style="text-decoration: underline">easier</span>!

Note:
- Why should we learn about this?
  - Very popular in the last years (see npmtrends) – could be part of your future job
  - Typically makes styling easier and faster (higher productivity)

---

### Outline
1. Concepts: "utility first" and "CSS framework"
2. Playing with TailwindCSS
3. Necessary evil: Build steps & Purging

Note:
- Understand this meme at the end of the lesson

---

### Exercise 1
*How can we improve/refactor `01/part-a.html`?*

Note:
1. Refactor `part-a` -> extract common CSS properties
2. What if we want to make buttons with different radiuses in `part-b`?
3. We've broken down the classes as much as we can -> these are now utility classes

---

### Definition: "Utility First CSS"

- Also called "Atomic CSS" ⚛
- A way to write and structure CSS classes
- Uses tiny atomic classes (classes that can't be broken down further)
- Composition happens in HTML, not in CSS

Note:

---
### Definition: CSS Framework

- Use somebody else's CSS
- Popular: Bootstrap, Foundation, Bulma (NOT Atomic/Utility based)
- Don't need to reinvent utility classes (they're always the same)
- How to:
```html
<head>
  <script src="https://cdn.tailwindcss.com" />
</head>
```

Note:
- We're not actually writing CSS, just HTML – might get by without a single line of CSS

---

### 👍🏻 Benefits

- More UI elements don't lead to more CSS
- Knowing how a component looks, just by looking at class names

```html
<img class="rounded-full border drop-shadow-md" />
```
vs.
```html
<img class="profile-pic" />
```
- Predictable (no "side effects" like nested selectors or element selectors)
- Consistent color palettes and scales
- No more naming fights


Note:


---


### Exercise 2
*Let's build a nav bar with TailwindCSS!<br/> (Try not to write any CSS)*


![](images/navbar.png)
Note:
- Give 10-15m for everyone to try build it
- Then build it together via live coding session
  - Structure first
  - Styling second

---

#### Which classes are available in TailwindCSS?

<figure>
<img src="images/rtfm.jpg" />
<figcaption>Source: <a href="https://devrant.com/rants/726139/while-most-people-want-the-force-to-get-stuff-like-a-tv-remote-i-want-to-use-it">devrant.com</a></figcaption>
</figure>


Note:


---