# SEEDS International — Website

Official website for **SEEDS International**, a nonprofit dedicated to providing quality education to impoverished and at-risk youth. Core initiatives include general high school education support, college scholarships (with an emphasis on STEM and medical fields), and essential resources like water filters for at-risk communities — alongside a free, hands-on coding camp for teens and international community partnerships.

## About the project

This is a static, multi-page website with no build step or framework — plain HTML, CSS, and vanilla JavaScript. It can be hosted anywhere that serves static files (GitHub Pages, Netlify, Vercel, S3, etc.).

### Pages

| Page | Description |
|---|---|
| `index.html` | Home — mission overview, three core initiatives, approach, global impact teaser |
| `about.html` | Mission, the three core initiatives, values |
| `programs.html` | Core initiatives (education, scholarships, essential resources) plus the free coding camp's five tracks, mentors, FAQ |
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
