# Little Relay — Waitlist Landing Page

A simple, beautiful waitlist page for [Little Relay](https://little-relay.vercel.app) built with HTML, CSS, and vanilla JavaScript. No dependencies, no build step.

## Getting Started

1. Clone or download this repo
2. Open `index.html` in a browser to preview
3. Connect a form backend (see below)
4. Deploy to GitHub Pages, Vercel, or Netlify

## Connecting Your Form

The form currently logs signups to the console. To collect real emails, replace the `console.log` in `index.html` with one of:

**Formspree (easiest — free tier available)**
```js
fetch('https://formspree.io/f/YOUR_FORM_ID', {
  method: 'POST',
  headers: { 'Content-Type': 'application/json' },
  body: JSON.stringify({ name, email, type })
});
```

**Mailchimp**
Point the form action at your Mailchimp audience signup URL.

**Airtable**
Use the Airtable REST API to log each signup to a base.

## Deploying to GitHub Pages

1. Push this repo to GitHub
2. Go to Settings > Pages
3. Set source to `main` branch, root folder
4. Your page will be live at `https://yourusername.github.io/little-relay-waitlist`

## Brand

- Primary green: `#4d6647`
- Cream: `#FAF6F0`
- Taupe: `#C9B99A`
- Blush: `#EDD9D0`
- Fonts: Cormorant Garamond + DM Sans (via Google Fonts)
