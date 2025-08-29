
# AI Ticketing — Quick Deploy

This folder contains a static site you can deploy **as-is**. The site entry point is `ai-ticketing-otp-qr/index.html`.

## Option A — GitHub Pages (free)
1) Create a new repo on GitHub.
2) Upload the entire `ai-ticketing-otp-qr` folder (keep the folder name).
3) Go to **Settings → Pages**.
4) Under **Build and deployment**, set **Source** to **Deploy from a branch**.
5) Select the branch you pushed and **/ (root)** as folder, then **Save**.
6) Your site will be live at `https://<your-username>.github.io/<repo-name>/ai-ticketing-otp-qr/index.html`.

## Option B — Netlify (drag & drop)
1) Go to https://app.netlify.com/drop
2) Drag the **entire folder** `ai-ticketing-otp-qr` into the page.
3) Netlify will publish it at a URL like `https://<random-name>.netlify.app/ai-ticketing-otp-qr/`.
4) Set a custom subdomain in Site settings if you like.

## Option C — Cloudflare Pages
1) Create a new project in Cloudflare Pages.
2) **Direct Upload** → Upload the folder `ai-ticketing-otp-qr`.
3) Deploy; your link will look like `https://<project>.pages.dev/ai-ticketing-otp-qr/`.

## Option D — Vercel
1) `vercel` → Import this folder as a static project.
2) It will publish at `https://<project>.vercel.app/ai-ticketing-otp-qr/`.

## Local test quickly
- Double click `ai-ticketing-otp-qr/index.html` (works offline), or
- Run a local server: `python3 -m http.server` from the parent folder and open
  `http://localhost:8000/ai-ticketing-otp-qr/index.html`

## Important
- This is a **static** demo. For production, wire OTP, sessions, pricing, and fraud checks to your backend and issue **HttpOnly, Secure** cookies instead of client-only state.
