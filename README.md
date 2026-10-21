# Pelle Pico, personal website

Live at [pelle-pico.online](https://pelle-pico.online).

My personal site and CV. I'm a data science student at Copenhagen Business School (MSc Data Science &
Business Administration, 2026–2028) with a BSc in Global Business Informatics from the IT University of
Copenhagen. I work with Python, SQL, SAS, Power BI and Tableau, and I'm currently learning machine learning.

## What's on the site

- A halftone dot portrait drawn on a `<canvas>`. The eyes follow the cursor, using the eye region of the
  real photo.
- A word-of-the-day game at the top, with a new five-letter word each day. Guesses are checked against a
  list of real English words.
- A "Looking for someone who can…" picker that shows where I've done each kind of work.
- A timeline of jobs and degrees.
- A ⌘K command palette for keyboard navigation.
- A Copenhagen clock, an email menu (Gmail, Outlook, mail app or copy), and a tab icon that switches
  between light and dark with the visitor's time of day.

## How it's built

Everything is in `index.html`: plain HTML, CSS and JavaScript, with no framework, build step or
dependencies. Animations respect `prefers-reduced-motion`. It's hosted on Vercel, which redeploys on
every push to `main`.

## Running it locally

```sh
git clone https://github.com/PellePico/pelle-website.git
cd pelle-website
python3 -m http.server 3000
```

Then open http://localhost:3000.

## Files

| File | What it is |
|---|---|
| `index.html` | The whole site |
| `pelle.jpg` | Photo used for the dot portrait |
| `words.txt` | Allowed guesses for the word game (from [dwyl/english-words](https://github.com/dwyl/english-words), public domain) |
| `Pelle_Pico_CV_english_2026_online.pdf` | My CV |
| `favicon-*`, `apple-touch-icon.png` | Day and night tab icons |
