# DSM · UC Irvine

Website for the Distributed Systems Middleware Group at the University of California, Irvine.

Live site: https://lyq12345.github.io/dsm-lab/

## Editing

This is a build-free static website. Edit `index.html`, `projects.html`, `members.html`, or `publications.html` directly. Shared styles and scripts live in `assets/`.

Add publications to `publications/bibliography.bib` and put local paper PDFs under `publications/papers/`. The publication page reads the bibliography dynamically. Selected publications on the home page are curated separately in `index.html`.

Navigation and footer HTML is shared by convention and repeated in all four main pages.

## Local preview

```sh
python3 -m http.server 8765 --bind 127.0.0.1
```

Open http://127.0.0.1:8765/. Use an HTTP server so the bibliography can load.

## Deployment

GitHub Pages publishes the root of the `main` branch. Push commits to `main` to update the website. `.nojekyll` keeps the HTML and assets unchanged during publication.

The repository contains the main website and the assets it uses. Historical project pages remain linked to their original UCI URLs. Course archives, unrelated server files, and local backups are outside this repository.

The site uses the existing bibliography renderer and its locally stored jQuery and Moment dependencies. Their original license notices remain in the distributed files. Research publications and photos retain their original ownership.
