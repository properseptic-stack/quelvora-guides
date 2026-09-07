# Quelvora Guides (affiliate / Impact Website channel)

Minimal static site for **Bryan Bergen** (Salmon Arm, BC / properseptic@gmail.com).

Purpose:

- Owned **Website** property for Impact.com Partner verification
- Demand Scout / Amazon.ca Associates (`quelvora-20`) content home
- Practical BC septic + rural + landlord guides (not social-first)

**Do not** create new Etsy products from this repo. Quelvora Etsy sales-hold remains.

## Local layout

```
quelvora-affiliate-site/
├── index.html
├── about.html
├── articles/
│   └── septic-additive.html
├── css/styles.css
├── robots.txt
├── impact-site-verification.html   # stub — fill Impact token later
├── IMPACT.md
└── README.md
```

## Preview locally

```bash
cd /workspace/quelvora-affiliate-site
python3 -m http.server 8080
# open http://127.0.0.1:8080/
```

## Publish to GitHub Pages (free, fully controlled)

`gh` was **not** authenticated when this site was built. Do not buy a domain yet.
Use `*.github.io` until Impact verification works.

### One-time (Bryan / CoS on Bryan’s machine)

1. Log into GitHub as Bryan (browser or `gh auth login`).
2. Create a **public** repo, e.g. `quelvora-guides` (or `quelvora-affiliate-site`).
3. From this folder:

```bash
cd /workspace/quelvora-affiliate-site   # or copy folder to Bryan’s machine first
git init
git add .
git commit -m "Initial Quelvora Guides static site for Impact Website channel"
git branch -M main
git remote add origin https://github.com/BRYAN_GITHUB_USER/quelvora-guides.git
git push -u origin main
```

4. GitHub → **Settings → Pages**:
   - Source: **Deploy from a branch**
   - Branch: `main` / root `/`
   - Save

5. Wait 1–2 minutes. Home URL will be:

```
https://BRYAN_GITHUB_USER.github.io/quelvora-guides/
```

(If the repo is named `BRYAN_GITHUB_USER.github.io`, the home URL is `https://BRYAN_GITHUB_USER.github.io/`.)

6. Confirm these load:

- `/` (home)
- `/about.html`
- `/articles/septic-additive.html`
- `/impact-site-verification.html`
- `/robots.txt`

7. Then follow **IMPACT.md** to connect + verify ownership in Impact Partner.

### Optional custom domain later

Do **not** buy a domain until Impact Website connect works on github.io.
When ready: Pages → Custom domain → add `CNAME` / DNS as GitHub documents.

## Affiliate rules (Amazon.ca)

- Store ID: **quelvora-20** (LIVE)
- Example product links already use `?tag=quelvora-20` and `rel="sponsored"`
- **Bryan per-message sign-off** before publishing any new affiliate post / paid promo
- Prefer education-first copy; never spam dumps of ASIN lists

## What not to do

- Do not push while `gh auth status` shows logged out (this box was logged out)
- Do not create GitHub accounts or buy domains from automation
- Do not publish new Etsy listings from this workstream
