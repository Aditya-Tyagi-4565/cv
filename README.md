# Single-Page CV

A single-page Curriculum Vitae built with **semantic HTML only** (no CSS or JavaScript). This project focuses on structuring content correctly — headings, sections, articles, lists, and metadata — so it's ready for a styling pass in a future project.

Project brief: [roadmap.sh/projects/single-page-cv](https://roadmap.sh/projects/single-page-cv)

## Project Structure

```
.
├── cv.html        # The CV page (semantic HTML, SEO + OG tags, favicon link)
├── favicon.ico    # (add your own — see "Favicon" below)
└── README.md      # This file
```

## Features

- **Semantic HTML** — `<header>`, `<main>`, `<section>`, `<article>`, `<address>`, `<time>`, and `<footer>` used according to their intended purpose.
- **SEO meta tags** — description, keywords, author, and robots tags in the `<head>`.
- **Open Graph tags** — for clean previews when shared on social media / messaging apps.
- **Favicon link** — ready to point at an icon file.

## How to Run It

No build tools, servers, or dependencies are required — it's a single static HTML file.

### Option 1: Open directly in a browser
1. Locate `cv.html` on your computer.
2. Double-click it, or right-click → **Open with** → your browser of choice.

### Option 2: Run a local server (optional)
Useful if you want URLs/paths to behave like they would on a real website.

**Using Python (built-in on most systems):**
```bash
# Navigate to the project folder first
cd path/to/project

# Python 3
python3 -m http.server 8000
```
Then open `http://localhost:8000/cv.html` in your browser.

**Using Node.js:**
```bash
npx serve .
```
Then open the URL it prints in your terminal.

## Customizing the Content

All content in `cv.html` is placeholder (name: *Jordan Ellis*). To make it yours:

1. Replace the name, job title, and contact details in `<header>`.
2. Update the `<section id="summary">` paragraph.
3. Edit or add `<article>` entries inside `#experience` and `#education` with your own roles/dates.
4. Update the skill lists inside `#skills`.
5. Adjust or remove `#certifications` as needed.
6. Update the `<meta name="description">`, `<meta name="keywords">`, and all `og:*` tags in the `<head>` to match your real info and hosted URL.

## Favicon

The page links to `favicon.ico` in the same folder:
```html
<link rel="icon" type="image/x-icon" href="favicon.ico">
```
Add your own `favicon.ico` (or update the `href` to point to a different icon file/path) so it displays correctly.

## Next Steps

This project intentionally has **no CSS**. Styling (layout, colors, typography, print styles, etc.) is planned for a follow-up project.
