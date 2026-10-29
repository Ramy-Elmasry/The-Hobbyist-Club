# CSC 111 Web Development - Oral Defense & Study Cheatsheet

This cheatsheet covers **every single HTML tag, CSS property, selector, and relative path** used in **The Hobbyist Club** project. 

Use this to study for your oral discussion with the instructor and TAs. Keep answers simple, direct, and confident.

---

## Part 1: HTML Tags (What They Do & Why We Used Them)

### 1. Document Setup & Meta Tags
* **`<!DOCTYPE html>`**
  * **What it does:** Tells the web browser that this document is written in modern **HTML5**. It must be the very first line of every HTML file.
* **`<html>`**
  * **What it does:** The root element that wraps all content on the webpage.
  * **Attribute `lang="en"`:** Specifies the primary language of the page (English) for search engines and accessibility screen readers.
* **`<head>`**
  * **What it does:** Contains invisible "metadata" about the webpage (page title, character encoding, external stylesheets, viewport settings). Nothing inside `<head>` appears directly on the page body.
* **`<meta charset="UTF-8">`**
  * **What it does:** Sets character encoding to UTF-8, which supports all standard characters, symbols, and languages without broken text symbols.
* **`<meta name="viewport" content="width=device-width, initial-scale=1">`**
  * **What it does:** Makes the webpage mobile-friendly by matching the screen's width and setting the default zoom level to 100%.
* **`<title>`**
  * **What it does:** Sets the text shown on the browser's tab and in bookmark menus (e.g., `<title>The Hobbyist Club</title>`).
* **`<link>`**
  * **What it does:** Connects an external resource to the HTML document.
  * **Our use:** `<link rel="stylesheet" href="style.css"/>` links our external CSS stylesheet to style the HTML.
* **`<style>`**
  * **What it does:** An internal container inside `<head>` where CSS code is written directly into that specific HTML file.

---

### 2. Page Structure & Semantic Elements
> **Oral Exam Tip:** If asked *"What are semantic tags?"*, answer: *"They are tags whose names clearly describe their purpose to both the browser and the developer, rather than using generic `<div>` tags everywhere."*

* **`<body>`**
  * **What it does:** Contains all the visible content of the webpage (text, images, links, cards, tables).
* **`<header>`**
  * **What it does:** Semantic container for introductory content at the top of a page, such as the main title and navigation.
* **`<nav>`**
  * **What it does:** Semantic container dedicated exclusively to navigation menus and hyperlinks connecting site pages.
* **`<main>`**
  * **What it does:** Identifies the central, unique content of the page (excluding repeating headers and footers).
* **`<section>`**
  * **What it does:** Groups related content into thematic sections (e.g., Hero Section, Featured Hobbies Section, Team Section).
* **`<div>`**
  * **What it does:** A generic block-level container used to group elements for CSS styling and layout (e.g., `<div class="container">`, `<div class="card">`).
* **`<footer>`**
  * **What it does:** Semantic container placed at the bottom of the webpage for copyright notices and project metadata.

---

### 3. Headings, Text & Inline Formatting
* **`<h1>`, `<h2>`, `<h3>`**
  * **What they do:** Section headings ranked by importance. `<h1>` is the primary title of the page, `<h2>` is for major sections, and `<h3>` is for sub-sections/card titles.
* **`<p>`**
  * **What it does:** Defines a paragraph of text. Browsers automatically add vertical spacing before and after it.
* **`<a>`**
  * **What it does:** Anchor tag used to create hyperlinks.
  * **Attribute `href`:** Holds the target destination path (e.g., `<a href="../index.html">Main Home</a>`).
* **`<strong>`**
  * **What it does:** Marks text with strong importance (renders bold visually and emphasizes speech in screen readers).
* **`<b>`**
  * **What it does:** Stylistic bolding without inherent semantic importance.
* **`<br>`**
  * **What it does:** Creates a single line break without starting a new paragraph. It is a self-closing / void tag.
* **`<hr>`**
  * **What it does:** Inserts a horizontal thematic dividing line between sections.

---

### 4. Lists
* **`<ul>`**
  * **What it does:** Defines an **unordered list** (bulleted list).
