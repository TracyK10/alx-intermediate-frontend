# Semantic HTML, Tailwind CSS & Sass Practice Project

## 📄 Overview

This project is a hands-on exploration of **semantic HTML**, **Tailwind CSS**, and **Sass/SCSS**, aimed at building responsive, accessible, and modular web layouts. It includes tasks that progressively develop skills in structuring HTML documents semantically, designing layouts with utility-first CSS (Tailwind), and writing maintainable styles using Sass features like variables, nesting, and mixins. All configurations and setups were completed on a **Windows environment** using **Node.js**, **PowerShell**, and the **Sass CLI**.


## ✅ Project Breakdown

### ✅ 1. Basic HTML Structure (`0-index.html`)
- Created an HTML5 document using `<!DOCTYPE html>`.
- Included `<html>`, `<head>`, and `<body>` tags.
- Added a `<header>` with a `<nav>` containing three links.
- Added a `<main>` with an `<article>` that includes:
  - `<h1>` title
  - A `<section>` with dummy blog content.
- Included a `<footer>` with copyright.

---

### ✅ 2. Meta Tags & SEO (`1-index.html`)
- Added semantic meta tags inside `<head>`:
  - `charset="UTF-8"`
  - `description`
  - `keywords`
  - `author`
  - `viewport`
- Updated the `<title>` to `"Semantic Html Blog Post"`.

---

### ✅ 3. Semantic Blog Layout (`2-index.html`)
- Enhanced the article section to represent a real blog post.
- Added a nested `<header>` inside `<article>` with:
  - `<h2>` title
  - `<time>` tag for publication date.
- Divided content into three `<section>` blocks:
  - **Introduction**: explained semantic HTML.
  - **Main Content**: included `<code>` examples and a `<figure>` with image and caption.
  - **Conclusion**: summarized the benefits of semantic HTML.
- Added an article-specific `<footer>` with author and publish date.

---

### ✅ 4. Accessible Form with ARIA (`3-index.html`)
- Created a new `<section>` inside `<main>` for a contact form.
- Added a `<form>` element with:
  - `action="#"`, `method="POST"`, `aria-labelledby`, and `role="form"`
- Included:
  - A heading with `id="form-title"` for ARIA reference.
  - Input fields for `Name` and `Email` using `aria-required="true"`.
  - A `submit` `<button>` with `aria-label="Submit the form"`.
  - A live alert `<div>` with `aria-live="polite"` and `role="alert"`.

---

## 🎯 Key Learnings
- How to build semantic HTML with `<header>`, `<nav>`, `<main>`, `<article>`, `<section>`, `<footer>`.
- Importance of meta tags for SEO and accessibility.
- Using ARIA roles and attributes to improve screen reader accessibility.
- Organizing content in a meaningful and structured way.

---

  
## 📂 Project Structure

```
0x00-semantic html/
├── 0-index.html              
├── 1-index.html              
├── 2-index.html              
├── 3-index.html             
```
---

## 📅 Tailwind CSS Layout Practice

### 5. Tailwind Setup (`tailwind.config.js`, `src/input.css`, `src/output.css`)
- Installed and configured Tailwind CSS via CLI.
- Created `tailwind.config.js` to scan `src/**/*.{html,js}`.
- Used `@tailwind base;`, `@tailwind components;`, and `@tailwind utilities;` in `input.css`.
- Ran CLI to watch and generate `output.css`.

---

