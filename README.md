# Charter Residential

A polished single-page marketing website for Charter Residential, a GTA-focused property management and modular living company. The site presents two primary service paths: performance-based rental property management and modular garden, laneway, and secondary-suite construction.

## Overview

The website is built as a static HTML page with CDN-hosted frontend libraries. It uses Alpine.js to switch between the home, property management, and modular living views without a build step, and Tailwind CSS for responsive styling.

Key goals of the site:

- Explain Charter Residential's performance-based property management model.
- Promote modular garden suites, laneway conversions, multiplex conversions, and advanced modular homes.
- Showcase service benefits, process steps, testimonials, project imagery, videos, and PDF decks.
- Provide clear calls to action for free property income assessments and consultations.

## Features

- Responsive landing page with sticky navigation and mobile menu.
- Home gateway with separate calls to action for Property Management and Modular Living.
- Property Management view covering:
  - rental profit positioning
  - Charter's performance-based model
  - included services vs owner responsibilities
  - landlord testimonials
  - embedded strategy deck
- Modular Living view covering:
  - video-backed hero section
  - garden suites, laneway suites, multiplexes, and modular homes
  - tax rebate guidance link
  - service offering matrix
  - embedded modular and garden-suite PDF decks
  - project gallery and testimonials
- Shared assessment CTA and footer contact section.

## Tech Stack

- HTML5
- Tailwind CSS via CDN
- Alpine.js via CDN
- Lucide Icons via CDN
- Google Fonts, using Poppins
- Static images, PDFs, and MP4 video assets

Because the project is static, no package manager, bundler, or backend server is required.

## Project Structure

```text
.
├── assets
│   ├── docs
│   │   ├── garden-suites-presentation.pdf
│   │   └── modular-housing-framework.pdf
│   ├── images
│   │   ├── garden-suite-exterior.png
│   │   ├── laneway-suite-concept.png
│   │   └── modular-sip-home.png
│   └── videos
│       └── modular-living-hero.mp4
├── index.html
└── README.md
```

## Local Preview

Open `index.html` directly in a browser, or serve the folder with any static file server.

Example using Python:

```bash
python3 -m http.server 8000
```

Then visit:

```text
http://localhost:8000
```

Using a local server is recommended so local PDFs, images, and video behave the same way they will after deployment.

## Deployment

This project can be deployed to any static hosting provider, including:

- GitHub Pages
- Netlify
- Vercel
- Cloudflare Pages
- any standard web host that serves static files

For GitHub Pages, publish the `main` branch from the repository root because `index.html` is already at the top level.

## Asset Notes

- `assets/videos/modular-living-hero.mp4` powers the Modular Living hero background video.
- `assets/images/garden-suite-exterior.png`, `assets/images/laneway-suite-concept.png`, and `assets/images/modular-sip-home.png` are used in the modular product cards.
- `assets/docs/garden-suites-presentation.pdf` is embedded in the Garden Suites section.
- `assets/docs/modular-housing-framework.pdf` is embedded in the Modular Framework section.
- The Property Management deck is embedded from Google Drive.

## Contact Information Displayed

- Phone: `+1 437-974-2863`
- Email: `hello@charterresidential.com`
- Location: Toronto, Ontario, Greater Toronto Area

## Maintenance Notes

- Update company copy, phone number, email, and service claims directly in `index.html`.
- Keep asset filenames unchanged unless the matching `src` references in `index.html` are updated.
- If external CDN links are removed, replace Tailwind CSS, Alpine.js, Lucide Icons, and Google Fonts with local or bundled equivalents.
- Review tax and rebate language periodically because government incentives and eligibility rules can change.
