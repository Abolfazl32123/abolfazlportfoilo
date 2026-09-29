# Abolfazl Rajabi Portfolio — V27 Speed Optimized

Cloudflare Workers portfolio with local static assets.

Speed optimizations in this version:
- Large logo PNG optimized from 1254px / ~3.5MB to 512px WebP (~54KB).
- Mr Mobile project image optimized to 1000px WebP (~36KB).
- Below-the-fold images use lazy loading and async decoding.
- OpenStreetMap iframe is deferred until the contact map approaches the viewport.
- Below-the-fold sections use content-visibility to reduce initial rendering work.
- Google Fonts stylesheet is loaded from the document head with preconnect instead of CSS @import.
- Corrected the stale hero/footer phone link to 0991-848-3441.
- Added favicon based on the portfolio logo.

Deploy with Wrangler as before:

npm run deploy
