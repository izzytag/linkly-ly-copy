<!-- LOVABLE:BEGIN -->
> [!IMPORTANT]
> This project is connected to [Lovable](https://lovable.dev). Avoid rewriting
> published git history — force pushing, or rebasing/amending/squashing commits
> that are already pushed — as it rewrites history on Lovable's side and the
> user will likely lose their project history.
>
> Commits you push to the connected branch sync back to Lovable and show up in
> the editor, so keep the branch in a working state.
<!-- LOVABLE:END -->

## linkly architecture
- Plan rules (link limit, Pro-only themes, username validation) live in `src/lib/themes.ts` and are mirrored in DB (`is_pro()`, `enforce_link_limit` trigger) — the DB is the source of truth so limits can't be bypassed from the browser.
- Public pages `/$username` load via a public server function with the publishable key, so SSR can emit per-profile SEO tags.
- Avatars live in a private bucket served via long-lived signed URLs, because the workspace blocks public buckets.
- Billing goes through `src/lib/billing.ts`; Pro status must only be written server-side (verified Razorpay webhook), never from the client.
