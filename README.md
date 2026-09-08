# ACA × ApexAlgos landing page

Two files: `index.html` (everything inline, no build step) and `favicon.svg` (the site icon). Both need to be uploaded — the favicon reference in `index.html` expects `favicon.svg` to sit next to it in the same folder.

## 1. Upload the files to your repo

Repo: `https://github.com/apexalgosindia/aca`

Easiest way (no git required):
1. Open the repo on github.com.
2. Click **Add file → Upload files**.
3. Drag in `index.html`, `favicon.svg`, and this `README.md` if you want.
4. Commit directly to the `main` branch.

Or with git:
```bash
git clone https://github.com/apexalgosindia/aca.git
cd aca
cp /path/to/index.html /path/to/favicon.svg .
git add index.html favicon.svg
git commit -m "Add landing page"
git push
```

## 2. Turn on GitHub Pages

1. In the repo, go to **Settings → Pages**.
2. Under **Build and deployment → Source**, choose **Deploy from a branch**.
3. Branch: `main`, folder: `/ (root)`. Save.
4. GitHub will give you a URL like `https://apexalgosindia.github.io/aca/` within a minute or two.

## 3. Optional: a custom domain

If you own a domain (e.g. `acaopen.in`):
1. In **Settings → Pages → Custom domain**, enter it and save — GitHub creates a `CNAME` file in your repo automatically.
2. At your domain registrar, add a `CNAME` record pointing your subdomain (e.g. `www`) to `apexalgosindia.github.io`, or `A` records for an apex domain pointing to GitHub's IPs (185.199.108.153, .109.153, .110.153, .111.153).
3. Wait for DNS to propagate, then tick **Enforce HTTPS** back in Pages settings.

## What's on the page

- Hero comparing ₹4/order (AC Agarwal via ApexAlgos) against ₹20/order (typical discount brokers)
- A live savings calculator (defaults to 1,000 orders/month, editable)
- Why-algo-traders-choose-this-account benefits section
- Step-by-step account opening flow, including the "don't log in during the XTS shift" warning
- Step-by-step Tradetron API connection guide, with a callout for MCX/static IP
- Support contact details

Everything is in one file, so editing copy just means editing the text inside `index.html` — search for the sentence you want to change.
