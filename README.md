# The portfolio site

This folder **is** the website. Every file in it is published exactly as it is.
There is nothing to install and no command to run.

Live at: `https://basmatierajcoomar-pixel.github.io`

---

## What is in here

| File | What it is |
|---|---|
| `index.html` | Home: the headline, three lifted figures, the corpus figure, selected work |
| `research.html` | Independent research and writing |
| `coursework.html` | Everything grouped by course, with a coverage table |
| `afm291.html` | The AFM 291 vault hub |
| `tools.html` | The six interactive tools |
| `library.html` | Every piece, split into independent, personal and coursework |
| `about.html` | About and contact |
| `colophon.html` | How the site is built and how every number on it is measured |
| `site.css` | The look of all of the above. One file. |
| `site.js` | Theme toggle, search palette, library filters, the age in the first sentence |

Everything else is a piece: one self-contained `.html` file named after its web
address. `skill-forge.html` is live at `/skill-forge.html`. The `-fig1.png` files
are diagrams pulled out of the Word documents during conversion; each one belongs
to the page whose name it starts with.

---

## Adding a new piece

**Step 1.** Rename the file to lowercase with hyphens instead of spaces.
`My New Thing.html` becomes `my-new-thing.html`. That becomes its web address.

**Step 2.** On github.com, open this repository. Click **Add file**, then
**Upload files**. Drag the file in. Scroll down, click **Commit changes**.

**Step 3.** Wait about a minute, then open `/my-new-thing.html`. It is live.

It works immediately but is not *listed* anywhere yet. To get it onto the home
page and into the library, ask Claude: *"add my-new-thing.html to my site's index
and library."* The index pages are generated from measurements taken from the
files themselves, so they have to be regenerated rather than hand-edited.

## Adding a note or a Word document

Twenty-two pages here started as markdown notes or Word files and are converted at
build time. To add another, send Claude the `.md` or `.docx` and say which section
it belongs in. Do not paste the content into an HTML file by hand: the converters
handle the callouts, the checkpoint questions, the internal note links, the tables
and the embedded diagrams, and doing it manually loses all of them.

## Replacing or deleting

Upload a file with the same name to replace it. To delete, open the file on
github.com, click the trash icon, then **Commit changes**. Ask Claude to
regenerate the index pages afterwards so it stops being listed.

---

## Things that will save you a support call

- **Nothing appears, or an old version appears.** Wait a minute, then reload with
  `Cmd + Shift + R`. GitHub takes 30 to 60 seconds to publish and browsers hold
  onto old copies.
- **Never put a space in a filename.** Spaces become `%20` and links break.
- **Never rename `index.html`.** That file *is* the home page.
- **Do not delete `.nojekyll`, `site.css`, `site.js` or `sw.js`.**
- **Everything here is public** and search engines will index it. Do not upload
  anything carrying marks, personal information, or graded work you have not
  submitted yet.

---

## How it is built

Plain HTML, CSS and JavaScript, served as static files by GitHub Pages. No
framework, no build step on the reader's side, no tracking and no cookies. Figures
are static SVG, so they render with JavaScript turned off. Full detail, including
the exact definition behind every number on the site, is on `colophon.html`.
