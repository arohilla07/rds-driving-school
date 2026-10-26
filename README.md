# rdsdrivingschool.co.uk static site

This is a static one-page replacement for the WordPress site, built 26 Oct 2026. Upload the whole folder to Cloudflare Pages (or Netlify); there's no build step.

- **Enquiry form:** it posts to Web3Forms. Replace `WEB3FORMS_ACCESS_KEY` in index.html with a free key from https://web3forms.com, which emails enquiries to the address you register. Until the key is set, the form opens WhatsApp with the enquiry pre-filled instead.
- **Phone and WhatsApp:** +44 7548 513489, taken from the old site's chat widget.
- **_headers:** security headers (CSP, HSTS and others). The CSP whitelists the two inline scripts by SHA-256 hash, so recompute the hashes after editing either script, or the page's JS will be blocked.
- **_redirects:** sends the old /contact-rds-driving-school/ URL to #contact.
- **Images:** the logo, hero photo and Pass Plus logo are copied from the old site.
