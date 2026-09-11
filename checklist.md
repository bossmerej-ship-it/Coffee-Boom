# HTML Tag Checklist — Coffee Boom Website

**Authors:** Timur Naumov & Merey Kuatbay  
**Project:** Coffee Boom (Samal-12 Branch, Astana)  
**Student Pages by Timur Naumov:** `colophon.html`, `about.html`, `feedback.html`

---

## 1. Universal Requirements (Present on Every Page)

| Requirement / Element | File | Exact Line Number | Author | Description / Usage |
| :--- | :--- | :---: | :--- | :--- |
| `<!DOCTYPE html>` | `colophon.html`<br>`about.html`<br>`feedback.html` | Line 1<br>Line 1<br>Line 1 | Timur Naumov | Declares HTML5 document type |
| `<html lang="en">` | `colophon.html`<br>`about.html`<br>`feedback.html` | Line 2<br>Line 2<br>Line 2 | Timur Naumov | Root element with English language attribute |
| `<meta charset="UTF-8">` | `colophon.html`<br>`about.html`<br>`feedback.html` | Line 4<br>Line 4<br>Line 4 | Timur Naumov | Character encoding declaration |
| `<meta name="viewport">` | `colophon.html`<br>`about.html`<br>`feedback.html` | Line 5<br>Line 5<br>Line 5 | Timur Naumov | Responsive viewport configuration |
| `<meta name="description">` | `colophon.html`<br>`about.html`<br>`feedback.html` | Line 6<br>Line 6<br>Line 6 | Timur Naumov | Search engine description snippet |
| `<meta name="author">` | `colophon.html`<br>`about.html`<br>`feedback.html` | Line 7<br>Line 7<br>Line 7 | Timur Naumov | Author metadata attribution |
| Author HTML Comment | `colophon.html`<br>`about.html`<br>`feedback.html` | Line 11<br>Line 11<br>Line 11 | Timur Naumov | `<!-- Page author: Timur Naumov -->` |
| Unique `<title>` | `colophon.html`<br>`about.html`<br>`feedback.html` | Line 8<br>Line 8<br>Line 8 | Timur Naumov | Specific document title for browser tab |
| Exactly one `<h1>` | `colophon.html`<br>`about.html`<br>`feedback.html` | Line 14<br>Line 14<br>Line 14 | Timur Naumov | Single top-level heading in `<header>` |
| Correct heading hierarchy | `colophon.html`<br>`about.html`<br>`feedback.html` | Lines 14, 30, 34<br>Lines 14, 32, 45, 60<br>Lines 14, 30, 41 | Timur Naumov | `h1` &rarr; `h2` &rarr; `h3` without skipping levels |
| `<header>` | `colophon.html`<br>`about.html`<br>`feedback.html` | Line 13<br>Line 13<br>Line 13 | Timur Naumov | Site name and banner container |
| `<nav>` | `colophon.html`<br>`about.html`<br>`feedback.html` | Line 18<br>Line 15<br>Line 15 | Timur Naumov | Navigation with relative links to all 6 pages |
| `<main>` | `colophon.html`<br>`about.html`<br>`feedback.html` | Line 29<br>Line 27<br>Line 27 | Timur Naumov | Unique primary document content container |
| `<footer>` | `colophon.html`<br>`about.html`<br>`feedback.html` | Line 79<br>Line 139<br>Line 115 | Timur Naumov | Footer with contacts and copyright entity |
| Explanatory Comments | `colophon.html`<br>`about.html`<br>`feedback.html` | Lines 33, 50, 59, 63<br>Lines 30, 43, 125<br>Lines 28, 39, 44 | Timur Naumov | Substantive comments explaining architectural rationale |

---

## 2. Structural & Semantic Elements

| Element | File | Exact Line Number | Author | Description / Context |
| :--- | :--- | :---: | :--- | :--- |
| `<section>` | `about.html` | Lines 31, 85 | Timur Naumov | Location/atmosphere and hall capacity sections |
| `<article>` | `about.html` | Line 44 | Timur Naumov | Branch spaces and operational standards guide |
| `<aside>` | `about.html` | Line 120 | Timur Naumov | Senior barista quote and secondary contact block |
| `<figure>` | `about.html` | Lines 37, 79, 115 | Timur Naumov | Image containers for facade, hall, and seating |
| `<figcaption>` | `about.html` | Lines 39, 81 | Timur Naumov | Descriptive captions for facade and guest hall |

