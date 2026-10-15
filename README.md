# Z-Screen investor & collaborator portal

Source for [www.z-screen.com](https://www.z-screen.com): the Z-Screen discovery platform portal, the technical white paper (web edition and PDF), and the evidence register behind every reported number.

> The site is intentionally unindexed (`noindex` meta tag). It is shared by link with investors and scientific collaborators.

## What lives here

- `docs/` - the public website, served by GitHub Pages from this folder
  - `docs/index.html` - portal (platform, benchmarks, chemical and genetic twins, prioritized programs, figure atlas)
  - `docs/whitepaper.html` - technical white paper, web edition
  - `docs/docs/ZScreen_Technical_White_Paper.pdf` - technical white paper, print PDF (V2.0, October 2026)
  - `docs/docs/RSI_Therapeutics_White_Paper_Draft.pdf` - companion volume, *Recursive Self-Improvement in Therapeutics*
  - `docs/evidence.html` and `docs/evidence/` - source tables with SHA-256 hashes and provenance
  - `docs/assets/figures/wp/` - figures generated directly from the evidence tables (SVG)
- `docs/CNAME` - custom-domain configuration (do not remove)

## Scope of the numbers

All compound and profile counts on the site describe the Z-Screen pilot dataset analyzed in the white paper (pilot package V2: 162,914 compounds, 190,699 compound-context profiles). They are not platform limits; Z-Screen is designed to scale to millions of compounds and beyond.

Chemical structure images and SMILES/scaffold fields are withheld in this public edition; tables retain compound identifiers and measured results (see `docs/PUBLIC_STRUCTURE_REDACTION.json`).

## Previous release

This portal supersedes the April 2026 five-preprint briefing that was previously served here. The reproducibility bundle for that release remains on Zenodo: [10.5281/zenodo.19872807](https://doi.org/10.5281/zenodo.19872807).

## Rebuilding

The site is generated from a private build folder (white-paper text, figure generator, portal template); `docs/` is the exported, ready-to-serve output. Regenerate and re-export from that folder, then replace `docs/` (keeping `docs/CNAME`).

## License

- Website code (HTML/CSS/JS) in `docs/`: MIT (see `LICENSE`)
- White paper PDFs: (c) Zafrens, Inc.

## Contact

[z-screen@zafrens.com](mailto:z-screen@zafrens.com) - feedback, partnerships, collaborations

[www.zafrens.com](https://www.zafrens.com) - about Zafrens
