# Impact.com Partner — Website channel + ownership proof

Owner: **Bryan Bergen** · Salmon Arm, BC · properseptic@gmail.com  
Site: Quelvora Guides (this static folder)  
Amazon.ca Associates: **quelvora-20** (LIVE; tax done)  
Etsy: Quelvora shop exists but Impact will **not** unlock “Next” on an unverified Etsy URL — hence this owned site.

## What Impact needs

1. **Website channel connected** in Impact Partner (not Instagram / TikTok — not required for this path).
2. **Ownership verification** of that URL via one of Impact’s methods (typically):
   - Meta tag in `<head>` of the homepage, **or**
   - Upload / host a verification HTML file at a path Impact specifies, **or**
   - DNS / file token (less common for simple Partners — follow the in-console wizard)
3. Site must be **publicly reachable over HTTPS** with real content (home + about + at least one article is enough to look legitimate).

Impact will reject or stall on:

- Unverified marketplace storefront URLs (e.g. raw Etsy shop links)
- Empty parking pages / parked domains
- Sites you don’t control (Medium/Substack can work for *content*, but ownership verify is cleaner on a repo you push yourself — GitHub Pages preferred)

## How we’ll prove ownership once hosted

1. Publish this folder to **GitHub Pages** (see README.md). Example home URL:

   `https://BRYAN_GITHUB_USER.github.io/quelvora-guides/`

2. In Impact Partner → Channels / Properties → **Add Website** → paste that exact base URL.

3. Impact shows a token. Put it in **one** place:

   - Preferred for this repo: edit root `impact-site-verification.html`
     - Replace `REPLACE_WITH_IMPACT_TOKEN` in the meta tag **and/or**
     - Replace file contents with whatever HTML file Impact downloads for you
   - Or add Impact’s meta tag into `index.html` `<head>` if that’s what the wizard asks

4. Commit + push; wait for Pages CDN (~1 min).

5. Click **Verify** in Impact. Confirm fetch succeeds on:

   `https://…github.io/…/impact-site-verification.html`  
   (or whatever path Impact listed)

6. After verify: request / unlock partner programs that required a Website property; use this same URL as the Demand Scout / content home when asked for a site.

Stub already in repo:

```
impact-site-verification.html
```

Keep that filename unless Impact mandates a different path — then rename/add as instructed and note it here.

## Next CoS steps (recommended order)

| Step | Action | Owner | Blocker |
|------|--------|-------|---------|
| 1 | Bryan (or CoS with Bryan present) runs `gh auth login` on a machine with his GitHub | Bryan | **gh not authenticated on build box** |
| 2 | Create public repo + push this folder + enable Pages | CoS / Bryan | Needs gh auth |
| 3 | Hand Bryan the live github.io URL for one-click Impact “Add Website” | CoS | After Pages live |
| 4 | Paste Impact token into stub → push → Verify | CoS | Impact console token |
| 5 | Demand Scout / program applications using verified Website | Bryan sign-off | Impact verify done |
| 6 | New affiliate articles: draft here → **Bryan per-message sign-off** before publish | Both | Content approval |
| — | Custom domain | Later | Do **not** buy until github.io verify works |
| — | Substack | Optional parallel | Good for email; weaker as sole Impact ownership proof vs Pages we control |
| — | Etsy URL for Impact | Skip | Unverified Etsy won’t unlock Next |

### Recommended next step for CoS

**Push GitHub Pages first** (one Bryan auth click / `gh auth login`), then hand Bryan the live URL for Impact Website connect. Prefer Pages over Substack for ownership verify. Do not buy a domain yet.

## Compliance notes

- Affiliate posts / Amazon deep-links: Bryan sign-off per message before publishing.
- Quelvora Etsy: sales-hold — no new products/listings from this stream.
- Niches for future posts: (1) BC septic/ROWP (2) rural winter resilience (3) Canadian landlord ops.
