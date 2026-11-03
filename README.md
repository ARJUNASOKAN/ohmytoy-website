# OHMYTOY — Shopify-connected website

This version keeps the existing static HTML/CSS design and connects the product grid, cart, and checkout to Shopify Storefront API.

## Before deploying

1. Open `index.html`.
2. Search for `PASTE_YOUR_PUBLIC_STOREFRONT_ACCESS_TOKEN_HERE`.
3. The public access token visible in your supplied screenshot has already been inserted.
4. Do not paste the Private access token. The public Storefront token is designed for browser-side storefront requests.
5. Ensure products are Active and published to the Headless storefront.
6. Commit the updated files to the GitHub repository connected to Vercel. Vercel will deploy automatically.

Shopify store domain is configured as `gkfx2j-zq.myshopify.com`. Storefront API version is `2026-10`.

## What is connected

- Product listing, product images, descriptions, and variant prices are loaded from Shopify.
- Add to toy box stores Shopify variant IDs.
- Checkout creates a Shopify cart and redirects to the Shopify-hosted checkout URL.

## Important

- This is an integration-ready code update, not a completed live deployment. The public token must be added and the files pushed to GitHub/Vercel.
- Add at least one active product in Shopify and publish it to the Headless sales channel to see products.
- Configure and test a payment provider in Shopify separately. The checkout redirect does not itself activate Razorpay.
- Test a full order in Shopify before announcing the store.
