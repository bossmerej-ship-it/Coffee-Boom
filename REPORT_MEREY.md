# Web Development Project Report: Coffee Boom (Samal 12 Branch)
**Author:** Merey Kuatbay  
**Course:** Web Technologies / Frontend Fundamentals  

---

## 1. Architectural Analysis of Reference Website (Site Audit)
For our structural baseline, we analyzed the commercial web presence of **Coffee Boom Kazakhstan** (`coffeeboom.kz`).

### Structural Limitations of the Reference Website:
* **Presentation Wrap Overload (Div Soup):** The production website relies heavily on dynamic CMS page builders. Content blocks, menus, and banners are encapsulated within layers of nested `<div>` wrappers without semantic purpose, obscuring the logical outline of the document.
* **Semantic & Accessibility Gaps:** Key landmark elements such as `<main>`, structured `<article>`, and explicit form `<label>` associations are frequently omitted or replaced by proprietary script-based elements, impeding assistive screen readers.
* **Asset Overhead:** Displaying simple branch information and static beverage prices triggers extensive third-party scripts and animation bundles, creating unnecessary network overhead.

### Architectural Solution for Our Implementation:
* **Native Landmark Tree:** We rebuilt the core branch architecture using native HTML5 elements (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<footer>`), delivering an instant document outline.
* **Form Usability:** The pre-order interface utilizes semantic grouping (`<fieldset>`, `<legend>`), explicit field binding, and native input constraints (`tel`, `time`, `email`).
* **Zero Script Overhead:** Dynamic menus are represented as accessible HTML tabular data (`<table>`, `<caption>`, `<thead>`, `<tbody>`), ensuring full W3C validation compliance and near-instant load performance.

---

## 2. Reflective Essay — Merey Kuatbay
During this project, my primary development scope encompassed establishing the root document structure (`index.html`), implementing the comprehensive product pricing catalog (`menu.html`), and engineering the takeaway pre-order system (`order.html`).

Architecting `menu.html` required a structured approach to data hierarchy. Instead of treating pricing information as unstructured text, I constructed a semantically accessible table utilizing `<caption>`, `<thead>`, `<tbody>`, and column/row-scoped headers (`<th scope="col">`, `<th scope="row">`). During validation, the W3C Nu HTML Validator flagged the legacy presentation attribute `border="1"` as obsolete in HTML5. Eliminating this attribute and adhering strictly to semantic markup resolved the issue, returning zero errors.

In `order.html`, my objective was maintaining clear visual hierarchy without CSS styling. Grouping customer data and beverage configurations into separate `<fieldset>` elements provided logical separation. I employed `<optgroup>` within `<select>` elements to categorize coffee beans and brew styles, and utilized a native `<textarea>` for kitchen instructions to support multiline feedback.

Collaborating through Git surfaced valuable real-world challenges. When pulling upstream commits containing my partner's review components, branch divergence triggered an interactive Vim merge prompt (`MERGE_MSG`). Resolving merge sequences via terminal commands (`:wq` and `--no-edit`), alongside resetting branch pointers after accidental folder nesting, provided deep practical experience in production-level Git synchronization and version control.