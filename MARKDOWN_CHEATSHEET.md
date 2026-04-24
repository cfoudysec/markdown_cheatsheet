<!--
╔══════════════════════════════════════════════════════════════════╗
║  MARKDOWN CHEATSHEET  ::  the basics, and only the basics        ║
║  works everywhere: GitHub, Reddit, Obsidian, Notion, Discord...  ║
╚══════════════════════════════════════════════════════════════════╝
-->

<p align="center">
  <img src="kryptokat.png" alt="neon cat on the grid" width="320">
</p>

<h1 align="center">📓 Markdown Cheatsheet</h1>

<p align="center">
  <em>The ten things you actually need to know.</em><br>
  <sub>Works everywhere markdown works.</sub>
</p>

---

## 🗺️ Contents

1. [Headers](#1-headers)
2. [Bold & Italic](#2-bold--italic)
3. [Unordered Lists](#3-unordered-lists)
4. [Ordered Lists](#4-ordered-lists)
5. [Nested Lists](#5-nested-lists)
6. [Links](#6-links)
7. [Images](#7-images)
8. [Inline Code](#8-inline-code)
9. [Code Blocks](#9-code-blocks)
10. [Blockquotes](#10-blockquotes)
11. [Horizontal Rules](#11-horizontal-rules)
12. [Paragraphs & Line Breaks](#12-paragraphs--line-breaks)

---

## 1. Headers

Pound signs at the start of a line. More pounds means smaller header.

```markdown
# Biggest header
## Big header
### Medium header
#### Small header
##### Smaller header
###### Smallest header
```

**Rule of thumb:** only one `#` (H1) per document. Use it for the title.

---

## 2. Bold & Italic

Wrap text in asterisks.

```markdown
*italic text*
**bold text**
***bold and italic***
```

You can use underscores instead (`_italic_`, `__bold__`) but asterisks are the standard. Pick one and stay consistent.

---

## 3. Unordered Lists

Dash at the start of each line.

```markdown
- milk
- eggs
- bread
```

You can also use `*` or `+` but `-` is the most common.

---

## 4. Ordered Lists

Number followed by a period.

```markdown
1. first thing
2. second thing
3. third thing
```

**Useful trick:** the numbers don't actually matter. This renders the same way:

```markdown
1. first thing
1. second thing
1. third thing
```

Handy when you're inserting items in the middle of a long list and don't want to renumber everything.

---

## 5. Nested Lists

Indent two spaces for each level of nesting.

```markdown
- main item
  - sub-item
  - another sub-item
    - deeper sub-item
- next main item
```

This works with ordered lists too, and you can mix ordered and unordered:

```markdown
1. Boot the lab
   - spin up the VM
   - check network
2. Run the test
3. Write it up
```

---

## 6. Links

Square brackets around the visible text, parentheses around the URL.

```markdown
[click here](https://example.com)
```

Renders as: [click here](https://example.com)

To link to another file in the same folder:

```markdown
[see the notes](./notes.md)
```

---

## 7. Images

Same as links, but with an exclamation mark in front.

```markdown
![description of the image](path-to-image.png)
```

The description (called "alt text") shows up if the image fails to load, and is read by screen readers.

**To center an image on GitHub**, you need a little HTML trick because plain markdown can't do it:

```html
<p align="center">
  <img src="kryptokat.png" alt="a cat" width="300">
</p>
```

---

## 8. Inline Code

Single backticks around a word or phrase.

```markdown
Run `npm install` before starting.
```

Renders as: Run `npm install` before starting.

Great for file names, command names, function names, any bit of code embedded in a sentence.

---

## 9. Code Blocks

Three backticks on their own line, your code, then three more backticks on their own line.

````markdown
```
def hello():
    print("hi")
```
````

For syntax highlighting, add the language name right after the opening backticks:

````markdown
```python
def hello():
    print("hi")
```
````

Common language tags: `python`, `javascript`, `bash`, `html`, `css`, `json`, `yaml`, `sql`, `markdown`.

---

## 10. Blockquotes

Greater-than sign at the start of a line.

```markdown
> Something someone important said once.
```

Renders as:

> Something someone important said once.

For multi-line quotes, put `>` at the start of every line:

```markdown
> Line one of the quote.
> Line two of the quote.
> Line three.
```

---

## 11. Horizontal Rules

Three dashes on their own line. Useful for separating sections.

```markdown
---
```

You can also use `***` or `___` but `---` is the standard.

---

## 12. Paragraphs & Line Breaks

This one trips everyone up at first.

**Paragraphs** need a completely blank line between them:

```markdown
This is paragraph one.

This is paragraph two.
```

If you just hit enter once without a blank line, most markdown renderers will smush the lines together into one paragraph:

```markdown
This line
and this line
become one paragraph.
```

**To force a line break** without starting a new paragraph, end the line with two spaces, or just use `<br>`:

```markdown
Line one<br>
Line two
```

---

## 🎓 That's Everything

You now know every piece of core markdown syntax. Everything else you'll encounter (tables, task lists, strikethrough, alerts, diagrams, math equations) is an extension that specific platforms add on top. Those are nice when you need them, but the twelve things above will get you 95% of the way through any markdown file you'll ever write.

<p align="center">
  <sub>🐈‍⬛ keep it simple. ship the words. 🐈‍⬛</sub>
</p>
