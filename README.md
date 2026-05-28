# G&C Fireworks — Website

Family-owned, veteran-led fireworks store in Fayetteville, AR. Operated by G & C Johnson LLC.

This is a single-page static website with photos, hours, locations, and a floating chat-bubble contact form that opens an email to **gandcnwa@gmail.com**.

## Live site

Once GitHub Pages is enabled on this repo, the site is served from `https://<username>.github.io/gcfireworks-site/`.

## File structure

```
index.html              All HTML, CSS, and JavaScript in a single file
assets/
  images/               27 photos: logo, hero, gallery, hero-discount icons, distributor brand marks
README.md               This file
```

## How to update

- **Edit text or layout:** open `index.html` in any text editor. All copy is inline and clearly labeled by section.
- **Replace a photo:** drop the new image into `assets/images/`, then update the matching `src=` reference in `index.html`.
- **Update hours, locations, or phone:** search `index.html` for the current value; it appears in the relevant section.
- **Connect a real backend for the contact chat:** the chat form currently uses a `mailto:` link. To replace with a hosted form, swap the `chatForm` submit handler in `index.html` for a `fetch()` POST to your form provider (Formspree, Netlify Forms, Cloudflare Workers, etc.). Add server-side rate limiting and a honeypot field for spam protection.

## Open items before custom-domain launch

- Replace the placeholder Terms & Conditions and Privacy links in the footer with real policy pages.
- Confirm Arkansas state-law and Fayetteville municipal compliance language with counsel.
- Point the `gcfireworks.com` domain at GitHub Pages once it's released from the previous vendor (DNS CNAME to `<username>.github.io`).

## License

All site copy, photos, and brand assets © G & C Johnson LLC. Site code is for the exclusive use of G&C Fireworks.
