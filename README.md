# Minari — QR landing page

Static, mobile-first page that customers reach by scanning the QR code on the Minari menu.
It links to Instagram, Facebook and YouTube, and offers call, directions, save-contact, banquet enquiry and home delivery.

- `index.html`: the whole page (inline CSS, no build step)
- `assets/`: logo, favicon, share image
- `minari.vcf`: "Save contact" card

## Hosting
GitHub Pages serves `main` / root at https://nnalin04.github.io/minari/

### Moving to your own domain later
1. Buy a domain (e.g. `minari.in`) and add DNS records:
   - apex: `A` records → 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
   - or a subdomain: `CNAME www` → `nnalin04.github.io`
2. Repo → Settings → Pages → Custom domain → enter the domain, then tick "Enforce HTTPS".
3. Point the printed QR code at the new domain.

Any other static host (Netlify, Cloudflare Pages, Vercel, or a plain nginx server on your own IP) works too: upload these files as they are.
