# $LEZARD 🦎 — le lézard du chain

The official landing page for $LEZARD, the meme coin on TON.

## What's in this repo

- **`index.html`** — the entire site. One self-contained file with all images embedded (base64) and fonts loaded from Google Fonts CDN. No build step, no dependencies.
- **`.nojekyll`** — tells GitHub Pages not to process this with Jekyll (so files starting with `_` are served correctly).

## Deploy

### Option A — GitHub Pages (recommended)

1. Create a new GitHub repo (e.g. `tonlezard-site`).
2. Upload `index.html` and `.nojekyll` to the root of the `main` branch.
3. In the repo, go to **Settings → Pages**.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Select **`main`** branch, **`/ (root)`** folder. Save.
6. Wait ~1 minute. Your site will be live at `https://<username>.github.io/<repo-name>/`.

For a custom domain (like `tonlezard.com`), add a `CNAME` file with the domain inside it and configure your DNS to point to GitHub Pages.

### Option B — Netlify Drop

Drag both files into [netlify.com/drop](https://app.netlify.com/drop). Live in seconds.

### Option C — Vercel

Push to GitHub, then import the repo into Vercel. Auto-detects as a static site.

## Editing things later

All editable values are in `index.html`. Search for these placeholders to update them before launch:

| What | Where to look for it |
|---|---|
| Contract address | `EQDxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx` (in the contract bar) |
| Telegram link | `href="#"` inside the `TELEGRAM` buttons (hero + footer) |
| Sticker pack link | `href="#"` on the `STICKER PACK 🦎` button (footer) |
| DEXScreener link | `href="#"` on the `DEXSCREENER 📈` button (footer) |
| Ston.fi swap link | `href="#"` on the `SWAP ON STON.fi` button (Hop In section) |
| DeDust swap link | `href="#"` on the `SWAP ON DEDUST` button (Hop In section) |
| Chart link | `href="#"` on the `CHART ON GECKOTERMINAL` button (Hop In section) |
| X/Twitter link | Already wired to `https://x.com/tonlezard` |

The marquee strip text lives in the `<div class="marquee-track">` near the top of the body if you want to change it.

## Tech notes

- Single HTML file, ~600 KB
- No framework, no JS dependencies beyond a tiny scroll listener for the jumping mascot
- Fonts: Bagel Fat One + DM Mono + Rubik Mono One via Google Fonts
- Designed mobile-first, scales to desktop
- The jumping lezard pinned to the bottom-right fades in once the user scrolls past the hero

## Credits

Mascot art by the $LEZARD community. Built with care for the colony.

🦎 ssssss