* **`<ol>`**
  * **What it does:** Defines an **ordered list** (numbered list, used for step-by-step sequences).
* **`<li>`**
  * **What it does:** Defines an individual **list item** inside either `<ul>` or `<ol>`.

---

### 5. Media & Tables
* **`<img>`**
  * **What it does:** Embeds an image on the webpage.
  * **Attribute `src`:** The file path or filename of the image (e.g., `volleyball.jpg`).
  * **Attribute `alt`:** Alternative text displayed if the image fails to load, and read aloud by screen readers for accessibility.
* **`<table>`**
  * **What it does:** Container used to display structured, tabular data in rows and columns.
* **`<tr>`**
  * **What it does:** Table Row — represents a horizontal row inside the table.
* **`<th>`**
  * **What it does:** Table Header cell — labels a column; text is bold and centered by default.
* **`<td>`**
  * **What it does:** Table Data cell — contains the standard information in a column row.

---

## Part 2: CSS Properties (What They Do & Why We Used Them)

### 1. The CSS Box Model & Sizing
> **Oral Exam Tip:** The Box Model consists of: **Content &rarr; Padding &rarr; Border &rarr; Margin**.

* **`box-sizing: border-box;`**
  * **What it does:** Forces the element's defined `width` and `height` to include its padding and borders. This prevents layout breakage when adding padding.
* **`margin`**
  * **What it does:** Clears space **outside** the border of an element, pushing adjacent elements away.
  * `margin: 0 auto;` &rarr; Horizontally centers a block element with a fixed `max-width`.
  * `margin: 20px auto;` &rarr; 20px space on top and bottom, centered horizontally.
  * `margin-bottom: 15px;` &rarr; Adds space only beneath an element.
* **`padding`**
  * **What it does:** Clears space **inside** the border, creating breathing room between the element's border and its inner text/content.
* **`border`**
  * **What it does:** Draws an outline directly around an element's padding (e.g., `border: 1px solid #ddd;`).
* **`border-radius`**
  * **What it does:** Rounds the corners of an element's outer border box (e.g., `border-radius: 8px;`).
* **`max-width`**
  * **What it does:** Caps how wide an element can expand on large desktop screens, while allowing it to shrink naturally on smaller screens (e.g., `max-width: 900px;`).
* **`width`**
  * **What it does:** Sets an explicit width on an element (e.g., `width: 100%;` for tables, `width: 350px;` for images).

---

### 2. Colors & Backgrounds
* **`color`**
  * **What it does:** Sets the color of the **text** (e.g., `color: #fff;` for white, `color: #333;` for dark gray).
* **`background` / `background-color`**
  * **What it does:** Sets the background fill color of an element (e.g., `background-color: #2e7d32;` for green header).
* **Hex Color Codes vs Named Colors:**
  * `#222` / `#333` = Dark grays/blacks.
  * `#fff` = Pure white.
  * `#f4f7f6` = Soft off-white / light gray background.
  * `#2e7d32` = Forest green.
  * `#880e4f` = Deep maroon/magenta.
* **`rgba(0, 0, 0, 0.1)`**
  * **What it does:** Red, Green, Blue, plus **Alpha (transparency)**. `0.1` means 10% opacity, perfect for subtle drop shadows.

---

### 3. Typography & Text Formatting
* **`font-family`**
  * **What it does:** Sets the font typeface (e.g., `Arial, sans-serif`). If Arial is unavailable on the user's computer, it falls back to the system's default sans-serif font.
* **`font-size`**
  * **What it does:** Controls the size of the text (e.g., `font-size: 16px;`).
* **`font-weight`**
  * **What it does:** Controls text thickness (`font-weight: bold;` or `font-weight: normal;`).
* **`line-height`**
  * **What it does:** Controls vertical spacing between lines of text inside a paragraph (e.g., `line-height: 1.6;` makes text much easier to read).
* **`text-align`**
  * **What it does:** Controls the horizontal alignment of text (`text-align: center;` or `text-align: left;`).
* **`text-decoration`**
  * **What it does:** Controls decorative text lines. `text-decoration: none;` removes the default blue underline from hyperlinks; `text-decoration: underline;` adds it back.

