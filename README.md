# Clothify — Demo Store (Vite + React + Tailwind)

This is a ready-to-run demo storefront for *Clothify*.

## Quick start (locally)
1. Install deps:
   ```
   npm install
   ```
2. Start dev server:
   ```
   npm run dev
   ```
3. Open http://localhost:5173

## Stripe Checkout (optional)
The demo includes a serverless function at `/api/create-checkout-session`.
To enable:
1. Provision a Stripe account and get your **Secret Key** (test mode).
2. Deploy the serverless function (Vercel, Netlify Functions or Express).
3. Set environment variable `STRIPE_SECRET_KEY` for the deployment.
4. Set `SUCCESS_URL` and `CANCEL_URL` env vars or edit the handler.

## Deploy to Vercel
1. Create a GitHub repo and push these files.
2. Go to https://vercel.com/new and import the repo.
3. In Vercel settings, add `STRIPE_SECRET_KEY` if using Stripe.
4. Deploy — Vercel will provide a public URL.

## Notes
- This is a demo. Replace contact email and product data before going live.
- For production payments, set up proper webhooks, inventory checks, and SSL.
