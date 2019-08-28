# Semantic HTML

# Content Models
* Metadata content
* Flow content
* Sectioning content
* Heading content
* Phrasing content
* Embedded content
* Interactive content

## Sectioning Content, the semantic elements
A snapshot of selected semantic elements should be ordered in a hierarchy:

* `<header>`
  - `<nav>`
  - `<menu>`
    - `<menuitem>`
* `<main>` - only one of me can exist in an HTML document!
  - `<aside>` - used for sidebars
    - `<header>`
  - `<section>`
    - `<aside>` - ...or side information
    - `<article>`
      - heading: `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>`
      - `<details>`
        - `<summary>`
      - `<figure>`
        - `<figcaption>`
      - `<mark>`
      - `<time>`
* `<footer>`

---

## Sources
* [WHATWG - HTML - Content Models](https://html.spec.whatwg.org/multipage/dom.html#kinds-of-content)
