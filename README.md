# Sheffield University RFC — Website

Static rebuild of the SURFC site rescued from Wix (`sharazeuan.wixsite.com/sheffield-university`).
Plain HTML + one CSS file, no build step, no JavaScript. Host it anywhere for free.

## Pages

| File | Page |
|---|---|
| `index.html` | Home — hero, 1st XV fixtures & results, upcoming events, media strip |
| `teams.html` | Squad overview + coaching staff & captains |
| `events.html` | Upcoming events |
| `gallery.html` | Match day gallery (30 photos) |
| `sponsors.html` | Sponsors, sponsorship tiers, partners |
| `style.css` | All styling |
| `assets/img/` | All 50 images, saved at original resolution from Wix's CDN |

## How to update content

Everything is plain HTML — open the file, edit the text, save.

- **Fixtures/results**: edit the two lists in `index.html` (search for "Last 5").
- **Events**: same block appears in `index.html` and `events.html`.
- **New photos**: drop the file in `assets/img/` and add an `<img>` tag in `gallery.html`.

## Deploying (all free)

**GitHub Pages** (recommended)
1. Create a repo on GitHub and push this folder.
2. Repo → Settings → Pages → Source: `main` branch, `/ (root)`.
3. Site appears at `https://<user>.github.io/<repo>/`.

**Netlify / Cloudflare Pages**: drag-and-drop this folder in their dashboard, done.

**Custom domain**: all of the above support one for free — you only pay for the domain itself (~£10/yr).

## Leftover placeholders from the Wix site (carried over as-is)

- Contact email is `email@sheffield.felixmakeitnow` — not a real address, appears in every footer and the sponsor "Enquire Now" buttons.
- Captain bios on `teams.html` still say "Insert bibliography...".
- Sponsorship tier benefits say "Beast tell us the credentials".
- Valued partners are "Partner 1–8" with no names.
- Wix's RSVP buttons couldn't migrate (they needed Wix's booking backend) — they now link to the club Instagram. Point them at a Google Form or SU page when you have one.
