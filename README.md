# fw-zoo-site

Fixture static site for Far & Wide "connector zoo" UAT — a realistic GitHub PR
patch target. Plain static HTML (`index.html` at repo root → detected stack
`static_html`).

Deliberately imperfect SEO so the fix generator has real work to propose:

- **Missing meta descriptions** on every page (`meta_tags` / `add_missing`)
- **Weak `<title>` tags** — "Home", "About", "Products", "Contact"
  (`meta_tags` / `replace_existing`)
- **Images with no `alt`** — hero, beans, roastery, product photos
  (`image_alt` / `patch_items`)
- No Open Graph / Twitter tags, no JSON-LD, no `llms.txt`, no canonical tags

Not a real business — "Meadowlark Roastery" is invented for testing.
