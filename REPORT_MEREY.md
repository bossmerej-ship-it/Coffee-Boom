# Reflective Report — Merey Kuatbay

A web page is fundamentally a plain-text document structured with HTML elements, loaded alongside assets like images. When fetched, the browser’s rendering engine parses the raw HTML tokens into a Document Object Model (DOM) tree. It calculates layout geometries, constructs the render tree, and paints the pixels onto the screen viewport. Without external CSS, the engine applies internal user-agent stylesheets to render default typography and margins.

In my codebase, I strictly prioritized semantic tags over generic `<div>` containers:
1. In `menu.html`, I wrapped our pricing data inside a semantic `<table>` with `<thead>` and `<tbody>` instead of styled grid divs, giving assistive technologies explicit tabular data context.
2. In `order.html`, I utilized `<fieldset>` paired with `<legend>` rather than wrapper divs to logically group takeaway preferences, ensuring screen readers announce category contexts.
3. For kitchen notes in `order.html`, I implemented a native `<textarea>` instead of an editable div container to maintain accessible multi-line input handling.

Today, when a visitor clicks the submit button on `order.html`, the browser triggers native client-side validation against attributes like `required` and `type="tel"`. Because no backend server script handles the request, the browser attempts an HTTP GET request, appending field values as URL query parameters and reloading the static page.