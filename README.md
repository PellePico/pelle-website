# Pelle Pico — personal website

**Live:** [pelle-pico.online](https://pelle-pico.online)

My personal site and CV. I'm a data science student at Copenhagen Business School
(MSc Data Science & Business Administration, 2026–2028) with a BSc in Global Business
Informatics from the IT University of Copenhagen. I work with Python, SQL, SAS,
Power BI and Tableau, and I'm currently learning machine learning and AI tooling.

## What's on the site

- **Dot portrait that looks back at you.** My photo is redrawn as a halftone grid of dots
  on a `<canvas>`. The eyes follow your cursor by re-sampling the eye region of the real photo,
  so they stay mine and don't look drawn in.
- **Word of the day.** A small Wordle-style game at the top. A new five-letter word each day,
  and every word says something about me once you solve it. Guesses are checked against a
  list of real English words.
- **"Looking for someone who can…"** Pick what your team needs, and the site shows where
  I've already done it (dashboards, automation, SQL, …).
- **Timeline** of jobs and degrees.
- **⌘K command palette** to jump around the page from the keyboard.
- **Small details:** a Copenhagen clock that guesses what I'm doing right now, an email menu
  (Gmail, Outlook, mail app or copy), and a tab icon that switches between light and dark
  with the visitor's local time of day.

## How it's built

- One file, `index.html`: plain HTML, CSS and JavaScript. No framework, no build step,
  no dependencies.
- Animations respect `prefers-reduced-motion`.
- Hosted on Vercel, which redeploys automatically on every push to `main`.
- Built with Claude Code as a coding partner: I set the direction and design decisions,
  and reviewed every change.

## Run it locally

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

## Contact

The best way to reach me is through the email button on the site.
