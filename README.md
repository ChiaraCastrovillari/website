# Personal website — Chiara Castrovillari

A minimal, single-page academic website built with plain HTML/CSS (no build step),
ready to publish with GitHub Pages.

## Structure

```
index.html                        the whole page
styles.css                        all styling
assets/profile-placeholder.svg    placeholder photo (swap for a real one)
cv/CV_Chiara_Castrovillari.pdf    put your CV here — the "here" link in the
                                   About section already points to this path
```

## What still needs filling in

Everything highlighted in **yellow** on the page (class `edit-me` in the HTML)
is a placeholder — search `index.html` for `edit-me` / `[...]` and replace with
your own text, then delete the `edit-me` class so the highlight goes away.

Specifically:
- The two research-field blanks and one-line pre-doc summary in the intro paragraph.
- The three "Selected Works In Progress" entries (titles, coauthors, status/links, descriptions).
- The two "Pre-Doctoral Research" entries (advisor/institution, dates, description).
- Duplicate a `<article class="work-entry">…</article>` block in either section to add more entries.

## Adding your photo

Replace `assets/profile-placeholder.svg` with your own image, e.g. `assets/profile.jpg`,
and update the `src` on the `<img class="profile-photo">` tag in `index.html` accordingly.

## Adding your CV

Drop your CV PDF into the `cv/` folder as `CV_Chiara_Castrovillari.pdf` (or update the
link in `index.html` if you name it differently).

## Preview locally

Just open `index.html` in a browser — no server or build tools required.

## Publish with GitHub Pages

1. Create a new repository on GitHub (e.g. `chiara-castrovillari.github.io` for a
   `username.github.io` site, or any name for a project site).
2. From this folder:
   ```
   git remote add origin <your-repo-url>
   git branch -M main
   git push -u origin main
   ```
3. On GitHub: **Settings → Pages → Source → Deploy from branch → main / (root)**.
4. Your site will be live at `https://<username>.github.io/` (or
   `https://<username>.github.io/<repo-name>/` for a project repo) within a minute or two.
