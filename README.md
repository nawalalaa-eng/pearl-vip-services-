# VIP Concierge — Bilingual installable PWA

An English/Arabic academic demonstration for VIP airport service bookings.

## Included
- Home and six VIP services
- Booking form (name, service, arrival/departure, date, passengers, optional flight number)
- Confirmation with unique demo booking reference
- Saved bookings and deletion, using **localStorage on each device only**
- Arabic/English toggle, navy/gold styling, installable PWA manifest and offline cache

## Publish free with GitHub Pages
1. Create a free account at https://github.com and a new **public** repository (for example `vip-concierge`).
2. Upload **the contents** of this folder to the root of the repository, keeping the `icons` folder.
3. Go to **Settings → Pages → Build and deployment → Deploy from a branch**, select `main` and `/ (root)`, then Save.
4. Wait for the site to deploy. Its URL is usually `https://YOUR-USERNAME.github.io/vip-concierge/`.
5. Open the URL over HTTPS on a phone. On iPhone Safari: Share → Add to Home Screen → Add (enable Open as Web App if offered). On Android Chrome: menu → Install app / Add to Home screen.
6. Share the same URL with your instructor and team.

## Important limitations
- This is a **working demo**, not a live airport reservation system. It does not contact airports, process payments, or check real lounge availability.
- Bookings persist only in the browser/device where they were created. Clearing browser storage removes them; there is no shared database or authentication.
- To share bookings across devices, add a backend such as Supabase with authentication and row-level security. Do not put privileged database keys in public front-end files.
- Service workers and installability require HTTPS or localhost. Opening `index.html` directly as a file does not fully test PWA installation.
- GitHub Pages hosting is free for public repositories, subject to GitHub's terms and limits.
