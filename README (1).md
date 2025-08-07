# HTML Basics – Day 1 Practice

## 📌 What is HTML?

**HTML (HyperText Markup Language)** is the standard language used to create and structure content on the web. It defines the structure of web pages using a system of elements represented by tags.

HTML is not a programming language – it’s a *markup language* used to annotate content so that browsers know how to display it.

---

## 📘 What are HTML Elements?

An **HTML element** consists of a *start tag*, *content*, and an *end tag*. For example:

```html
<p>This is a paragraph.</p>
```

In this example:
- `<p>` is the **start tag**
- `This is a paragraph.` is the **content**
- `</p>` is the **end tag**

HTML elements can also include attributes to provide additional information (like `href`, `src`, `alt`, `title`, etc.).

---

## 🔍 Code Overview

This code demonstrates the most basic and essential HTML elements.

### 1. **Headings**
```html
<h1> to <h6>
```
Displays text in various sizes. `<h1>` is the largest heading; `<h6>` is the smallest.

---

### 2. **Formatting Elements**
These elements add semantic meaning and styling to text:

| Element | Purpose                       |
|---------|-------------------------------|
| `<b>`   | Bold (no semantic meaning)    |
| `<strong>` | Strong importance (bold + semantic) |
| `<i>`   | Italic (no semantic meaning)  |
| `<em>`  | Emphasized (italic + semantic)|
| `<mark>`| Highlighted text              |
| `<small>`| Smaller text                 |
| `<del>` | Deleted (strikethrough) text  |
| `<ins>` | Inserted (underlined) text    |
| `<sub>` | Subscript (e.g., H₂O)         |
| `<sup>` | Superscript (e.g., x²)        |

---

### 3. **Quotation and Citation Elements**

| Element    | Use Case                                      |
|------------|-----------------------------------------------|
| `<blockquote>` | For long block quotations                |
| `<q>`          | For short inline quotations              |
| `<cite>`       | Citing the title of a work (e.g., book)  |
| `<dfn>`        | Definition term                          |
| `<abbr>`       | Abbreviation with tooltip (`title` attr) |
| `<var>`        | Variable name                            |
| `<code>`       | Code snippet                             |
| `<samp>`       | Sample output from a program             |
| `<kbd>`        | Keyboard input (e.g., Ctrl + C)          |

---

### 4. **Links (Anchor Tags)**

| Attribute | Description                                     |
|-----------|-------------------------------------------------|
| `href`    | URL to open                                     |
| `target="_blank"` | Opens link in a new tab                |
| `target="_self"`  | Opens link in the same tab             |
| `target="_parent"` | Opens in parent frame                 |
| `target="_top"`   | Opens in full window                   |
| `rel="noopener noreferrer"` | Improves security            |
| `title`   | Tooltip shown when hovering over the link       |
| `download` | Triggers file download                         |

Example:
```html
<a href="bgimg.jpg" download="bgimage.jpg">Download Background Image</a>
```

---

## 🧠 Summary

This HTML file is a **Day 1 practice** to understand basic structure and elements of HTML including:
- Headings
- Paragraphs
- Formatting tags
- Quotations
- Links and anchor attributes

These are the building blocks of any web page and essential for learning how the web works.

---

## 📂 File Info

- **Filename:** `day1.html`
- **Topics Covered:** HTML Elements, Formatting, Quotation, Links