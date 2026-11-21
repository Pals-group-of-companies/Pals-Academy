# Pals Academy website

Static website for Pals Academy, a kindergarten in Waithaka, Nairobi (Baby Class, PP1, PP2).

## Pages
- Home `/`, About `/about`, Contact `/contact`, Privacy `/privacy`, Terms `/terms`, Cookies `/cookies`.
- Each page is a folder with its own `index.html`. The old `about.html` and `contact.html` addresses redirect to the new ones.

All images are in `assets/`. No build step is needed: open `index.html` in a browser, or serve the folder with any static host (GitHub Pages, Netlify, cPanel).

## How things work
- Fonts are stored in `assets/fonts` (Outfit and a handwriting font, both under the SIL Open Font License). Nothing loads from Google or any other outside service when a page opens, so no cookie banner is needed.
- The contact form sends enquiries to enroll@palsacademy.co.ke through FormSubmit (formsubmit.co). The first time someone sends the form, FormSubmit emails that inbox an activation link that must be clicked once; enquiries arrive after that.
- `sitemap.xml`, `robots.txt` and `llms.txt` are for search engines and AI assistants. Update them when pages change.
- `404.html` is shown for addresses that don't exist.
