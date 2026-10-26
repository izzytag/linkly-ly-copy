# Linkly Ly

Build a link-in-bio web app for Indian creators and small businesses, like Linktree but priced at ₹99/month. Use React, Tailwind, and Supabase (auth + database). Mobile-first, fast, clean design.

BRAND

Name: linkly . Style: modern, minimal, friendly. Primary color: [e.g. indigo].

PUBLIC PAGE

- URL format: /username (e.g. yourapp.in/priya)

- Shows avatar, name, short bio, social icons, and a vertical list of link buttons

- Each link click is counted

- Support light/dark themes and 6 preset themes

- Include a "WhatsApp me" button and a "Pay via UPI" button (UPI ID shown as a QR + tap-to-pay link)

- Footer "Made with [YourAppName]" on the free plan only

DASHBOARD (after login)

- Sign up / login with Google and email

- Pick a unique username

- Edit profile: avatar upload, name, bio

- Add, edit, delete, and drag-to-reorder links (title, URL, on/off toggle)

- Add social links (Instagram, YouTube, WhatsApp, X, LinkedIn)

- Theme picker with live preview

- Analytics: total views, clicks per link, last 7 and 30 days (simple charts)

- Download QR code of my page

PLANS

- Free: up to 5 links, branding footer, basic analytics

- Pro ₹99/month: unlimited links, no branding, full analytics, all themes

- Add an upgrade page and a plan check in the app. Leave a placeholder for Razorpay subscriptions (I'll connect it next).

DATABASE (Supabase)

Tables: profiles, links, link_clicks, page_views, subscriptions. Add row-level security so users can only edit their own data, and public read for live pages.

EXTRAS

- Landing page with hero, features, pricing (Free vs ₹99), and a "Create your page" button

- Language switcher placeholder (English/Hindi)

- SEO meta tags and Open Graph preview on each public page

- Fully responsive; test at 375px width first

Build it step by step: auth and profiles first, then links and the public page, then analytics, then the landing page and pricing.

This project was built with [Lovable](https://lovable.dev).

**Live app**: https://linkly-ly.lovable.app

## Build with Lovable

Continue developing this project in the [Lovable editor](https://lovable.dev/projects/6dbf97d5-011f-4441-9f2f-454fade1269c).

- **Ship faster**: describe what you want to build and Lovable handles the code.
- **Stay in sync**: every change made in Lovable is committed straight to this repository.
- **Full ownership**: this code is yours. Push to `main` on GitHub and your changes sync back into Lovable, ready for your next prompt.

## Development

Prefer working locally? You need Node.js and npm — [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating).

```sh
git clone <this-repository-url>
cd <repository-name>
npm i
npm run dev
```
