# Web2Table Sticker Studio

Standalone internal utility for creating square restaurant QR + NFC sticker artwork.

## Features
- Restaurant name, optional tagline, and logo upload (PNG/JPG/WebP/SVG, max 5 MB)
- Brand primary and accent colors
- QR generation from a restaurant storefront URL
- SVG and 3000×3000 PNG export
- Responsive layout for desktop and mobile
- Uses Web2Table typography: Inter and Manrope

## Run locally
Open `index.html` in a modern browser. An internet connection is required for Google Fonts and the QRCode.js CDN.

## Deployment notes
This is a static frontend prototype. It does not connect to Web2Table SaaS, Supabase, or customer data. It is **not access-controlled by itself**. Keep this repository private and add access control at the hosting layer before deploying it to a public internet address.

## Production checks still required
- Validate QR scan reliability with different phone cameras and printed samples.
- Verify SVG/PNG exports at intended physical dimensions.
- Bundle dependencies locally for reliable offline generation.
- Add hosting-layer authentication before exposing the tool.
