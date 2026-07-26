# N&D Fence and Deck - static site

Plain HTML + CSS, one tiny inline script for the mobile nav. No build step, no framework.

## Deploy to Cloudflare Pages

Option A, drag and drop:
1. Cloudflare dashboard -> Workers & Pages -> Create -> Pages -> Upload assets
2. Drag this folder in. Done.

Option B, git:
1. Push this folder to a repo
2. Pages -> Connect to Git, framework preset "None", build command empty, output directory `/`

## Contact form (free)

The form posts to Web3Forms, which is free for a basic contact form and needs no backend:
1. Go to https://web3forms.com, enter the email that should receive leads
2. They email you an access key
3. In `index.html`, replace `YOUR_WEB3FORMS_ACCESS_KEY` with it

Formspree works the same way if you prefer it (free tier is 50 submissions/month).

## Things to swap before launch

- Logo: drop `logo.png` (or .svg, just update the src) into `/images`. It shows in the header automatically; if the file is missing the text brand displays instead
- Service area text (currently "Greater Puget Sound area")
- Hero: swap the placeholder band for a real project photo (comment in the HTML shows how)
- Gallery: drop photos into `/images` and replace each placeholder div with an `<img>` tag
- Hours, warranty terms, license line in the footer
# ndfencedeck
