# Semantic HTML Blog Project

## 📄 Overview

This project is a step-by-step practice of creating a well-structured, semantic, and accessible HTML document. The goal is to understand and implement best practices in semantic HTML, accessibility (ARIA roles), and basic metadata for SEO.

## ✅ Objectives Achieved

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

## 🛠️ Tools Used
- HTML5
- Manual editing in a text editor (e.g. VS Code)

---

## 📌 Author
**Tracy Karanja🌸**

---

