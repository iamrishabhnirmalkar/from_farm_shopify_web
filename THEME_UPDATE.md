# Why Your Theme Changes Don’t Show & How to Update

## Why edits don’t appear on the live store

The files in this folder are your **local theme**.  
Shopify serves the **theme that’s installed in your store**.  
Until you **upload/push** this local theme to Shopify, the live or preview theme will not include your latest edits.

So: **local changes ≠ live theme** until you deploy.

---

## How to get your updates onto the theme

### Option 1: Shopify CLI (recommended)

1. **Install Shopify CLI** (if needed):
   ```bash
   npm install -g @shopify/cli @shopify/theme
   ```

2. **Log in and connect your store**:
   ```bash
   cd /path/to/fromfarm_shopify_web
   shopify auth login --store YOUR-STORE.myshopify.com
   ```

3. **Push this theme to Shopify** (overwrites the linked theme on the store):
   ```bash
   shopify theme push
   ```
   Or push to a **new** theme (safe, doesn’t overwrite current):
   ```bash
   shopify theme push --unpublished
   ```

4. **Live preview while you edit** (see changes as you save):
   ```bash
   shopify theme dev
   ```
   This gives you a preview URL; saving files refreshes the preview.

---

### Option 2: Zip and upload in admin

1. Zip the theme folder (include all files: `layout`, `sections`, `snippets`, `assets`, `config`, `locales`, `templates`, etc.).
2. In Shopify admin: **Online Store → Themes → Add theme → Upload zip file**.
3. After upload, **Preview** the new theme and, when ready, **Publish** it.

---

### Option 3: Edit in Theme Editor (no local files)

- In Shopify admin: **Online Store → Themes → Customize**.
- Changes you make there are saved **directly to the theme** on Shopify.
- Those changes are **not** in this local folder unless you download the theme again (e.g. `shopify theme pull`).

---

## Quick checklist

- [ ] I’ve run `shopify theme push` (or uploaded the theme zip) after making local changes.
- [ ] I’m previewing/publishing the **same theme** I just pushed/uploaded.
- [ ] I’ve done a hard refresh (Ctrl+F5 / Cmd+Shift+R) or cleared cache to avoid old CSS/JS.

---

## Performance improvements in this theme

- **Single global load for custom CSS**  
  `rish-custom.css` is loaded once in the theme layout (in `snippets/stylesheets.liquid`) instead of in each section. That means one request and better caching, which improves load time.

- **Background images**  
  Blog and other sections use the same pattern as Category/About: `background-size: cover`, `background-position: center`, `background-repeat: no-repeat` so images display correctly and consistently.

For more on deployment and CLI, see: [Shopify Theme CLI](https://shopify.dev/docs/themes/tools/cli).
