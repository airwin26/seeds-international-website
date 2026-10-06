# SEEDS International — Website

Official website for **SEEDS International**, a nonprofit whose main offering is a free, hands-on coding camp for teens. Wherever a camp runs, SEEDS also partners with local organizations to meet real community needs — food, clean water, shelter, and education — as in its July 2026 Cambodia trip with Cultivating Cambodia.

## About the project

This is a static, multi-page website with no build step or framework — plain HTML, CSS, and vanilla JavaScript. It can be hosted anywhere that serves static files (GitHub Pages, Netlify, Vercel, S3, etc.).

### Pages

| Page | Description |
|---|---|
| `index.html` | Home — coding camp spotlight, what we do, how it works, global impact teaser |
| `about.html` | Mission, approach, what we do, values |
| `programs.html` | The coding camp (five tracks, mentors, FAQ) plus the community partnerships that come with each camp |
| `global-impact.html` | Community partnerships in action, featuring the July 2026 Cambodia trip with Cultivating Cambodia |
| `get-involved.html` | Volunteer, donate, and partner pathways + volunteer signup form |
| `contact.html` | Contact form and info |

### Structure

```
├── index.html
├── about.html
├── programs.html
├── global-impact.html
├── get-involved.html
├── contact.html
├── css/style.css
├── js/main.js
└── assets/
    ├── seeds_logo.png
    ├── seeds_banner_wide.jpg
    └── cambodia/       # photos from the July 2026 Cambodia trip
```

## Running locally

No build tools required — just serve the folder:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## Before launch — TODO

The forms on `contact.html` and `get-involved.html` are front-end only (they show a success message but don't send anywhere). Before going live:

- [ ] Connect the contact and volunteer forms to a real backend or form service (e.g. Formspree, Netlify Forms, Google Forms) — search for `data-fake-submit` in the HTML
- [ ] Replace the placeholder email address (`hello@seeds-international.org`) with the real contact email
- [ ] Point the **Donate** buttons at a real donation platform (currently `contact.html`)
- [ ] Add real social media links (currently `#` placeholders in the footer and contact page)
- [ ] Fill in a physical address / phone number if applicable

## Credits

Logo and brand illustration assets carried over from the SEEDS International brand.
