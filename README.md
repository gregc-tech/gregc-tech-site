# gregc.tech

Personal site for Greg Collins: a short about page and an online resume.

**Live:** [gregc.tech](https://gregc.tech)

## Pages

| File | What it is |
|---|---|
| `index.html` | About / landing page |
| `resume.html` | Resume / CV, with a print-friendly layout ("Print / Save PDF") |
| `styles.css` | Shared styles, including dark mode and print styles |
| `favicon.svg`, `apple-touch-icon.png` | Browser tab and home-screen icons |
| `images/portrait.jpg` | Portrait |
| `CNAME` | Custom domain for GitHub Pages |

## How it's built

Plain HTML and CSS. No build step, frameworks, or JavaScript beyond the print button. Fonts are loaded from Google Fonts (Space Grotesk, Inter, JetBrains Mono).

## Hosting

Served by GitHub Pages from the `main` branch root, with HTTPS enforced. DNS is managed at GoDaddy:

- `A @` → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
- `CNAME www` → `gregc-tech.github.io`

Email for the domain runs through iCloud+ Custom Email Domain. Leave the MX, SPF/DMARC TXT, and `sig1._domainkey` records alone when changing DNS.

## Updating

Edit the files, then commit and push to `main`. GitHub Pages republishes in a minute or two.

To preview locally:

```bash
python3 -m http.server 8765
```

Then open http://localhost:8765.
