# Bio Site

A three-page static personal site (home, skills, contact) in plain HTML and CSS.

## Context

I uploaded this in July 2020, when I had just started learning HTML and CSS. The pages are in `project 1/`. This README replaces a February 2023 one that described a contact form the site doesn't have.

## Stack

- HTML and CSS only
- Font Awesome icons via a kit script

## Running it

Open `project 1/index.html` in a browser. No build step.

## Status

Archived. Kept as a record of where I started.

## Known gaps

- Every page has a malformed tag in the header, `<p<i class=...>` (line 14 on each page).
- The Google Fonts tag is `<link url=...>` (`index.html` line 7, line 6 on the other pages), which browsers ignore, and `style.css` line 4 misspells the font as `'Fondoento'`. The intended fonts never load.
- `skills.html` line 5 has `content="width=, ..."` in the viewport tag. `index.html` closes `</main>` and `</div>` in the wrong order (lines 56-57).
- "Contact us" in the header is a styled `<p>`, not a link. `contact.html` has no form, only text and a screenshot of Google Maps (`map.png`), plus a stray `</i>` (line 26) and a placeholder phone number.
- The service descriptions are lorem ipsum, and the copy has spelling mistakes ("currntly", "thier", "Programing", "Methdologies", "Ioinic").
- `skills.html` lists frameworks, languages and process terms together under "Programing languages".
- Images aren't sized for the web: `myimg.png` is 4.7 MB and shown 100px wide. `myimg.jpeg`, `jax.jpg` and `web.jpg` (about 3.4 MB together) are unused.
- Fixed widths (800px paragraphs, 500px card and map) make the pages overflow on phones.
- The folder name has a space in it, and the icons depend on a personal Font Awesome kit (`kit.fontawesome.com/6da635e2db.js`) that may no longer exist.

## What I'd do differently now

- Run the HTML through a validator; it catches most of the issues above.
- Resize and compress images before committing them.
- Use relative widths and a mobile-first layout.
