# My website

This folder **is** the website. Every file in it gets published exactly as it is.
There is nothing to install, nothing to compile, and no command to run.

Live at: `https://basmatierajcoomar-pixel.github.io`

---

## The three pages that hold it together

| File | What it is |
|---|---|
| `index.html` | The home page: the headline, the stats, the six featured items |
| `library.html` | The full searchable list of everything |
| `about.html` | The about page |
| `site.css` | The look of those three pages. Change a colour here and all three change. |

Everything else is a project. Each project is one self-contained `.html` file
named after its web address: `skill-forge.html` is live at
`https://basmatierajcoomar-pixel.github.io/skill-forge.html`.

---

## Adding a new project

**Step 1.** Rename your file to lowercase with hyphens instead of spaces.
`My New Thing.html` becomes `my-new-thing.html`. This becomes its web address,
so keep it short.

**Step 2.** Go to your repository on github.com. Click **Add file**, then
**Upload files**. Drag the file onto the page. Scroll down, click
**Commit changes**.

**Step 3.** Wait about a minute, then open
`https://basmatierajcoomar-pixel.github.io/my-new-thing.html`. It is live.

At this point the project works but is not *listed* anywhere. To get it onto the
home page and the library, ask Claude: *"add my-new-thing.html to my site's
index and library."* Claude regenerates `index.html` and `library.html` and
hands them back; you upload those two the same way, and GitHub replaces the old
versions automatically.

## Replacing a file

Upload a file with the same name. GitHub overwrites it. Same one-minute wait.

## Deleting a project

On github.com, click the file, then the trash icon at the top right of the file
view, then **Commit changes**. Ask Claude to regenerate the two index pages
afterwards so it stops being listed.

---

## Things that will save you a support call

- **Nothing appears / an old version appears.** Wait a minute, then reload with
  the cache bypassed: `Cmd + Shift + R`. GitHub takes 30 to 60 seconds to
  publish, and browsers hold onto old copies.
- **Never put a space in a filename.** Spaces turn into `%20` in the address
  and links break. Hyphens only.
- **Never rename `index.html`.** That file *is* the home page.
- **Don't delete `.nojekyll` or `sw.js`.** `.nojekyll` stops GitHub from trying
  to reinterpret your HTML. `sw.js` is what lets the installable apps be added
  to a phone home screen.
- **Everything here is public.** Anyone with the address can read it, and search
  engines will index it. Do not upload anything with marks, personal
  information, or graded work you have not submitted yet.

---

## What this site is built on

Plain HTML and CSS, served by GitHub Pages. No framework, no build step, no
monthly cost. The only outside dependency is the Inter typeface loaded from a
public CDN; if that ever fails, the site falls back to a system font and keeps
working.
