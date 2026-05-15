# Ninja Cat Co — brand site

Live at https://ninjacatco.com

## What lives here

- `index.html` — the funnel (3-Day Ninja Intro). QR target from the printed insert card.
- `care-guide.html` — printable/bookmarkable full Playbook + troubleshooting.
- `logo.svg` — primary horizontal logo.
- `CNAME` — tells GitHub Pages to serve at `ninjacatco.com`.

## Deploy

Static site, served via GitHub Pages from `main` branch root. Cloudflare handles DNS for `ninjacatco.com`.

## Config inside `index.html` to edit before launch

Near the bottom of the file, three constants:

```js
const MODE = 'gated';          // 'gated' = review-funnel; 'safe' = no gate
const FORM_ENDPOINT = '';      // Formspree (or equivalent) lead capture URL
const AMAZON_REVIEW_URL = 'https://www.amazon.com/review/create-review?asin=YOUR_ASIN';
```

Update `YOUR_ASIN` once the Amazon listing is live, and paste a Formspree URL into `FORM_ENDPOINT` to capture leads.
