# Turbo SMM Panel

This is the starter project for a real SMM panel using:
- HTML/CSS/JavaScript frontend
- Vercel serverless API
- Supabase Auth + PostgreSQL
- A common SMM provider API format (`/api/v2`, actions such as services/order/status)

## Setup

1. Create a Supabase project.
2. Open Supabase SQL Editor and run `supabase.sql`.
3. In Vercel, create a new project from this folder/GitHub repository.
4. Add the environment variables from `.env.example`.
5. Set your SMM provider API URL and API key.
6. Deploy.

## Important

Never put `SMM_API_KEY` in frontend JavaScript. It belongs only in Vercel Environment Variables.

The current UI is the visual front-end. The API routes are ready for:
- service synchronization
- placing orders
- order history
- provider status checking
- balance checking

Before going live, add:
- Login/Register UI using Supabase Auth
- Add Funds/payment gateway
- Admin dashboard
- automated service sync / markup
- refill/cancel endpoints if supported by your provider
- rate limits and abuse protection
