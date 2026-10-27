# Hoorvia.net — Free Printable Cheat Sheets & Reference Charts

Static site for GitHub Pages, built from the user's sample Tailwind template and rebranded from PrintSheetPro to Hoorvia.

Tagline: Free Printable and Cheat Sheets

## Stack
- Plain HTML + Tailwind CSS via CDN (sample tailwind.config: paper #F8FAFC, warmPaper #FAF9F6, slateText #1E293B, brandNavy #0F172A, brandTeal #0D9488, ctaGreen #10B981 / hover #059669, ctaAmber #F59E0B / hover #D97706; Plus Jakarta Sans headings, Inter body)
- No build step, no framework, no WordPress (GitHub Pages cannot run WordPress)
- `.nojekyll` is included so GitHub Pages serves files exactly as-is without Jekyll processing.

## Structure
- `index.html` — homepage: sticky header, hero, live search, category filter pills, 20 cards, trust section
- `kitchen/`, `crafting/`, `home-health/`, `tech/` — category pages + 5 post pages each (20 posts total)
- `about.html`, `contact.html`, `privacy-policy.html`, `terms.html`, `disclaimer.html` — legal pages (footer links, not modals)
- `assets/pdfs/` and `assets/previews/` — future homes for real PDFs / WebP previews (see their README files)
- `sitemap.xml`, `robots.txt`, `ads.txt`, `CNAME` (hoorvia.net)

## Downloads — honest note
There are currently NO PDF files in this repo. Download buttons open the browser print dialog; the user chooses "Save as PDF" and selects US Letter or A4. The print stylesheet hides header, footer, buttons and guides so only the printable sheet prints. Do not add fake PDF links.

## Deploy (not yet done)
1. Push this folder to the `main` branch of a public repo (e.g. `hoorvia-info`), at repo root.
2. GitHub: Settings → Pages → Deploy from branch `main` / root.
3. Custom domain: set `hoorvia.net` in Pages settings, Enforce HTTPS.
4. DNS: apex A records 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153; www CNAME → `<username>.github.io`.
5. Before AdSense: replace the placeholder in `ads.txt` with the real publisher ID, and replace the clearly-marked contact placeholder in `contact.html` with a real email. No AdSense approval is claimed or guaranteed.
