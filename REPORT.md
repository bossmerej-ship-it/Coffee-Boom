# Assignment 1 Report — Introduction to Web Technologies

**Course:** Introduction to Web Technologies  
**Assignment:** Assignment 1 — Internet & WWW basics, Semantic HTML, Forms, Tables  
**Project Topic:** Coffee Boom (Samal-12 Branch, Astana Tower, Astana)  
**Authors:** Timur Naumov & Merey Kuatbay  
**Student Author (this report):** Timur Naumov  
**Repository:** [https://github.com/bossmerej-ship-it/Coffee-Boom](https://github.com/bossmerej-ship-it/Coffee-Boom)

---

## Task A — Anatomy of a Real Page

### 1. Selected Website
* **Target Website:** Official corporate website of the Coffee Boom coffeehouse chain
* **URL:** `https://coffeeboom.kz`
* **Inspection Date:** September 11, 2026

### 2. Document Head and Metadata Audit
* **DOCTYPE:** `<!DOCTYPE html>` (Standard HTML5 doctype declaration)
* **Language Attribute:** `lang="kk"` inside `<html class="html" lang="kk">`
* **Character Encoding:** Legacy declaration via `<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>`
* **Viewport Configuration:** `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
* **Document Title:** `Coffee Boom — Қазақстан, Ресей және Өзбекстандағы кофеханалар желісі.`
* **Three Key Meta Tags:**
  1. `<meta name="Description" content="Coffee Boom — 2010 жылдан бері жұмыс істеп келе жатқан, 130-дан астам кофеханасы бар халықаралық желі. Өзіміз қуыратын кофе, жеке өндірісіміз және авторлық десерттер — бәрі өзімізден.">`
  2. `<meta name="theme-color" content="whitesmoke">`
  3. `<meta property="og:image" content="https://coffeeboom.kz/wa-data/public/wcms/images/07/04/00/461/461.0x0.png">`

### 3. Semantic Analysis vs. Div-Soup Statistics
A comprehensive scan of the source markup on `https://coffeeboom.kz` revealed severe structural deficiencies:
* `<header>` count: **1**
* `<footer>` count: **1**
* `<main>` count: **1**
* `<nav>` count: **0** (Primary site navigation containing over 20 links is wrapped purely in non-semantic `<div>` containers)
* `<section>` count: **0** (Thematic sections are not demarcated)
* `<article>` count: **0** (Blog posts and CBRB editorial entries lack article semantics)
* `<aside>` count: **0** (No complementary landmarks)
* `<table>` count: **0** (City directories and branch parameters are built using floating div columns)
* `<form>` count: **0** (Interactive applications rely on JavaScript popups without accessible semantic markup)
* `<div>` count: **570** (Extreme reliance on generic div elements for all visual components)

### 4. Three Structural Mistakes and How We Avoided Them

1. **Mistake 1: Extreme "Div-Soup" and Complete Absence of Landmark Navigation (`<nav>`)**
   * *Problem on coffeeboom.kz:* The navigation bar holding 20+ destination links is constructed using unsemantic `<div>` blocks instead of a `<nav>` container. Screen readers cannot locate navigation shortcuts, hurting web accessibility.
   * *Our Solution:* In all our pages (`about.html`, `colophon.html`, `feedback.html`), navigation is strictly wrapped in a semantic `<header>` containing `<nav>` with a standard unordered list (`<ul>` and `<li>`), allowing assistive tools to easily identify navigation landmarks.

2. **Mistake 2: Obsolete Character Encoding Declaration**
   * *Problem on coffeeboom.kz:* The page specifies encoding through the archaic HTTP-EQUIV syntax `<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>` inherited from legacy HTML4 standards.
   * *Our Solution:* We adopted the clean, modern HTML5 standard `<meta charset="UTF-8">` across all documents, which reduces head overhead and parses reliably across modern browsers.

3. **Mistake 3: Zero Data Tables for Tabular Information**
   * *Problem on coffeeboom.kz:* The chain presents data for 20+ regional cities, seating formats, and production facts exclusively via float-based div cards (`<table>` count is 0), making side-by-side data comparison inaccessible for voice readers.
   * *Our Solution:* In `about.html`, we engineered a fully accessible data table using `<table>`, `<caption>`, `<thead>`, `<tbody>`, and explicit scope attributes (`<th scope="col">` and `<th scope="row">`) to clearly convey branch zone capacities and amenities.

### 5. Hand-Drawn Page Structure Sketch
*(Note: A physical hand-drawn wireframe sketch of the coffeeboom.kz layout has been hand-drafted on paper, signed, dated by Timur Naumov, and photographed as `sketch.jpg` in the project directory).*

```text
+--------------------------------------------------------------------------+
|  HEADER (Brand Logo "Coffee Boom", Language Selectors: KZ / RU / EN)     |
+--------------------------------------------------------------------------+
|  DIV [Error: Should be <nav>] (Links: About, Guests, Franchise, Roasting)|
+--------------------------------------------------------------------------+
|  MAIN                                                                    |
|  +--------------------------------------------------------------------+  |
|  | Hero Slider Banner: Visual Promotions & Tagline [DIV]             |  |
|  +--------------------------------------------------------------------+  |
|  | City Locations Bar (Astana, Almaty, Shymkent, Karaganda) [DIV]     |  |
|  +--------------------------------------------------------------------+  |
|  | Magazine & Editorial Stories: CBRB Heritage [Error: No <article>]  |  |
|  +--------------------------------------------------------------------+  |
|  | Coffee Boom Factory & Roasting Production Units [Error: No <sec>]  |  |
|  +--------------------------------------------------------------------+  |
|  | Franchise Application Inquiry CTA Block [DIV]                     |  |
+--------------------------------------------------------------------------+
|  FOOTER (Hotline: +7 707 313-02-02, Email, Social Links, Copyright)      |
+--------------------------------------------------------------------------+
Handwritten signature: Timur Naumov | Date: September 11, 2026
```

---

## Task B — Written Part

### Question & Response (185 words)

A web page is a text document structured with HTML tags that define headings, paragraphs, and tables. When a browser opens our `about.html` file, it reads the code from top to bottom, building an in-memory tree called the DOM (Document Object Model). Without CSS, the browser uses its built-in default styles to calculate margins and fonts, then paints the layout onto the screen.

In my files, I chose semantic tags over generic `<div>` containers in three specific spots:
1. In `about.html`, I chose `<article>` instead of `<div>` for the "Branch Spaces and Standards" section because it forms an independent, self-contained guide.
2. In `about.html`, I used `<aside>` instead of `<div>` for Senior Barista Miras Baitileu’s quote, marking it as complementary side content.
3. In `feedback.html`, I used `<section>` instead of `<div>` to group the review introduction under its own `<h2>` heading.

When a visitor clicks "Submit Feedback" in `feedback.html`, the browser checks required fields via HTML5 validation. If valid, it triggers a POST request to `action="#"`, refreshing the page without sending data because no backend server is connected yet.
