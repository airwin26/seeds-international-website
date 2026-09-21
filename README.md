# SEEDS International — Website

Official website for **SEEDS International**, a nonprofit that runs a free, hands-on coding camp for teenagers and partners with local organizations on community projects around the world.

## About the project

This is a static, multi-page website with no build step or framework — plain HTML, CSS, and vanilla JavaScript. It can be hosted anywhere that serves static files (GitHub Pages, Netlify, Vercel, S3, etc.).

### Pages

| Page | Description |
|---|---|
| `index.html` | Home — mission overview, program highlights, how camp works, global impact teaser |
| `about.html` | Mission, approach, and values |
| `programs.html` | The five camp tracks (software development, cybersecurity, data analytics, web development, UX design), a day at camp, mentors, FAQ |
| `global-impact.html` | Community partnerships, featuring the July 2026 Cambodia trip |
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
    └── seeds_banner_wide.jpg
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
- [ ] Swap in real photos from camp and the Cambodia trip where illustrations are used
- [ ] Fill in a physical address / phone number if applicable

## Credits

Logo and brand illustration assets carried over from the SEEDS International brand.
