# 📚 Course 1: HTML Basics - Your Web Development Journey Starts Here!

## 🎯 What is HTML?

**HTML** stands for **HyperText Markup Language** 🌐

- 📝 HTML is the **standard markup language** for creating web pages
- 🏗️ It describes the **structure** of a web page
- 🧱 HTML consists of **elements** that tell the browser how to display content
- 🚫 HTML is **NOT** a programming language - it's a markup language!

---

## 🏛️ Basic HTML Structure

Every HTML page has a basic structure. Think of it like building a house! 🏠

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My First Page</title>
  </head>
  <body>
    <h1>Hello World!</h1>
    <p>This is my first web page.</p>
  </body>
</html>
```

### 🔍 Breaking It Down:

- `<!DOCTYPE html>` 📋 - Declares this is an HTML5 document
- `<html>` 🌍 - The root element that wraps all content
- `<head>` 🧠 - Contains meta information (not visible on the page)
- `<title>` 🏷️ - Sets the page title (shows in browser tab)
- `<body>` 🎨 - Contains all visible content
- `<h1>` 📢 - A heading (the biggest one!)
- `<p>` 📄 - A paragraph of text

---

## 🏷️ HTML Tags & Elements

### What Are Tags? 🤔

HTML uses **tags** to create elements. Tags are like labels that wrap around content.

**Anatomy of an HTML Element:**

```
<tagname>Content goes here</tagname>
   ↑            ↑              ↑
Opening Tag  Content      Closing Tag
```

### 📌 Important Concepts:

- **Opening tag:** `<p>` ➡️ Starts the element
- **Content:** The text or nested elements
- **Closing tag:** `</p>` ⬅️ Ends the element
- **Self-closing tags:** Some tags don't need closing tags! Example: `<br>` or `<img>`

---

## 📝 Essential HTML Tags You Must Know

### 1️⃣ Headings (h1 - h6) 📢

Headings organize your content from most important to least important:

```html
<h1>Main Heading - Biggest!</h1>
<h2>Subheading</h2>
<h3>Smaller heading</h3>
<h4>Even smaller</h4>
<h5>Getting tiny</h5>
<h6>Smallest heading</h6>
```

💡 **Tip:** Use only ONE `<h1>` per page for SEO!

---

### 2️⃣ Paragraphs 📄

```html
<p>This is a paragraph. It contains text that forms a complete thought.</p>
<p>This is another paragraph. Browsers automatically add space between paragraphs.</p>
```

---

### 3️⃣ Links (Anchor Tags) 🔗

Links let users navigate between pages:

```html
<a href="https://www.google.com">Click here to visit Google!</a>
<a href="page2.html">Go to Page 2</a>
<a href="#section1">Jump to Section 1 on this page</a>
```

**Attributes:**
- `href` 🎯 - The destination URL
- `target="_blank"` 🪟 - Opens link in new tab

---

### 4️⃣ Images 🖼️

```html
<img src="photo.jpg" alt="Description of image">
<img src="https://example.com/image.png" alt="Online image" width="300">
```

**Attributes:**
- `src` 📍 - Path to the image file
- `alt` 📝 - Alternative text (for accessibility & SEO)
- `width` & `height` 📏 - Size of the image

⚠️ **Note:** `<img>` is a self-closing tag!

---

### 5️⃣ Lists 📋

**Unordered List (Bullets):**

```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```

**Ordered List (Numbers):**

```html
<ol>
  <li>First step</li>
  <li>Second step</li>
  <li>Third step</li>
</ol>
```

---

### 6️⃣ Divisions & Spans 📦

**`<div>` - Block Container:**

```html
<div>
  <h2>Section Title</h2>
  <p>This div groups related content together.</p>
</div>
```

**`<span>` - Inline Container:**

```html
<p>This is <span style="color: red;">important</span> text.</p>
```

🔑 **Key Difference:**
- `<div>` 📦 - Block-level (takes full width, starts on new line)
- `<span>` ✨ - Inline (only takes needed space, stays in line)

---

### 7️⃣ Line Breaks & Horizontal Rules ➖

```html
<p>This is line one.<br>This is line two.</p>
<hr>
<p>Content after a horizontal line.</p>
```

- `<br>` ⤵️ - Line break (self-closing)
- `<hr>` ➖ - Horizontal rule/separator (self-closing)

---

### 8️⃣ Text Formatting ✍️

```html
<strong>Bold text (important)</strong>
<b>Bold text (stylistic)</b>
<em>Italic text (emphasis)</em>
<i>Italic text (stylistic)</i>
<u>Underlined text</u>
<mark>Highlighted text</mark>
<small>Smaller text</small>
<del>Deleted text</del>
<ins>Inserted text</ins>
```

---

## 🎨 HTML Attributes

Attributes provide **additional information** about elements.

### Common Attributes:

```html
<element attribute="value">Content</element>
```

**Examples:**

```html
<img src="image.jpg" alt="Photo" width="200">
      ↑         ↑        ↑          ↑
   attribute  value  attribute   value

