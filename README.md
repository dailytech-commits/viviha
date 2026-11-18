# VIET HAN (VIVIHA) — B2B website source code

## Open locally
Open `index.html` in Chrome, or open the folder in VS Code and use Live Server. No build tools or dependencies required; language translations are bundled into `script.js` for file:// compatibility.

## Files
- `index.html` — structure and accessible sections
- `styles.css` — navy/orange responsive styling
- `script.js` — offline multilingual content and RFQ mailto behaviour
- `locales/en.json`, `vi.json`, `ko.json` — editable translations/reference files (if edited, also update the language bundles in script.js; no automatic build step is included)
- `data.json` — structured machine inventory and headcount by department
- `assets/` — 9 company-provided factory photos

## Grounding and publication notes
Source: 36-slide `2026-05-VIET HAN PROFILE.pptx` supplied by the company. Total workforce 260 is reproduced as stated even though department subtotals add to 250. Capacity figures are **alternative product scenarios on four lines**, not additive. Market split: Korea 70%, US 20%, EU/others 10%; profile does not give a measurement year for these shares. No unconfirmed certifications are asserted. Buyer names and logos are not displayed pending permission. Contact details shown are director and vice director from profile overview (slide 2); contact slide 35 lists additional/different roles and must be reconciled before going live. Department photos are placeholders until new company photos arrive. Korean translation should be professionally proofread.

## Inquiry form
The form opens an email draft via `mailto:`; it does not deliver messages automatically or store leads. Before launch, add server-side email integration, anti-spam measures, privacy notice and consent policy.


## Product carousel — Vests & jackets (November 2026 update)
- 18 product photos: `assets/products/jackets/jacket-01.png` to `jacket-18.jpg` (extensions vary; see `product-images.json`).
- The carousel is implemented in `script.js` (`productImages`, `renderProducts`, `changePhoto`, `openViewer`).
- Click the image to zoom; navigate with buttons or left/right keyboard arrows; press Escape to close.
- To add a new product category later: put the pictures in `assets/products/<category>/`, add their paths to `productImages` in `script.js` using the zero-based category index.
- Carousel controls and image captions change between English, Vietnamese and Korean.
- Image names are neutral; no claims about brand or exact model.
