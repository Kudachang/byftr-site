# byftr-site

---

# byftr.com — Build Log

Teaser page for the FUTURE brand, live at [byftr.com](http://byftr.com). Hosted on GitHub Pages from this repo (`main` branch).

This README doubles as a running build log. Newest entries at the top.

---

## 2026-08-04 — Teaser page locked (v1)

**Status:** Live and locked. This is a placeholder teaser, not the final site — just something to land on at the domain while the real site is built.

**Page contents:**
- FUTURE™ logo + wordmark (centered, image assets)
- Subline: "HUMAN CREATIVITY x AI VELOCITY"
- Tagline: "Something's coming. Not live yet."
- Contact: `future@byftr.com`
- Link: [about.me/Bill_Future](https://about.me/Bill_Future)
- Full-page video background with 40% black overlay for text legibility
- Footer: © 2026 FUTURE

**Files:**
- `index.html` — single-file page (logo + wordmark embedded as base64, Noto Sans via Google Fonts)
- `bg-video.mp4` — compressed full-bleed background video (960px wide, H.264, ~9MB)
- `CNAME` — GitHub Pages custom domain config (`byftr.com`)

**Infrastructure:**
- **DNS (Porkbun):** 4x A records at apex (`byftr.com`) pointing to GitHub Pages IPs (185.199.108–111.153). MX/TXT (Google Workspace email) untouched.
- **HTTPS:** auto-provisioned by GitHub Pages after DNS resolved.
- **Hosting decision:** moved off Porkbun's free "Link in Bio" product (a template-only microsite builder, not real file hosting) to GitHub Pages for full control over the custom HTML/design.
- **Auth note:** pushes use a classic GitHub PAT ("macbook", repo scope) — check expiration before future updates.

**Not done yet:**
- Replace teaser with the actual FUTURE site
- Re-encode background video for broader compatibility if playback issues are ever reported