---

## 3. Data Tables

| Element | File | Exact Line Number | Author | Description / Context |
| :--- | :--- | :---: | :--- | :--- |
| `<table>` | `about.html` | Line 89 | Timur Naumov | Table describing hall zones, seats, sockets, and features |
| `<caption>` | `about.html` | Line 90 | Timur Naumov | Table caption: *Seating Capacity and Features at Samal 12* |
| `<thead>` | `about.html` | Line 91 | Timur Naumov | Header group containing column labels |
| `<tbody>` | `about.html` | Line 99 | Timur Naumov | Body group containing zone records |
| `<th scope="col">` | `about.html` | Lines 93, 94, 95, 96 | Timur Naumov | Column headers with explicit `scope="col"` |
| `<th scope="row">` | `about.html` | Lines 101, 107 | Timur Naumov | Row headers with explicit `scope="row"` |

---

## 4. Lists

| List Type | File | Exact Line Number | Author | Description / Context |
| :--- | :--- | :---: | :--- | :--- |
| Nested List | `about.html` | Lines 50–59 | Timur Naumov | `<ul>` of zones containing nested `<ul>` of features |
| Ordered List with Attribute | `about.html` | Line 65 | Timur Naumov | `<ol type="1" start="1">` service sequence steps |
| Definition List (`<dl>`) | `about.html` | Line 72 | Timur Naumov | Glossary container for branch zones |
| Definition Term (`<dt>`) | `about.html` | Lines 73, 75 | Timur Naumov | Terms: *Indoor Hall* and *Summer Veranda* |
| Definition Description (`<dd>`) | `about.html` | Lines 74, 76 | Timur Naumov | Descriptions of seating and layout for each zone |

---

## 5. Hyperlinks & Media

| Element / Link Type | File | Exact Line Number | Author | Description / Context |
| :--- | :--- | :---: | :--- | :--- |
| External Link (`target`, `rel`) | `about.html` | Line 131 | Timur Naumov | `<a href="https://go.2gis.com/3NTY2" target="_blank" rel="noopener noreferrer">` |
| `mailto:` Link | `about.html` | Line 132 | Timur Naumov | `<a href="mailto:samal@coffeeboom.kz">` |
| `tel:` Link | `about.html` | Line 140 | Timur Naumov | `<a href="tel:+77073130202">` |
| Same-Page Anchor Link 1 | `about.html` | Line 28 | Timur Naumov | `<a href="#branch-zones">Zones</a>` |
| Same-Page Anchor Link 2 | `about.html` | Line 28 | Timur Naumov | `<a href="#branch-capacity">Capacity</a>` |
| Image 1 with meaningful `alt` | `about.html` | Line 38 | Timur Naumov | `images/coffee-shop.jpg` (Front entrance and signage) |
| Image 2 with meaningful `alt` | `about.html` | Line 80 | Timur Naumov | `images/hall.jpeg` (Interior dining hall and tables) |
| Image 3 with meaningful `alt` | `about.html` | Line 116 | Timur Naumov | `images/cozy.jpg` (Comfortable sofa seating and wall quote) |

---

## 6. Typography, Quotes & Phrase Elements

