# Sheffield University RFC — Website

The club website, live at **https://surfc.co.uk** (rescued from Wix, hosted free on GitHub Pages).

## Updating the site — no code needed

Content lives in simple data files that the pages fill in automatically. Edit it at
**[pagescms.org](https://pagescms.org)**: sign in with GitHub, open this repo, and you get
friendly forms for:

- **Fixtures & Results** — update the Last 5 / Next 5 lists after each match
- **Upcoming Events** — add/remove events, upload a photo
- **Teams** and **Coaches & Captains** — photos, names, bios
- **Sponsors & Partners** — logos, links, tier benefits
- **Match Gallery** — upload match photos
- **Site Settings** — contact email, address, social links

Hit **Save** and the live site updates itself in about a minute.

### Giving a committee member access

1. They create a free account at github.com
2. Repo → **Settings → Collaborators → Add people** → their username
3. They accept the email invite, then sign in at pagescms.org and pick this repo

## For developers

Plain Jekyll (built natively by GitHub Pages — no Actions, no gems to install):

| Path | What |
|---|---|
| `_data/*.yml` | All editable content (this is what Pages CMS edits) |
| `_layouts/default.html` | Shared header/footer shell |
| `index/teams/events/gallery/sponsors.html` | Page templates (Liquid) |
| `style.css` | All styling — zero JavaScript on the whole site |
| `assets/img/` | Images (originals pulled from Wix's CDN) |
| `.pages.yml` | Pages CMS form definitions |
| `CNAME` | Custom domain (surfc.co.uk) |

Deploys automatically on every push to `master`.

## Known placeholders carried over from the old Wix site

- Contact email `email@sheffield.felixmakeitnow` is not a real address
- Captain bios say "Insert bibliography…" — edit under **Coaches & Captains**
- Tier benefits say "Beast tell us the credentials" — edit under **Sponsors & Partners**
- Valued partners are "Partner 1–8"
- RSVP buttons link to Instagram (Wix's RSVP needed their backend) — point them at a
  Google Form via **Upcoming Events** when ready
