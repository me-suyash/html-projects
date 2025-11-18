# HTML Tags Reference Guide

Quick reference for all HTML tags used in Projects 1 & 2.

---

## 📸 Project Screenshots

### Project 1: Personal Portfolio
![Personal Portfolio Screenshot](./img/project-1.png)
*A simple portfolio page with navigation, skills, projects, and contact form.*

### Project 2: Travel Blog
![Travel Blog Screenshot](./img/project-2.png)
*A travel blog showcasing destinations with images and contact form.*

---

## Document Structure

**`<!DOCTYPE html>`** - Declares HTML5 document type

**`<html lang="en">`** - Root element with language attribute

**`<head>`** - Contains metadata (title, charset, viewport)

**`<body>`** - Contains all visible page content

---

## Metadata Tags

**`<meta charset="UTF-8">`** - Character encoding

**`<meta name="viewport">`** - Responsive design settings

**`<title>`** - Browser tab title

---

## Page Structure

**`<header>`** - Top section with site title and tagline

**`<nav>`** - Navigation menu with links

**`<main>`** - Main content area of the page

**`<section>`** - Thematic content group with `id` for navigation

**`<article>`** - Self-contained content (project cards, blog posts)

**`<footer>`** - Bottom section with copyright info

---

## Headings

**`<h1>`** - Main page title (use once per page)

**`<h2>`** - Section headings

**`<h3>`** - Sub-section headings

---

## Text Content

**`<p>`** - Paragraph text

**`<strong>`** - Important/bold text

**`<u>`** - Underlined text

**`<span>`** - Inline text container

**`<br />`** - Line break

---

## Lists

**`<ul>`** - Unordered (bulleted) list

**`<li>`** - List item

**`<dl>`** - Description list

**`<dt>`** - Description term (title)

**`<dd>`** - Description definition (details)

---

## Links & Navigation

**`<a href="#">`** - Hyperlink
- `href="#id"` - Link to section on same page
- `href="mailto:email"` - Email link
- `href="tel:phone"` - Phone link

---

## Images

**`<img>`** - Embed images
```html
<img src="url" alt="description" width="300" height="200" />
```
- `src` - Image URL
- `alt` - Alternative text (required for accessibility)
- `width`, `height` - Dimensions

---

## Forms

**`<form>`** - Form container
```html
<form action="#" method="post">
```

**`<label for="id">`** - Input label (connects to input)

**`<input>`** - Input field
- `type="text"` - Text input
- `type="email"` - Email input
- `type="submit"` - Submit button
- `placeholder` - Hint text
- `required` - Makes field mandatory

**`<textarea>`** - Multi-line text input
- `rows="5"` - Number of visible lines

---

## Special Characters

Use HTML entities for special characters:
- `&amp;` - & (ampersand)
- `&lt;` - < (less than)
- `&gt;` - > (greater than)

Example: `Mobile Developer &amp; Frontend Developer`

---

## CSS Rules (When Needed)

### ✅ Allowed (Layout/Position Only)
- `display: flex`, `flex-wrap`, `flex: 1`
- `position: fixed/relative/absolute`
- `margin`, `padding`, `gap`
- `width`, `height`
- `justify-content`, `align-items`, `text-align`
- `overflow: auto`

### ❌ Not Allowed
- Colors, backgrounds, fonts, borders, shadows
- External CSS files or `<style>` tags

---

## Common Patterns

**Section with ID for Navigation:**
```html
<section id="about">
  <h2>About</h2>
  <p>Content here...</p>
</section>
```

**Navigation Links:**
```html
<nav>
  <a href="#about">About</a> | 
  <a href="#skills">Skills</a>
</nav>
```

**Contact Links:**
```html
<a href="mailto:your@email.com">Email</a>
<a href="tel:+919876543210">Phone</a>
```

**Simple Form:**
```html
<form action="#" method="post">
  <label for="name">Name:</label>
  <input type="text" id="name" name="name" required />
  <input type="submit" value="Send" />
</form>
```

---

## Page Layout Structure

### Project 1: Personal Portfolio
```
header
  ├── name & title
  └── contact info

nav
  └── section links

main
  ├── about section
  ├── skills section
  ├── projects section (articles)
  ├── experience section
  ├── education section
  └── contact section (form)

footer
  └── copyright
```

### Project 2: Travel Blog
```
header
  ├── blog title
  └── tagline

nav
  └── page links

main
  ├── home section
  ├── destinations section (articles with images)
  ├── gallery section (multiple images)
  └── contact section (form)

footer
  └── copyright
```

---

## Best Practices

✅ Use semantic HTML tags for better structure

✅ Always include `alt` text for images

✅ Use heading hierarchy (h1 → h2 → h3)

✅ Add `id` attributes to sections for navigation

✅ Use `required` attribute for mandatory form fields

✅ Connect labels to inputs with `for` and `id`

✅ Use HTML entities for special characters (&amp;)
