# Avirah Health

A "Coming Soon" landing page for Avirah Health.

## Contents

- `index.html` — single-file landing page (HTML/CSS/JS inline, no build step)

## Features

- Responsive gradient hero with animated status indicator
- Email capture form (currently stores submissions in the visitor's browser via `localStorage` — swap in a real backend or mailing-list API before launch)
- Visitor counter powered by [CountAPI](https://countapi.xyz) (free, no signup), with a `localStorage` fallback if the API is unreachable

## Running locally

No build tools or dependencies required. Just open the file directly:

```bash
open index.html   # macOS
xdg-open index.html   # Linux
```

Or serve it with any static file server, e.g.:

```bash
python3 -m http.server 8000
```

then visit `http://localhost:8000`.

## Deploying

Since this is a static file, it can be hosted on any static host (GitHub Pages, Netlify, Vercel, S3, etc.) with no configuration.

## TODO

- Replace the localStorage-based email capture with a real backend or mailing-list integration (e.g. Mailchimp, SendGrid, or a custom API)
- Consider replacing the CountAPI visitor counter with a server-side counter once a backend exists
