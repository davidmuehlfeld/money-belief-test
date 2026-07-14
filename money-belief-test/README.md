# The Money Belief Test

16 questions that uncover money beliefs that quietly make financial decisions for you.
A companion test for [I am invested](https://iaminvested.substack.com/).

Built on the money-scripts framework from financial psychology (Klontz et al., 2011).

## Files

| File | What it does |
|---|---|
| `index.html` | The entire test. One file, no dependencies, no build step, no tracking. |
| `.nojekyll` | Tells GitHub Pages to serve files as-is. |
| `robots.txt` | Lets search engines index the page. **Edit the domain line.** |
| `sitemap.xml` | Helps Google find it. **Edit the domain line.** |

## Deploy to GitHub Pages (5 minutes)

1. Create a new **public** repo on GitHub, e.g. `money-belief-test`.
2. Upload all four files (drag them into the repo upload page).
3. **Settings → Pages.**
4. Source: **Deploy from a branch**. Branch `main`, folder `/ (root)`. Save.
5. Wait ~1 minute. Live at `https://<username>.github.io/money-belief-test/`

## Before you publish — two edits

1. In `robots.txt` and `sitemap.xml`, replace `REPLACE-WITH-YOUR-DOMAIN` with your real URL.
2. In `index.html`, the `<link rel="canonical">` currently points at your Substack.
   Once the test has its own permanent URL, change it to that URL instead.

## Test locally

```bash
python3 -m http.server 8000
```
Open http://localhost:8000

## Custom domain (optional)

1. Add a file named `CNAME` containing just your domain, e.g. `test.iaminvested.co`
2. At your DNS provider, add a CNAME record pointing that subdomain to `<username>.github.io`
3. Settings → Pages → enter the domain → tick **Enforce HTTPS**

## Embedding in Substack

Substack does not allow custom JavaScript in posts. So:

- **Link out.** Put a button in the post pointing at the live URL. Cleanest option.
- Publish the questions + scoring table as plain text in the post, and link here for people
  who'd rather not add up four columns by hand.

## Scoring

Four groups, four questions each, straight sums out of 20:

| Type | Questions |
|---|---|
| The Avoider | 1–4 |
| The Chaser | 5–8 |
| The Show-off | 9–12 |
| The Worrier | 13–16 |

Highest score wins. Top two within 2 points → The Torn.

## SEO notes

Already included: meta description, keywords, canonical, robots, Open Graph, Twitter Card,
and JSON-LD `Quiz` structured data.

After deploying, submit the URL to [Google Search Console](https://search.google.com/search-console)
to get indexed in days rather than weeks.

Target keyword worth owning: **"money scripts quiz"** — low competition, high intent.

## Images

The logo and author photo hotlink to Substack's CDN. That works. If you'd rather not depend
on it, download both, drop them in the repo, and update the two `<img src>` attributes.

## License

Do what you like with it.