---

### 4. Layout, Effects & Tables
* **`display: inline-block;`**
  * **What it does:** Allows an inline element (like an `<a>` link) to accept width, height, padding, and margins so it behaves like a styled button.
* **`box-shadow`**
  * **What it does:** Adds a subtle 3D drop shadow around card boxes (e.g., `box-shadow: 0 4px 8px rgba(0,0,0,0.1);`).
* **`border-collapse: collapse;`**
  * **What it does:** Collapses adjacent table cell borders into a single border line instead of showing double borders.

---

### 5. CSS Selectors Used in the Project
* **Universal Selector (`*`)**
  * Matches every single element on the page (used for `* { box-sizing: border-box; }`).
* **Element Selectors (`header`, `p`, `a`, `table`)**
  * Targets all HTML elements of that tag type across the page.
* **Class Selectors (`.container`, `.card`, `.reason-box`)**
  * Targets any element marked with that class name in HTML (e.g., `<div class="card">`). Classes can be reused on multiple elements.
* **Descendant Selectors (`nav a`)**
  * Targets any `<a>` element that lives **inside** a `<nav>` container.
* **Pseudo-Class (`:hover`)**
  * Applies styles only when the user hovers their mouse cursor over the element (e.g., `nav a:hover { text-decoration: underline; }`).

---

## Part 3: Relative Paths & File Navigation (Crucial!)

### How Paths Work in Our Project Structure

```text
The-Hobbyist-Club/
├── index.html        (Project Root Home)
├── about.html        (Team & Project Details)
├── style.css         (Global Shared Stylesheet)
├── cheatsheet.md     (This study guide)
├── Jerome G/
│   ├── index.html
│   └── weekend.html
├── Omar A/
│   ├── index.html
│   └── page2.html
├── Omar N/
│   ├── index.html
│   └── page2.html
├── Marogina A/
│   ├── basics.html
│   ├── types.html
│   └── *.jpg
└── Ramy A/
    ├── index.html
    └── page2.html
```

### Path Rules to Explain:
1. **Sibling in same folder:** Just the filename:
   * From `Omar A/index.html` &rarr; `href="page2.html"`
2. **From root down into a folder:** Folder name + filename:
   * From `index.html` &rarr; `href="Omar A/index.html"`
3. **From inside a folder up to root:** Use `../`:
   * From `Omar A/index.html` &rarr; `href="../index.html"`
   * The `../` tells the browser to **exit the current directory and step up into the parent folder**.

---

## Part 4: Top 5 Oral Defense Questions & Answers

### Q1: "What is the difference between an external CSS file and internal `<style>`?"
* **Answer:** *"External CSS (`<link rel="stylesheet" href="style.css">`) is written in a separate file and shared across multiple pages, ensuring consistent site-wide design with zero repeated code. Internal CSS (`<style>` in `<head>`) is written directly in one HTML document to style rules unique to that specific page."*

### Q2: "What is the CSS Box Model?"
* **Answer:** *"The Box Model represents every element on a page as a rectangular box made of four layers from inside out: **Content** (text/images), **Padding** (inner space around content), **Border** (the visible line around padding), and **Margin** (outer space pushing other elements away)."*

### Q3: "Why did you use `box-sizing: border-box`?"
* **Answer:** *"By default (`content-box`), adding padding or borders increases an element's total width and can break layouts. `border-box` forces the element's width to include both padding and border, keeping layout sizes predictable."*

### Q4: "Why use semantic tags like `<header>`, `<nav>`, `<section>`, and `<footer>` instead of just `<div>`?"
* **Answer:** *"Semantic tags provide clear meaning to search engines, screen readers for accessibility, and other developers. A `<div>` has no semantic meaning, whereas `<nav>` explicitly indicates website navigation links."*

### Q5: "How does your site ensure navigation works when unzipped locally without a web server?"
* **Answer:** *"All navigation links use strict relative paths (`../index.html` to return to root, and `<folder>/<page>.html` to enter subpages). Because no absolute paths or server-dependent URLs are used, the entire site functions completely offline directly from the file system (`file://`)."*