<a href="page.html" target="_blank" title="Click me!">Link</a>

<p id="intro" class="highlight">Text with ID and class</p>
```

### 🌟 Universal Attributes (work on any element):

- `id` 🆔 - Unique identifier for an element
- `class` 🏷️ - Class name(s) for styling
- `style` 🎨 - Inline CSS styling
- `title` 💬 - Tooltip text on hover

---

## 📊 Tables 📋

Tables organize data in rows and columns:

```html
<table>
  <tr>
    <th>Name</th>
    <th>Age</th>
    <th>City</th>
  </tr>
  <tr>
    <td>John</td>
    <td>25</td>
    <td>New York</td>
  </tr>
  <tr>
    <td>Sarah</td>
    <td>30</td>
    <td>London</td>
  </tr>
</table>
```

- `<table>` 📊 - Creates a table
- `<tr>` ↔️ - Table row
- `<th>` 🏆 - Table header (bold & centered)
- `<td>` 📝 - Table data cell

---

## 📝 Forms 📬

Forms collect user input:

```html
<form action="/submit" method="POST">
  <label for="name">Name:</label>
  <input type="text" id="name" name="name">
  
  <label for="email">Email:</label>
  <input type="email" id="email" name="email">
  
  <label for="message">Message:</label>
  <textarea id="message" name="message" rows="4"></textarea>
  
  <button type="submit">Send</button>
</form>
```

### Common Input Types:

- `type="text"` ✏️ - Text input
- `type="email"` 📧 - Email input
- `type="password"` 🔒 - Password input
- `type="number"` 🔢 - Number input
- `type="checkbox"` ☑️ - Checkbox
- `type="radio"` 🔘 - Radio button
- `type="submit"` 📤 - Submit button

---

## 🎯 Semantic HTML5 Elements

Semantic elements clearly describe their meaning:

```html
<header>
  <nav>
    <a href="#home">Home</a>
    <a href="#about">About</a>
  </nav>
</header>

<main>
  <article>
    <h2>Article Title</h2>
    <p>Article content goes here...</p>
  </article>
  
  <section>
    <h2>Section Title</h2>
    <p>Section content...</p>
  </section>
</main>

<aside>
  <p>Sidebar content</p>
</aside>

<footer>
  <p>&copy; 2026 My Website</p>
</footer>
```

### 📌 Semantic Tags:

- `<header>` 🎯 - Page or section header
- `<nav>` 🧭 - Navigation links
- `<main>` 🎪 - Main content
- `<article>` 📰 - Self-contained content
- `<section>` 📑 - Thematic grouping
- `<aside>` 📌 - Sidebar content
- `<footer>` 👟 - Page or section footer

---

## 💡 HTML Best Practices

### ✅ DO:

1. **Always close tags properly** 🔒
2. **Use lowercase for tags and attributes** (modern standard)
3. **Quote attribute values** `<img src="photo.jpg">`
4. **Use semantic HTML** for better accessibility & SEO
5. **Add alt text to images** for accessibility ♿
6. **Indent nested elements** for readability 📖
7. **Use meaningful ID and class names** 🏷️

### ❌ DON'T:

1. **Forget the DOCTYPE** declaration
2. **Use deprecated tags** like `<font>` or `<center>`
3. **Mix up opening and closing tags**
4. **Use inline styles everywhere** (use CSS instead!)
5. **Skip alt attributes on images**

---

## 🎓 Practice Exercise

Create a simple "About Me" page with:

✅ A main heading with your name  
✅ A paragraph about yourself  
✅ An image (can be any image)  
✅ A list of your hobbies  
✅ A link to your favorite website  
✅ Proper HTML structure (DOCTYPE, html, head, body)

---

## 🎉 Summary

You've learned:

- ✅ What HTML is and its basic structure
- ✅ How tags and elements work
- ✅ Essential HTML tags (headings, paragraphs, links, images, lists)
- ✅ HTML attributes
- ✅ Tables and forms
- ✅ Semantic HTML5 elements
- ✅ Best practices

---

## 🚀 Next Steps

In Course 2, you'll learn:
- 🎨 CSS Basics (styling your HTML)
- 🎯 Advanced HTML forms
- 📱 Making pages responsive

Keep practicing! The more you code, the better you'll get! 💪✨