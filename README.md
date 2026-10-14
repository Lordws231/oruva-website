# Oruva — oruva.com.ng landing site

New investor-ready landing site for Oruva Transportation Services, built 2026-10-14
to replace the Osun-only site at oruva.polsia.io as Oruva's public home on the
paid domain **oruva.com.ng**.

Dependency-free static site: `index.html` + `styles.css` + `app.js` + `assets/`.
No build step. Drop into the `oruva-website` GitHub repo as-is, or serve from any
static host (Vercel / Cloudflare Pages / Netlify).

## Sections (all clickable from the sticky nav)
Hero · About · Mission & Vision · Problem & Solution · Features · Bridging the Gap ·
Long-Term Impact · Entertainment Hub · ORVA Ecosystem · Riders Networking & Community ·
Partners · Roadmap · For Investors ($150k–$250k pre-seed, per Pitch Deck 3.0) · FAQ · Footer

## Honesty notes baked into the copy
- Entertainment integrations (Netflix etc.) and partner categories are presented as
  the ecosystem/phases Oruva is *building*, not as signed partnerships.
- "Gas-free" ORVA payments are described as Oruva's payment hub covering network
  cost for in-app ORVA payments — wording to confirm with the founder before launch
  if the mechanism differs.
- No contact email/phone is published (none verified for public use). The investor
  section routes enquiries via the live Oruva Points site until an investor desk
  address at oruva.com.ng is confirmed.

## Deployment checklist (needs Esther/founder approval at each external step)
1. Push these files to GitHub repo `Lordws231/oruva-website` (currently README-only)
   via the secure GitHub connector — never a pasted token.
2. Create a Vercel project `oruva-website` under team ORUVA TRANSPORTATION SERVICES
   (framework: Other / static, no build command), production branch `main`.
3. Add domains `oruva.com.ng` and `www.oruva.com.ng` to the Vercel project.
4. In Cloudflare (domain already active there; nameservers elmo/paris):
   point DNS at Vercel per Vercel's instructions and set SSL to Full (Strict).
   — As of 2026-10-14 21:35 WAT, https://oruva.com.ng returns Cloudflare error 525
   (origin SSL handshake failure), i.e. the domain is not yet pointed at a working
   origin. Steps 2–4 fix that.
5. Verify https://oruva.com.ng loads with a valid certificate, then announce the move.
   oruva.polsia.io is hosted on the Polsia/Blaxel platform — redirecting or retiring
   it is done from that account, separately.

## Assets
- `assets/oruva-logo.jpg` — official Oruva logo supplied by Esther on 2026-10-14.
- `assets/oruva-mark.jpg` — emblem cropped from the official logo for nav/favicon/footer.
