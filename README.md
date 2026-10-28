# Kashif Traders — Render-ready package

Single-seller public storefront for Kashif Traders, Pakistan.
Tagline: Your One-Stop Online Shopping Store.
Contact: +92309-6929813, ka9917578@gmail.com
Prices: PKR and USD, with USD converted from PKR at the live market rate when available (Rs 280 = $1 fallback, labelled "Fallback — not live").

## What this package is

- `index.html` — the complete, self-contained public storefront (products, categories, search, filters, product details, My List, WhatsApp ordering, contact).
- This is a **static storefront only**. It does NOT save customer accounts, orders, seller/admin data, or process online payments.
- The full marketplace with Admin, accounts, cart checkout and order tracking lives separately in Muse (artifact: kashif-traders) and is not included in this static package.

## Deploy on Render (free, Static Site)

1. Upload all files in this folder to the GitHub repository `KASHIF-Trader` (ka9917578-netizen), replacing/keeping README.md as needed. Keep `index.html` at the repository root.
2. In Render Dashboard: New > Static Site.
3. Connect the `KASHIF-Trader` repository.
4. Settings:
   - Build Command: (leave empty)
   - Publish Directory: `.` (root) — or leave as Render's default for a root index.html
   - Branch: main (or the branch you uploaded to)
5. Create Static Site. Render will give a free subdomain, for example `https://kashif-trader.onrender.com` (exact name depends on availability).
6. Test: home page, name at the very top, categories, search, PKR/USD prices, WhatsApp order button, contact phone/email.
7. Custom domain later: Render > Settings > Custom Domain, then add the DNS record Render shows. SSL is automatic.

## Notes

- Ordering on this static site is via prefilled WhatsApp messages, not a saved checkout.
- To show new products on the Render site, update this package and re-upload to GitHub; Render redeploys automatically.
- Do not put admin passcodes, API keys, or passwords in this repository.
- Online payments (JazzCash/Easypaisa/cards) and email notifications are NOT live in this package. Enable them only after merchant accounts and an email service are configured and tested.
