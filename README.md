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

- Service area text (currently "Greater Puget Sound area")
- Hours, warranty terms, license line in the footer

## Photos

The hero is `images/cedar_fence_rebuild_main.jpg`; the gallery uses the other five
project photos. To add a gallery tile, copy a `<figure>` block in the Gallery section
and point it at a new file in `/images`.

Two CSS crop helpers are available on gallery images, for tall phone photos where a
centre crop would land on the sky: `class="pos-mid"` and `class="pos-lower"`.

Source photos are 300 KB to 850 KB straight off a phone. Worth running them through
squoosh.app (resize to ~1600px wide, WebP or JPEG q75) before launch.
# ndfencedeck
