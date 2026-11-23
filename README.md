# Free Shopify Product CSV Checker

Find Shopify product CSV import errors **by row and column** before you upload — invalid handles, duplicate variants, empty prices, SKUs broken by Excel (`8.90123E+11`), wrong encoding (`Ã©`, `â€™`), semicolon separators, bad image URLs and more.

**▶ Use it now: https://ceoyur.github.io/shopify-csv-checker/** — or download `index.html` and double-click it.

- Free, no sign-up
- Private: runs entirely in your browser, your file is never uploaded
- Works with the current Shopify product CSV template and the older one (`Handle`, `Variant SKU`, `Image Src`)

## What it checks

| Area | Examples |
|---|---|
| File | Windows-1252 / non-UTF-8 encoding, garbled characters, `;` or tab separators, unclosed quotes, shifted cells, duplicate or missing columns |
| Products | Invalid or missing handles, two products sharing one handle, product rows scattered through the file, missing Title or Status |
| Variants | Duplicate option combinations, missing option values or names, duplicate SKUs, SKUs/barcodes in scientific notation |
| Values | `$19.99` / `19,99` prices, empty prices (import as 0.00), compare-at ≤ price, cost > price, `0.5 kg` weights, `Yes`/`No` booleans, invalid status / inventory policy / weight unit |
| Images & SEO | URLs without `https://` or with spaces, `_small`/`_thumb` images, invalid image positions, SEO title > 70 / description > 320 chars, > 250 tags |

## Full version

The free checker **shows** problems. **[CSV Preflight full version](https://ceoyur.gumroad.com/l/csv-preflight?utm_source=github&utm_medium=lite&utm_campaign=csv_preflight)** ($19, one-time) also:

- **auto-fixes** the routine problems and downloads a clean, import-ready file
- **converts supplier / wholesaler spreadsheets** (any column names) into Shopify CSV with variants, images, and price markup (×, +, round to .99)
- runs **offline** as a downloaded file on Windows and Mac

---

Not affiliated with or endorsed by Shopify Inc. "Shopify" is a trademark of Shopify Inc.
