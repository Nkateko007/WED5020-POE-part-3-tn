# TN Real Estate — Website Project

## Project Title
TN Real Estate Website (WEDE5020 POE — Part 3)

## Student Information
- Name & Surname: [Your Full Name]
- Student Number: [Your Student Number]
- Group: [Your Group, if applicable]

## Project Overview
A five-page website for TN Real Estate, a new property and accommodation
service that connects people with homes, rooms, hotels and event venues to
rent or buy. The site lets visitors search and browse listings, make an
enquiry, and gives property owners a way to list their property.

## Website Goals and Objectives
- Let people search for and enquire about properties online.
- Give property owners an easy way to list their properties.
- Make it simple to find homes, rooms, hotels and event venues in one place.
- KPI: number of property enquiries per month.
- KPI: number of properties listed by owners.
- KPI: number of visitors who use the search.

## Key Features and Functionality
- Homepage with a search bar, a photo gallery and category cards.
- About Us page with the company story, mission, vision, FAQ and team.
- Properties page listing houses, apartments, rooms, hotels and event venues,
  with search, a type filter and an A-Z / Z-A sort.
- Enquiry page (replaces the old List Your Property page) with a validated
  form that shows an estimated cost and availability.
- Contact page with an interactive Leaflet map and a native contact form.
- Consistent navigation menu across all five pages.

## Timeline and Milestones
| Milestone | Target |
|---|---|
| Website Project Proposal | Part 1 due date |
| HTML structure (all 5 pages) | Part 1 due date |
| CSS styling and responsive design | Part 2 due date |
| JavaScript functionality and SEO | Part 3 due date |

## Part 1 Details
- The HTML structure for all pages, with a consistent header, navigation and footer.
- Folder structure: root HTML files, with `css/`, `js/`, and `images/` subfolders.

## Part 2 Details
- A single external stylesheet (`css/style.css`) linked from every page, with a
  CSS reset (`*`), base typography and the navy / white / grey colour scheme.
- Navigation built as `nav > ul > li > a`, styled with `nav ul` / `nav ul li a`.
- A reusable `.container` / `.container div` grid pattern used for the category
  cards, listing cards and team cards (3 columns → 2 → 1).
- A `.responsive-image` utility class plus a global `img` rule.
- `:hover`, `:focus` and `:active` states on links, buttons and form fields, and
  `box-shadow` for depth on cards and buttons.
- Two breakpoints: `@media screen and (max-width: 768px)` for tablet and
  `@media screen and (max-width: 480px)` for mobile.
- Responsive images: `srcset`/`sizes` on the homepage photos and listing cards
  (480w/800w/1200w files in `images/responsive/`), and a `<picture>` element
  with art-directed sources for the Properties page banner.

## Part 3 Details
- **Interactive elements:** accordion on the About page (Mission, Vision and FAQ)
  and a fade-in animation when the page loads, in `js/main.js`.
- **Interactive map:** Leaflet + OpenStreetMap map on the Contact page with a
  popup marker for the office (`js/map.js`).
- **Gallery lightbox:** clicking a homepage photo opens it full size; click, press
  Escape or use the X to close (`js/lightbox.js`).
- **Dynamic content and search:** the Properties page builds its cards from a
  JavaScript array, with a search box, a property type filter and an A-Z / Z-A
  sort (`js/properties.js`). The homepage search (`js/home.js`) and the category
  buttons send the visitor to the Properties page with the search already filled in.
- **Enquiry form:** text, email, phone, dropdown, radio buttons, checkboxes, date
  and textarea; JavaScript validation with error messages; shows an estimated
  cost and availability. The listing name is pre-filled when the visitor clicks
  "Enquire" on a listing (`js/enquiry.js`).
- **Contact form:** validated, then compiled into an email that the visitor sends
  with the "Send Email" button to the recipient set in `js/contact.js`.
- **SEO:** keyword-based title tags, meta descriptions and meta keywords on every
  page, one `h1` with ordered `h2`/`h3` headings, descriptive alt text, internal
  links between pages, `robots.txt` and `sitemap.xml`, clean lowercase page URLs.