| Element | File | Exact Line Number | Author | Description / Context |
| :--- | :--- | :---: | :--- | :--- |
| `<strong>` | `about.html` | Lines 50, 56 | Timur Naumov | Highlighting zone names in list |
| `<em>` | `about.html` | Line 127 | Timur Naumov | Emphasizing *hospitable service* quote |
| `<b>` | `about.html` | Lines 73, 75 | Timur Naumov | Bold styling for definition terms |
| `<i>` | `about.html` | Line 34 | Timur Naumov | Italicized technical term *Wi-Fi* |
| `<mark>` | `about.html` | Line 127 | Timur Naumov | Highlighting *hospitable service* |
| `<small>` | `about.html` | Line 131 | Timur Naumov | Fine print label for map link |
| `<sup>` | `about.html` | Line 67 | Timur Naumov | Superscript temperature unit: `65<sup>&deg;</sup>C` |
| `<abbr title="...">` (1) | `about.html` | Line 34 | Timur Naumov | `<abbr title="Business Center">BC</abbr>` |
| `<abbr title="...">` (2) | `about.html` | Line 34 | Timur Naumov | `<abbr title="Wireless Fidelity">Wi-Fi</abbr>` |
| `<blockquote>` | `about.html` | Line 123 | Timur Naumov | Real quote from Senior Barista Miras Baitileu |
| Inline `<q>` | `about.html` | Line 127 | Timur Naumov | Inline quote from senior barista |
| `<cite>` | `about.html` | Line 126 | Timur Naumov | Citation of speaker: *Miras Baitileu* |
| `<hr>` | `about.html` | Line 137 | Timur Naumov | Thematic divider preceding footer |
| `<br>` | `about.html` | Line 140 | Timur Naumov | Line break inside contact details |
| `<code>` | `colophon.html` | Line 52 | Timur Naumov | Code markup example |
| `<pre>` | `colophon.html` | Line 52 | Timur Naumov | Preformatted code block |
| `<kbd>` | `colophon.html` | Line 47 | Timur Naumov | Keyboard input: `<kbd>Ctrl</kbd> + <kbd>S</kbd>` |
| `<samp>` | `colophon.html` | Line 61 | Timur Naumov | Sample output from W3C syntax validator |
| HTML Entities | `about.html` | Lines 28, 67, 126, 140, 141 | Timur Naumov | `&copy;`, `&mdash;`, `&bull;`, `&deg;`, `&amp;` |

---

## 7. `<div>` and `<span>` Elements with Justifications

| Element | File | Exact Line Number | Author | Rationale / Why No Semantic Tag Fit |
| :--- | :--- | :---: | :--- | :--- |
| `<div>` | `about.html` | Line 130 | Timur Naumov | Acts strictly as a neutral grouping container for secondary map and email contact links inside `<aside>`, where no structural section (`section`/`article`) or semantic phrasing element applies. |
| `<span>` | `colophon.html` | Line 64 | Timur Naumov | Applied solely to isolate an arbitrary technical build version label where no phrasing tag like `strong`, `em`, or `mark` fits the neutral semantics. |

---

## 8. Interactive Form Elements

| Element / Attribute | File | Exact Line Number | Author | Description / Context |
| :--- | :--- | :---: | :--- | :--- |
| `<form>` (`method`, `action`) | `feedback.html` | Line 43 | Timur Naumov | `<form method="post" action="#">` |
| Form Backend Notice Comment | `feedback.html` | Line 44 | Timur Naumov | Explicit comment that no backend exists yet |
| `<fieldset>` | `feedback.html` | Lines 46, 63 | Timur Naumov | Grouping containers for contacts and review |
| `<legend>` | `feedback.html` | Lines 47, 64 | Timur Naumov | Captions for each fieldset |
| `<label>` bound to field by `id` | `feedback.html` | Lines 50, 54, 58, 66, 70, 74, 85, 88, 91, 95, 101 | Timur Naumov | Every label bound via `for` attribute matching input `id` |
| `type="text"` | `feedback.html` | Line 51 | Timur Naumov | Full name field |
| `type="email"` | `feedback.html` | Line 55 | Timur Naumov | Email address field |
| `type="tel"` | `feedback.html` | Line 59 | Timur Naumov | Phone number field |
| `type="date"` | `feedback.html` | Line 67 | Timur Naumov | Date of visit field |
| `type="number"` | `feedback.html` | Line 71 | Timur Naumov | Rating field (min 1, max 10) |
| `type="radio"` (Radio Group) | `feedback.html` | Lines 84, 87, 90 | Timur Naumov | Purpose of visit selection (`name="purpose"`) |
| `<select>` and `<option>` | `feedback.html` | Lines 75–79 | Timur Naumov | Seating zone dropdown menu |
| `<textarea>` | `feedback.html` | Line 96 | Timur Naumov | Multiline guest feedback comment box |
| `type="checkbox"` | `feedback.html` | Line 100 | Timur Naumov | Data processing consent checkbox |
| `required` attribute | `feedback.html` | Lines 51, 55, 67, 71, 75, 84, 96, 100 | Timur Naumov | Enforces required completion before submission |
| `placeholder` attribute | `feedback.html` | Lines 51, 55, 59, 71, 96 | Timur Naumov | Informative input hints and examples |
| `<button type="submit">` | `feedback.html` | Line 105 | Timur Naumov | Form submission trigger button |
| `<button type="reset">` | `feedback.html` | Line 106 | Timur Naumov | Form field reset trigger button |
