# Shane Salon – Westwood, Los Angeles

Production-ready website for **Shane Salon**, built from the same structure and layout as Beauty by Anderson, with Shane Salon branding, dark navy + white theme, and updated content.

## Quick start

Open `index.html` in a browser or serve the folder with any static server:

```bash
# Python
python3 -m http.server 8000

# Node (npx)
npx serve .
```

Then visit `http://localhost:8000`.

## Brand & contact

- **Business:** Shane Salon  
- **Phone:** (310) 208-1226 — `tel:+13102081226`  
- **Address:** 1080 Glendon Ave, Los Angeles, CA 90024  
- **Google Maps:** [Shane Salon](https://www.google.com/maps/place/Shane+Salon/@34.0609201,-118.4442388,17z)  
- **Directions:** [Get Directions](https://www.google.com/maps/dir//1080+Glendon+Ave,+Los+Angeles,+CA+90024)

## Pages

| Page        | File         | Notes                                                |
|------------|--------------|------------------------------------------------------|
| Home       | `index.html` | Hero, Why Choose, Services, Reviews preview, Details, Visit Us |
| Services   | `services.html` | Haircut, Color & highlights, Blowouts              |
| Reviews    | `reviews.html`  | 10 Google reviews + “See all on Google” link       |
| About Us   | `about.html`    | Story, philosophy, full Details & amenities       |
| Our Team   | `team.html`     | Shane + placeholder for more stylists             |
| Book       | `book.html`     | Call Now, Get Directions, Text, request form       |

## Design

- **Colors:** Primary `#0B1F3B`, white `#FFFFFF`, light sections `#F5F7FB`, optional accent `#C7A35A`.
- **Fonts:** Playfair Display (headings), Poppins (body), loaded from Google Fonts.
- **CTAs:** Call Now (`tel:+13102081226`), Book (form), Get Directions (Google Maps).

## Forms (Netlify)

The booking form uses Netlify Forms (`name="appointment"`). To receive submissions:

1. Deploy the site to Netlify.
2. In Netlify Dashboard → Site → Forms, find the **appointment** form.
3. Configure email notifications for new submissions.

A hidden duplicate form exists on `index.html` so Netlify can detect the form even when users land on the homepage first.

## Favicon

The site uses an inline SVG favicon (“S” in navy). To use your own:

- Add `favicon.ico`, `favicon/favicon-32x32.png`, `favicon/favicon-16x16.png`, and `favicon/apple-touch-icon.png`.
- For PWA: add `favicon/android-chrome-192x192.png` and `favicon/android-chrome-512x512.png` (referenced in `favicon/site.webmanifest`).

## SEO & accessibility

- LocalBusiness schema on the homepage (name, address, phone, rating, Google link).
- Meta title/description and Open Graph on all pages.
- Skip link, focus styles, semantic headings, and alt text where needed.
- Mobile-first layout with sticky header and bottom CTAs (Call, Book, Directions, Text) on small screens.

## File overview

```
shane's-salon/
├── index.html
├── about.html
├── services.html
├── reviews.html
├── team.html
├── book.html
├── styles.css
├── accessibility.css
├── transitions.js
├── favicon/
│   └── site.webmanifest
├── .gitignore
└── README.md
```

Images (hero, services) use Unsplash URLs. Replace with your own assets when ready. Add `images/og-shane-salon.png` for social sharing if desired.
