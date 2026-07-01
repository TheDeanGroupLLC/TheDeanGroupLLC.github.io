# The Dean Group Static Website

This is a five-page static HTML/CSS/JS implementation based on the supplied website content and brand guide.

## Pages

- `index.html` — Home
- `about.html` — About
- `services.html` — Services
- `past-performance.html` — Past Performance
- `contact.html` — Contact

## Asset filenames expected

Place the supplied PNG files in `assets/logos/` with exactly these names:

- `TheDeanGroup_Logo_Vertical_Pinyon.png` — primary logo; used in the Home hero as the imported wordmark PNG.
- `TheDeanGroup_Logo_Horizontal_Pinyon.png` — horizontal wordmark; used in the header and footer on every page.
- `TheDeanGroup_TDG_Badge_MD.png` — secondary mark; used in the footer on every page.
- `TheDeanGroup_Website_Header.png` — website header reference; reserved for future hero/header imagery if the client wants the header reference used visually.

Note: the uploaded manual text lists `TheDeanGroup_LinkedInBanner_Cream.png` as the website header reference, while the email note says `TheDeanGroup_Website_Header.png`. This project follows the newer email note filename. If the actual delivered file is named `TheDeanGroup_LinkedInBanner_Cream.png`, either rename it to `TheDeanGroup_Website_Header.png` or update the reference in this README.

## Verification against content guide

### Global

- Five separate pages are present.
- Navigation is clean and flat: Home, About, Services, Past Performance, Contact.
- No dropdowns or subpages are used.
- CSS is separated into `css/styles.css`.
- JS is separated into `js/main.js`.
- Base background is cream `#F5F2EE`.
- Navy `#1B3A6B`, teal `#2A7B73`, gold `#C49A2A`, and cream `#F5F2EE` are defined as CSS variables.
- PNG logo references are used; no text-created logo is used.
- Mobile hamburger navigation is included.

### Home

- Hero includes the imported vertical wordmark PNG, headline, subheadline, and two buttons. The wordmark is not recreated as text and is not placed in a separate side card.
- The Gap We Fill three-column section is included with the required copy.
- Six service snapshot tiles are included with the required copy.
- Full navy Origin Statement is included.
- Credentials bar is included.
- Footer appears on the page.

### About

- Page headline and subheadline are included.
- Full origin story is included.
- Principal section is included.
- Advisory Board section with Luis Rodriguez and Veronica Rodriguez is included.
- Program Expertise tags are included.

### Services

- Page headline and subheadline are included.
- Seven service lines are included.
- Pricing notes for Practical AI and Office Hours/Retainer are included.
- How to Engage three-step process is included.

### Past Performance

- Page headline and subheadline are included.
- Past performance cards are included.
- NAICS codes and registrations are included.

### Contact

- Page headline and subheadline are included.
- Three contact options are included.
- Contact form fields match the spec.
- Direct contact and subcontracting note are included.
- Calendly placeholders are included for later replacement.

## Before launch

1. Add the real PNG logo files to `assets/logos/`.
2. Replace Calendly placeholder blocks/links in `contact.html`.
3. Connect the contact form to a form handler such as Formspree, Netlify Forms, or backend email service.
4. Test all five pages on phone width and on desktop.
5. Run a link check and verify logo paths load correctly.
