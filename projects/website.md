# electricmotogarage.com

**Company website, store, order system and admin, all on Cloudflare's edge.**

## What I built
- A static site served by a Cloudflare Worker, with product pages, guides and an interactive app demo.
- Orders: PayPal payment notifications are recorded in a Cloudflare D1 database and shown on an admin orders dashboard.
- An admin area behind Cloudflare Access (single sign-on), plus a weekly email digest.
- Product notify and sign-up forms protected by Turnstile.
- Media stored in R2, and a deploy process that checks the live site against the local copy before every deploy.

## Engineering focus
Fast pages, good search ranking, and a small attack surface: nothing private is reachable without signing in.

Live: https://electricmotogarage.com
