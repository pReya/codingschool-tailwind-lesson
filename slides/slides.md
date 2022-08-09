---
title: "Utility-first CSS frameworks"
---
# Utility-first CSS frameworks

<br/>

Moritz Stückler<br/> 
<span style="font-size: 1.4rem;">[Twitter (@MoStueck)](https://twitter.com/MoStueck)<br/>
[Mastodon (@preya@mastodon.social)](https://mastodon.social/@preya)<br/>
[GitHub (pReya)](https://github.com/pReya)</span>

Note:


---
# HELLO 👋
### Who are you?

Note:
- Introductions
  - Moritz Stückler, 32, Freelance Software Developer, Technische Informatik
  - Names, background and skillset (how much do you know about HTML/CSS/JS?) of all participants
- Repeat all names to remember

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
- Important question: Why should we learn about this?
  - Very popular in the last years (see npmtrends) – could be part of your future job
  - Typically makes styling easier and faster (higher productivity)
  - Don't NEED to know/do this

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
- Most popular candidate: TailwindCSS

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
- Predictable (less "side effects" aka "Why/where does this happen?")
- Consistent color palettes and scales
  - Typically don't need millions of colors or pixel-sized scaling
- No more naming fights (typical for semantic CSS)


Note:


---


### Exercise 2
*Let's build a navbar with TailwindCSS!<br/> (Try not to write any CSS)*


![](images/navbar.png)
Note:
- Give 15m for everyone to try building it
- Then build it together via live coding session
  - Structure first
  - Styling second
- Show how to add media queries
- Optional: make a burger menu icon appear/disappear on mobile
---

#### ...But how?

<figure>
<img src="images/rtfm.jpg" />
<figcaption>Source: <a href="https://devrant.com/rants/726139/while-most-people-want-the-force-to-get-stuff-like-a-tv-remote-i-want-to-use-it">devrant.com</a></figcaption>
</figure>


Note:
- Let's look at some class names together:
  - Padding, Margin, Height, Flex
- Show Tailwind Documentation Search

---

### Necessary evil: Build steps & Purging

- Instead of a single HUGE CSS file, Tailwind is being built to our needs
- All source files are scanned for Tailwind class names
- Unused classes are "purged" 🗑 -> small output file
- Need to run a "build step" on every change or deployment

Note:

---

### Even lazier: Tailwind UI

- If "utility first" CSS is still too fine/low level -> Tailwind UI
- Complete pages and components to be reused

Note:
- Show Tailwind UI components