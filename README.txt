IBI Proforma & Tax Invoice Generator — v2.0
============================================
v2.0: Added "Label + Invoice" print — a shipping label (Deliver-To / Return
address, Prepaid/COD badge, Code-128 barcode of AWB / order / invoice no.,
weight + contents) on the TOP half of an A4 sheet, and a compact Tax Invoice /
Bill of Supply on the BOTTOM half. Toggle it in the preview toolbar
("Full invoice" / "Label + Invoice"). The original full-page invoice is unchanged.

Deploy as a static site (e.g. GitHub Pages). Put ALL these files in the
SAME folder / repo root so the PWA, icons and social preview resolve:

  index.html               <- the app (open this)
  service-worker.js        <- offline cache (cache: ibi-pinv-v2.0)
  manifest.webmanifest     <- PWA metadata
  preview.png              <- Open Graph / Twitter preview image
  icon-192.png
  icon-512.png
  icon-maskable-512.png

GitHub Pages quick deploy:
  1. Create/choose a repo (e.g. invoice.indiabusinessinternational.online or a /invoice path).
  2. Upload all files above to the repo root (or a /docs folder).
  3. Settings > Pages > Source: main branch (root or /docs) > Save.
  4. Add CNAME for your subdomain if using one.

Version bumps: minor patch -> v1.2 ; major feature -> v2.0
Remember to bump VERSION in index.html AND the cache name in service-worker.js together.
