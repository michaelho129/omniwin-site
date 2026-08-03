# Omniwin Limited — Public Site

A single static page for `theomniwin.com`.

## Deploy

1. Sign in to [Cloudflare Pages](https://pages.cloudflare.com/).
2. Create a project → **Upload assets** (drag and drop this folder).
3. Add custom domain `theomniwin.com`.
4. Cloudflare will show the exact DNS records to add in GoDaddy. Add **only** those two records:
   - one apex record for `@`
   - one `www` CNAME
   Do **not** change MX, TXT, SPF, DKIM, or NS records.
5. Wait for certificate provisioning, then verify:
   - `curl -sI https://theomniwin.com` returns `200`
   - `curl -sI https://www.theomniwin.com` returns `200`
   - `dig MX theomniwin.com +short` matches the value before the DNS edit.

## Content

- Entity: Omniwin Limited
- Location: Hong Kong
- Focus: Household software
- Contact: michael@theomniwin.com

No product names or branding for unreleased apps appear here (trademark-hold policy).