### 6. Basic Grid Layout (`src/1-index.html`)
- Created a 3-column CSS grid layout using Tailwind:
  ```html
  class="grid grid-cols-3 gap-4"

* Applied background colors and responsive design.

---

### 7. Nested Grids (`src/2-index.html`)

* Created a 2x2 grid layout with nested grids inside each column.
* Styled inner content with gradient backgrounds and padding.

---

### 8. Flexbox Navigation Bar (`src/3-nav_index.html`)

* Created a horizontal nav bar with Tailwind Flexbox.
* Applied spacing, text styling, hover effects, and responsive column behavior using media queries.

---

### 9. Responsive Flexbox Layout (`src/4-flexbox_index.html`)

* Used `flex` class to layout an `aside` and `section`.
* Applied width classes (`w-1/3` and `w-2/3`) and responsive direction changes.

---

### 10. Combining Grid & Flexbox (`src/5-gridflex_index.html`)

* Created a responsive layout using both Grid and Flexbox.
* Used:

  ```html
  class="grid grid-cols-1 lg:grid-cols-3"
  class="lg:col-span-2 flex"
  ```
* Ensured elements adjusted based on screen size.

---

### 11. Responsive Image Gallery (`src/6-imageGallery.html`)

* Added a responsive gallery using Tailwind Grid:

  * 3 columns on large screens: `lg:grid-cols-3`
  * 1 column on small screens: `grid-cols-1`
* Made images responsive using `w-full`, `h-48`, and `object-cover`.

---

## 📍 Project Structure

```
0x02-tailwind-css/
├── tailwind.config.js
├── src/
|   |── images/
│   ├── input.css
│   ├── output.css
│   ├── 0-index.html
│   ├── 1-index.html
│   ├── 2-index.html
│   ├── 3-index.html
│   ├── 3-nav_index.html
│   ├── 4-flexbox_index.html
│   ├── 5-gridflex_index.html
│   └── 6-imageGallery.html
```

---

## 🎨 Sass / SCSS Practice

> ⚙️ **Environment**: Development and compilation were done on **Windows** using Node.js and the Sass CLI.

### ✅ 1. Debugging Output (`0-debug_log.scss`)

* Used `@debug` to print a debug message:

  ```scss
  @debug "Hello world";
  ```

---

### ✅ 2. Color Variable (`1-color_variable.scss`)

* Declared a variable `$text-color: #3D3D3D;`
* Applied it to both `body` and `p` tags using Sass variable syntax.

---

### ✅ 3. Nested Tags (`2-nested_tag.scss`)

* Nested the `p` selector inside `body`:

  ```scss
  body {
    margin: 0px;
    padding: 0px;

    p {
      margin: 10px;
    }
  }
  ```

---

### ✅ 4. Margin Mixins (`8-mixin_margins.scss`)

* Created a mixin for horizontal margins:

  ```scss
  @mixin margins($value) {
    margin-left: $value;
    margin-right: $value;
  }
  ```
* Applied it using `@include`:

  * `@include margins(10px);` on `body`
  * `@include margins(15px);` on `div`

---

### ⚙️ Sass Installation and Compilation on Windows

#### Installation

```bash
npm install -g sass
```

#### Compilation Command

To compile a `.scss` file to `.css`:

```bash
sass input.scss output.css
```

To watch a file for changes and auto-compile:

```bash
sass --watch input.scss:output.css
```

You can also watch an entire folder:

```bash
sass --watch src/:dist/
```

> ℹ️ Replace `src/` with the folder containing your `.scss` files and `dist/` with the output destination for `.css` files.

---

## 📁 Sass Project Structure

```
0x03-sass_scss/
├── 0-debug_log.scss
├── 1-color_variable.scss
├── 2-nested_tag.scss
├── 3-mixin_margins.scss
```

---

## 🔬 Learning Objectives

* **Semantic HTML**: Proper document structure and accessibility using semantic tags.
* **Tailwind CSS**: Utility-first CSS framework for responsive design.
* **Flexbox & Grid**: Combined use of modern layout systems.
* **ARIA**: Accessible web forms with screen reader support.
* **Responsiveness**: Mobile-first layouts using Tailwind modifiers.
* **SEO**: Use of metadata and structure for improved discoverability.
* **Sass / SCSS**: Writing maintainable and modular CSS using variables, nesting, and mixins.
* **Command Line & Environment Setup**: Installing and running tools like Node.js and Sass CLI on Windows.

---

## 💡 Requirements

* Node.js (v14 or higher recommended)
* Windows terminal or PowerShell (for Windows users)
* Sass CLI (`npm install -g sass`)
* Basic knowledge of HTML, CSS, JavaScript
* Familiarity with VS Code or a similar code editor
* Git & GitHub for version control
* Tailwind CSS via npm or CDN
* A modern browser (e.g. Chrome, Firefox, Edge)

---

## 💧 Tools Used

* **HTML5**
* **Sass / SCSS** (CLI + modular CSS)
* **Tailwind CSS** (via CDN & CLI)
* **Visual Studio Code**
* **Git & GitHub**
* **Windows PowerShell** (for setup and CLI execution)

---


## 📎 Author

**Tracy Karanja 🌸**
*Student, Frontend Developer & Tech Enthusiast*

---

