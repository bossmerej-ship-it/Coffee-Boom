# HTML Tag Checklist — Coffee Boom Website

**Authors / Team:** Timur Naumov & Merey Kuatbay  
**Course:** Introduction to Web Technologies — Assignment 1  
**Project:** Coffee Boom (Samal-12 Branch, Astana Tower, Astana)  
**Repository:** [https://github.com/bossmerej-ship-it/Coffee-Boom](https://github.com/bossmerej-ship-it/Coffee-Boom)

### Student Page Allocation:
* **Timur Naumov:** `colophon.html`, `about.html`, `feedback.html`
* **Merey Kuatbay:** `index.html`, `menu.html`, `order.html`

---

## 1. Universal Requirements (Present on Every Page)

| Requirement / Element | File | Exact Line Number | Author | Description / Usage |
| :--- | :--- | :---: | :--- | :--- |
| `<!DOCTYPE html>` | `colophon.html`<br>`about.html`<br>`feedback.html`<br>`index.html`<br>`menu.html`<br>`order.html` | Line 1<br>Line 1<br>Line 1<br>Line 1<br>Line 1<br>Line 1 | Timur Naumov &<br>Merey Kuatbay | Standard HTML5 document type declaration on all 6 pages |
| `<html lang="en">` | `colophon.html`<br>`about.html`<br>`feedback.html`<br>`index.html`<br>`menu.html`<br>`order.html` | Line 2<br>Line 2<br>Line 2<br>Line 2<br>Line 2<br>Line 2 | Timur Naumov &<br>Merey Kuatbay | Root element specifying English language |
| `<meta charset="UTF-8">` | `colophon.html`<br>`about.html`<br>`feedback.html`<br>`index.html`<br>`menu.html`<br>`order.html` | Line 4<br>Line 4<br>Line 4<br>Line 4<br>Line 4<br>Line 4 | Timur Naumov &<br>Merey Kuatbay | UTF-8 character encoding declaration |
| `<meta name="viewport">` | `colophon.html`<br>`about.html`<br>`feedback.html`<br>`index.html`<br>`menu.html`<br>`order.html` | Line 5<br>Line 5<br>Line 5<br>Line 5<br>Line 5<br>Line 5 | Timur Naumov &<br>Merey Kuatbay | Responsive mobile viewport configuration |
| `<meta name="description">` | `colophon.html`<br>`about.html`<br>`feedback.html`<br>`index.html`<br>`menu.html`<br>`order.html` | Line 6<br>Line 6<br>Line 6<br>Line 6<br>Line 6<br>Line 6 | Timur Naumov &<br>Merey Kuatbay | Document description meta tag |
| `<meta name="author">` | `colophon.html`<br>`about.html`<br>`feedback.html`<br>`index.html`<br>`menu.html`<br>`order.html` | Line 7<br>Line 7<br>Line 7<br>Line 7<br>Line 7<br>Line 7 | Timur Naumov &<br>Merey Kuatbay | Author attribution meta tag |
| Author HTML Comment | `colophon.html`<br>`about.html`<br>`feedback.html`<br>`index.html`<br>`menu.html`<br>`order.html` | Line 11<br>Line 11<br>Line 11<br>Line 11<br>Line 11<br>Line 11 | Timur Naumov &<br>Merey Kuatbay | HTML comment identifying the author of each page |
| Unique `<title>` | `colophon.html`<br>`about.html`<br>`feedback.html`<br>`index.html`<br>`menu.html`<br>`order.html` | Line 8<br>Line 8<br>Line 8<br>Line 8<br>Line 8<br>Line 8 | Timur Naumov &<br>Merey Kuatbay | Unique document title for browser tab |
| Exactly one `<h1>` | `colophon.html`<br>`about.html`<br>`feedback.html`<br>`index.html`<br>`menu.html`<br>`order.html` | Line 14<br>Line 14<br>Line 14<br>Line 15<br>Line 15<br>Line 15 | Timur Naumov &<br>Merey Kuatbay | Exactly one `<h1>` heading in header on each page |
| Correct heading hierarchy | `colophon.html`<br>`about.html`<br>`feedback.html` | Lines 14, 30, 34<br>Lines 14, 32, 45, 60<br>Lines 14, 30, 41 | Timur Naumov | `h1` &rarr; `h2` &rarr; `h3` without skipped levels |
| `<header>` | `colophon.html`<br>`about.html`<br>`feedback.html`<br>`index.html`<br>`menu.html`<br>`order.html` | Line 13<br>Line 13<br>Line 13<br>Line 14<br>Line 14<br>Line 14 | Timur Naumov &<br>Merey Kuatbay | Semantic header enclosing brand and navigation |
| `<nav>` | `colophon.html`<br>`about.html`<br>`feedback.html`<br>`index.html`<br>`menu.html`<br>`order.html` | Line 18<br>Line 15<br>Line 15<br>Line 16<br>Line 16<br>Line 16 | Timur Naumov &<br>Merey Kuatbay | Semantic nav with relative links to all 6 pages |
| `<main>` | `colophon.html`<br>`about.html`<br>`feedback.html`<br>`index.html`<br>`menu.html`<br>`order.html` | Line 29<br>Line 27<br>Line 27<br>Line 26<br>Line 26<br>Line 26 | Timur Naumov &<br>Merey Kuatbay | Main content wrapper on each page |
| `<footer>` | `colophon.html`<br>`about.html`<br>`feedback.html`<br>`index.html`<br>`menu.html`<br>`order.html` | Line 79<br>Line 139<br>Line 115<br>Line 60<br>Line 134<br>Line 142 | Timur Naumov &<br>Merey Kuatbay | Semantic footer with contacts and copyright entity |
| Explanatory Comments | `colophon.html`<br>`about.html`<br>`feedback.html` | Lines 33, 50, 59, 63<br>Lines 30, 43, 125<br>Lines 28, 39, 44 | Timur Naumov | Comments explaining *why* a semantic choice was made |

---

## 2. Structural & Semantic Elements

| Element | File | Exact Line Number | Author | Description / Context |
| :--- | :--- | :---: | :--- | :--- |
| `<section>` | `about.html`<br>`feedback.html`<br>`index.html`<br>`menu.html` | Lines 31, 85<br>Line 29<br>Lines 27, 43, 53<br>Lines 27, 40, 116 | Timur Naumov<br>Timur Naumov<br>Merey Kuatbay<br>Merey Kuatbay | Thematic grouping of branch and menu information |
| `<article>` | `about.html`<br>`feedback.html` | Line 44<br>Line 40 | Timur Naumov<br>Timur Naumov | Independent guides for branch spaces and feedback form |
| `<aside>` | `about.html` | Line 120 | Timur Naumov | Senior barista quote and secondary contact block |
| `<figure>` | `about.html`<br>`index.html`<br>`menu.html` | Lines 37, 79, 115<br>Line 37<br>Line 31 | Timur Naumov<br>Merey Kuatbay<br>Merey Kuatbay | Image wrappers for branch photos and bakery displays |
| `<figcaption>` | `about.html`<br>`index.html`<br>`menu.html` | Lines 39, 81<br>Line 39<br>Line 33 | Timur Naumov<br>Merey Kuatbay<br>Merey Kuatbay | Descriptive captions accompanying figures |

---

## 3. Data Tables

| Element | File | Exact Line Number | Author | Description / Context |
| :--- | :--- | :---: | :--- | :--- |
| `<table>` | `about.html`<br>`menu.html` | Line 89<br>Line 42 | Timur Naumov<br>Merey Kuatbay | Seating capacity table (Timur) and beverage pricing table (Merey) |
| `<caption>` | `about.html`<br>`menu.html` | Line 90<br>Line 43 | Timur Naumov<br>Merey Kuatbay | Accessible table title captions |
| `<thead>` | `about.html`<br>`menu.html` | Line 91<br>Line 44 | Timur Naumov<br>Merey Kuatbay | Header rows container |
| `<tbody>` | `about.html`<br>`menu.html` | Line 99<br>Line 52 | Timur Naumov<br>Merey Kuatbay | Data rows container |
| `<th scope="col">` | `about.html`<br>`menu.html` | Lines 93, 94, 95, 96<br>Lines 46, 47, 48, 49 | Timur Naumov<br>Merey Kuatbay | Column header labels with scope |
| `<th scope="row">` | `about.html`<br>`menu.html` | Lines 101, 107<br>Lines 54, 75, 91, 109 | Timur Naumov<br>Merey Kuatbay | Row header labels with scope |

---

## 4. Lists

| List Type | File | Exact Line Number | Author | Description / Context |
| :--- | :--- | :---: | :--- | :--- |
| Nested List | `about.html` | Lines 50–59 | Timur Naumov | `<ul>` of zones containing nested `<ul>` of amenities |
| Ordered List with Attribute | `about.html`<br>`menu.html` | Line 65<br>Line 118 | Timur Naumov<br>Merey Kuatbay | `<ol type="1" start="1">` service steps (Timur) and `<ol>` ordering steps (Merey) |
| Definition List (`<dl>`) | `about.html` | Line 72 | Timur Naumov | Glossary container for branch zones |
| Definition Term (`<dt>`) | `about.html` | Lines 73, 75 | Timur Naumov | Terms: *Indoor Hall* and *Summer Veranda* |
| Definition Description (`<dd>`) | `about.html` | Lines 74, 76 | Timur Naumov | Descriptions of seating and layout for each zone |

---

## 5. Hyperlinks & Media

| Element / Link Type | File | Exact Line Number | Author | Description / Context |
| :--- | :--- | :---: | :--- | :--- |
| External Link (`target`, `rel`) | `about.html`<br>`index.html` | Line 131<br>Line 55 | Timur Naumov<br>Merey Kuatbay | `<a href="https://go.2gis.com/3NTY2" target="_blank" rel="noopener noreferrer">` |
| `mailto:` Link | `about.html`<br>`index.html` | Line 132<br>Line 56 | Timur Naumov<br>Merey Kuatbay | `<a href="mailto:samal@coffeeboom.kz">` |
| `tel:` Link | `about.html`<br>`index.html`<br>`colophon.html` | Line 140<br>Line 56<br>Line 80 | Timur Naumov<br>Merey Kuatbay<br>Timur Naumov | `<a href="tel:+77073130202">` |
| Same-Page Anchor Link 1 | `about.html` | Line 28 | Timur Naumov | `<a href="#branch-zones">Zones</a>` |
| Same-Page Anchor Link 2 | `about.html` | Line 28 | Timur Naumov | `<a href="#branch-capacity">Capacity</a>` |
| Three images with alt | `about.html` | Lines 38, 80, 116 | Timur Naumov | `images/coffee-shop.jpg`, `images/hall.jpeg`, `images/cozy.jpg` |

---

## 6. Typography, Quotes & Phrase Elements

| Element | File | Exact Line Number | Author | Description / Context |
| :--- | :--- | :---: | :--- | :--- |
| `<strong>` | `about.html`<br>`colophon.html` | Lines 50, 56<br>Line 37 | Timur Naumov | Emphasizing key zone labels and brand name |
| `<em>` | `about.html` | Line 127 | Timur Naumov | Emphasizing *hospitable service* quote |
| `<b>` | `about.html` | Lines 73, 75 | Timur Naumov | Bold styling for definition terms |
| `<i>` | `about.html` | Line 34 | Timur Naumov | Italicized technical term *Wi-Fi* |
| `<mark>` | `about.html`<br>`index.html` | Line 127<br>Line 49 | Timur Naumov<br>Merey Kuatbay | Highlighting keywords in quotes |
| `<small>` | `about.html`<br>`feedback.html` | Line 131<br>Line 48 | Timur Naumov | Fine print label for map link and form instructions |
| `<sup>` | `about.html` | Line 67 | Timur Naumov | Superscript temperature unit: `65<sup>&deg;</sup>C` |
| `<abbr title="...">` (1) | `about.html` | Line 34 | Timur Naumov | `<abbr title="Business Center">BC</abbr>` |
| `<abbr title="...">` (2) | `about.html`<br>`colophon.html` | Line 34<br>Lines 40, 73 | Timur Naumov | `<abbr title="Wireless Fidelity">Wi-Fi</abbr>`, HTML5, W3C, CSS |
| `<blockquote>` | `about.html`<br>`index.html` | Line 123<br>Line 45 | Timur Naumov<br>Merey Kuatbay | Real quote from Senior Barista Miras Baitileu (Timur) and customer (Merey) |
| Inline `<q>` | `about.html`<br>`index.html` | Line 127<br>Line 49 | Timur Naumov<br>Merey Kuatbay | Inline quotation |
| `<cite>` | `about.html`<br>`index.html` | Line 126<br>Line 48 | Timur Naumov<br>Merey Kuatbay | Speaker citation: *Miras Baitileu* |
| `<hr>` | `about.html`<br>`colophon.html`<br>`feedback.html` | Line 137<br>Line 68<br>Line 113 | Timur Naumov | Thematic break dividers |
| `<br>` | `about.html`<br>`colophon.html`<br>`feedback.html` | Line 140<br>Line 73<br>Lines 86, 89, 95 | Timur Naumov | Line breaks in contacts and form options |
| `<code>` | `colophon.html` | Line 52 | Timur Naumov | Code block demonstration |
| `<pre>` | `colophon.html` | Line 52 | Timur Naumov | Preformatted code block |
| `<kbd>` | `colophon.html` | Line 47 | Timur Naumov | Keyboard input: `<kbd>Ctrl</kbd> + <kbd>S</kbd>` |
| `<samp>` | `colophon.html` | Line 61 | Timur Naumov | Sample output from W3C syntax validator |
| HTML Entities | `about.html`<br>`index.html` | Lines 28, 67, 126, 140, 141<br>Lines 46, 61 | Timur Naumov<br>Merey Kuatbay | `&copy;`, `&mdash;`, `&bull;`, `&deg;`, `&amp;`, `&trade;` |

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
| `<form>` (`method`, `action`) | `feedback.html`<br>`order.html` | Line 43<br>Line 33 | Timur Naumov<br>Merey Kuatbay | Feedback form (Timur) and pre-order form (Merey) |
| Form Backend Notice Comment | `feedback.html` | Line 44 | Timur Naumov | Comment explaining that backend processing is coming later |
| `<fieldset>` | `feedback.html`<br>`order.html` | Lines 46, 63<br>Lines 36, 53, 101 | Timur Naumov<br>Merey Kuatbay | Form section grouping containers |
| `<legend>` | `feedback.html`<br>`order.html` | Lines 47, 64<br>Lines 37, 54, 102 | Timur Naumov<br>Merey Kuatbay | Grouping captions |
| `<label>` bound to field by `id` | `feedback.html`<br>`order.html` | Lines 50, 54, 58, 66, 70, 74, 85, 88, 91, 95, 101<br>Lines 39, 47, 57, 106 | Timur Naumov<br>Merey Kuatbay | Every single label connected via matching `for` and `id` |
| `type="text"` | `feedback.html`<br>`order.html` | Line 51<br>Line 40 | Timur Naumov<br>Merey Kuatbay | Text inputs for guest name |
| `type="email"` | `feedback.html`<br>`order.html` | Line 55<br>Line 48 | Timur Naumov<br>Merey Kuatbay | Email inputs |
| `type="tel"` | `feedback.html` | Line 59 | Timur Naumov | Phone number input |
| `type="date"` | `feedback.html` | Line 67 | Timur Naumov | Date picker for visit date |
| `type="number"` | `feedback.html` | Line 71 | Timur Naumov | Numeric rating field (1 to 10) |
| `type="radio"` (Radio Group) | `feedback.html` | Lines 84, 87, 90 | Timur Naumov | Purpose of visit selection (`name="purpose"`) |
| `<select>` and `<option>` | `feedback.html` | Lines 75–79 | Timur Naumov | Seating zone dropdown selection |
| `<textarea>` | `feedback.html` | Line 96 | Timur Naumov | Multiline guest feedback text box |
| `type="checkbox"` | `feedback.html` | Line 100 | Timur Naumov | Consent to personal data processing |
| `required` attribute | `feedback.html` | Lines 51, 55, 67, 71, 75, 84, 96, 100 | Timur Naumov | Required constraint validation |
| `placeholder` attribute | `feedback.html` | Lines 51, 55, 59, 71, 96 | Timur Naumov | Input guidance hints |
| `<button type="submit">` | `feedback.html`<br>`order.html` | Line 105<br>Line 129 | Timur Naumov<br>Merey Kuatbay | Form submission trigger buttons |
| `<button type="reset">` | `feedback.html` | Line 106 | Timur Naumov | Form reset button |