- **Deployment and security:** to be deployed on a free host that serves the site over HTTPS.

## Sitemap
```
Home (index.html)
├── About Us (about.html)
├── Properties (properties.html)
├── Make an Enquiry (enquiry.html)
└── Contact (contact.html)
```
All pages are on the same level and are reachable from the main
navigation menu on every page.

## Placeholders To Update Before Final Submission
- Name, student number and group at the top of this file.
- Phone number (`011 000 0000`), email (`info@tnrealestate.co.za`) and office
  location (`js/map.js`) on the Contact page.
- Listing names, prices and suburbs in `js/properties.js`, and the estimate
  prices in `js/enquiry.js`.
- `YOUR-SITE-URL` in `robots.txt` and `sitemap.xml`.
- Team roles on the About page (no names or photos were supplied).

## Changelog

### Part 1
- [Date] — Initial HTML structure created for all pages.
- [Date] — Consistent header, navigation, and footer added to every page.

### Part 2
- [Date] — Linked a single external stylesheet (`css/style.css`) from every page.
- [Date] — Applied the navy/white/grey colour scheme and Arial typography from the approved proposal.
- [Date] — Built the `.container`/`.container div` grid, responsive breakpoints at 768px and 480px, and hover/focus/active states.

### Part 3
- 1 November 2026 — Added JSON-driven listings with search and filter (Part 3: dynamic content and search).
- 3 November 2026 — Restructured the site to match the T.C. Carpentry project: 5 pages (Home, About Us, Properties, Make an Enquiry, Contact) instead of 7. Rooms, Hotels & Accommodation and Event Venues are now categories on the Properties page, and List Your Property is now a service option on the enquiry form.
- 3 November 2026 — Rebuilt the stylesheet from the T.C. Carpentry base (same layout rules, mobile Menu button, breakpoints) with the TN navy palette.
- 3 November 2026 — Replaced the listings JSON files and `js/main.js` (which had syntax errors) with `js/properties.js`, using a JavaScript array, search, type filter and A-Z / Z-A sort.
- 3 November 2026 — Replaced the "Photo Coming Soon" placeholders with real photos, resized to 480w/800w/1200w with `srcset`/`sizes`; removed duplicate image files.
- 3 November 2026 — Replaced the Google Form and Google Maps placeholders with a native validated enquiry form and a Leaflet map.
- 3 November 2026 — Rewrote the enquiry and contact scripts using the shared `js/validation.js` helpers (same approach as T.C. Carpentry); contact form now sends through a "Send Email" mailto button instead of the unfinished Formspree endpoint.
- 3 November 2026 — Added the mobile Menu button, page-load fade-in, About page accordion and homepage lightbox.
- 3 November 2026 — SEO: title tags, meta descriptions and keywords on every page; descriptive alt text; `robots.txt` (renamed from `robots.text`) and an updated `sitemap.xml` (removed the non-existent `rentals.html`).

## Photo Credits
All photography used on this site is from Unsplash (free-to-use licence, no
attribution legally required, credited here as good practice). Photographer
names are taken from the original file names:
- Roger Starnes Sr — modern family home
- Johnson — brick family home
- Isaac Quesada — garden apartment block
- Marlene Celine Nordvik — city apartment block
- Clay Banks — bright living room
- Spacejoy — furnished lounge
- Naveen Ketterer — guest house
- Nolann — heritage lodge
- Felix Eka Putra Kuntjoro — event venue building

## References
- MDN Web Docs (n.d.) *MDN Web Docs*. Mozilla. Available at: https://developer.mozilla.org
- Leaflet (n.d.) *Leaflet quick start guide*. Available at: https://leafletjs.com/examples/quick-start/
- OpenStreetMap contributors (n.d.) *Copyright and licence*. Available at: https://www.openstreetmap.org/copyright
- Unsplash (n.d.) *Free photos*. Available at: https://unsplash.com
