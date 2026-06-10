# Lbby Activation Code Generator

A static web tool for generating Ed25519-signed activation codes (JWTs) for the [Lbby](https://github.com/aindrewkwk/lbby-app) desktop app.

## Usage

1. Go to the site
2. Enter the access password
3. Paste your Ed25519 private key (PEM format)
4. Pick tier, expiry, optional device binding
5. Click **Generate Code**
6. Copy the code and paste it into Lbby → License → Activate

## Security

- All crypto runs **client-side** in your browser (Web Crypto API)
- The private key is **never stored** — it's gone when you close the page
- No analytics, no external requests, no data leaves your browser

## Hosting

Hosted on GitHub Pages. Zero cost, zero servers.

## Development

It's a single `index.html` file — no build step, no dependencies. Open it directly in a browser to test locally.

To change the password gate, edit the `SITE_PASSWORD` variable in the `<script>` section.
