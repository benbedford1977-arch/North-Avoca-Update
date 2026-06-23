# North Avoca Update

A textable community + property landing page for Ben Bedford (Ray White Central Coast).
Single self-contained `index.html` — no build step.

## What's tracked
- **Meta Pixel `414979734385927`** ("Ben Bedford Pixel") — fires `PageView`
- Custom events (visible in Events Manager):
  - `Scroll50`, `Scroll90` — scroll depth
  - `ReadCommunity`, `ReadRealEstate`, `ReachedCTA` — sections reached
  - `Engaged30s` — spent 30s+ on page
  - `CTAClick` + standard `Lead` — tapped Call / Book appraisal
- Everyone who opens the link → retargetable Meta custom audience.

## Deploy to GitHub Pages
1. Create a new GitHub repo (e.g. `north-avoca-update`).
2. Upload `index.html` (and the `images/` folder) to the repo root.
3. Repo → **Settings → Pages** → Source: `main` branch, `/root` → Save.
4. Live at `https://<username>.github.io/north-avoca-update/` in ~1 min.
5. (Optional) Add a custom domain on that same Pages settings screen.

## Then
- Paste the live URL into **Bitly** → get the short link to text out.
- In Events Manager, confirm events fire (use the Test Events tool + your phone).

## Appraisal form (Web3Forms)
The CTA form posts to Web3Forms (free, no account, emails each lead to you).
**Setup:** get an access key at web3forms.com using your email, then replace
`YOUR-WEB3FORMS-ACCESS-KEY` in index.html. Fires pixel `Lead` + `AppraisalRequest`
on success.

## Still to fill in (search "PLACEHOLDER" in index.html)
- Web3Forms access key (for the appraisal form)
- General Store: exact name + years running
- The Boy & The Rose: how long under Sonia (name/hours confirmed)
- People's Physiotherapy: location, physio name, services
- Photos: drop real images into `images/` and uncomment the `<img>` tags

## Done
- Real estate section: live with real figures from the 23/06/2026 suburb report
- Phone: 0433 778 000 wired into Call button
- Brand: "Ray White" (no suburb)
