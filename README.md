# Personal website — Chiara Castrovillari

A minimal, single-page academic website built with plain HTML/CSS (no build step).
Live at: **https://chiaracastrovillari.github.io/website/** (once GitHub Pages is
enabled in the repo's Settings → Pages, branch `main` / root).

## Structure

```
index.html            the whole page
styles.css             all styling
assets/profile.jpg     profile photo (circular, shown above the bio)
cv/CV_Chiara_Castrovillari.pdf   CV — the "here" link in the About section
                                  points to this path
```

## Updating content

- **Bio**: edit the `.intro` paragraph inside `<section id="about">` in `index.html`.
- **Works in progress / Pre-Doctoral Research**: each entry is an
  `<article class="work-entry">` block with a title, a meta line (status/coauthors),
  and a description. Duplicate a block to add more, or edit text in place.
- **Photo**: replace `assets/profile.jpg` with a new image of the same name (or update
  the `src` on `<img class="profile-photo">` in `index.html` if renaming it). It's
  rendered as a circle via CSS (`border-radius: 50%`), so a roughly square, centered
  headshot works best.
- **CV**: overwrite `cv/CV_Chiara_Castrovillari.pdf` with a new version, same filename.

## Preview locally

Just open `index.html` in a browser — no server or build tools required.

## Publishing changes

This folder is linked to GitHub Desktop and tracks
`https://github.com/ChiaraCastrovillari/website`. After editing, commit and push
(via GitHub Desktop, or `git add -A && git commit -m "..." && git push` from this
folder) and the live site updates within a minute or two of Pages rebuilding.
