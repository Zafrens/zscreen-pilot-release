Z-Screen public portal (pilot data package V2)

Open index.html in a browser. The technical white paper is available as a web edition (whitepaper.html) and as a print PDF (docs/ZScreen_Technical_White_Paper.pdf). The evidence register (evidence.html) links every source table with its SHA-256 hash.

All compound and profile counts describe the Z-Screen pilot dataset analyzed in the white paper (162,914 compounds, 190,699 profiles). They are not platform limits.

Chemical structure images and downloadable SMILES/scaffold fields have been removed. Public tables retain compound IDs and measured results. The companion RSI PDF has also had its structure figure removed. See PUBLIC_STRUCTURE_REDACTION.json.

Source-file hashes and sanitized-download hashes are distinguished in evidence/provenance.json. Source analysis directories remain private and unchanged.

Rebuilding the site and PDF
  The white paper text lives in _build/content.html; the portal page in _build/index.template.html; the generated figures in _build/figures.mjs (built from the evidence/ CSVs).
  node _build/build.mjs          regenerates assets/figures/wp/*.svg, whitepaper.html and index.html
  node _build/build.mjs --pdf    also renders docs/ZScreen_Technical_White_Paper.pdf (needs Google Chrome and `npm install puppeteer-core` inside _build)

  node _build/export.mjs         writes a clean drop-in copy of the site (only referenced files, plus .nojekyll) to _build/out/site for hosting, e.g. as /portal on z-screen.com
