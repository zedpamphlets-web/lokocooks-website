# Loko Cooks Website

Static website for **Loko Cooks** – Good Food. Closer to You.  
Food delivery from Lusaka’s markets to your door.

## Project Structure

```
├── index.html          # Homepage
├── privacy.html        # Privacy Policy
├── terms.html          # Terms & Conditions
├── css/
│   └── style.css
├── img/
│   ├── favicon.png
│   ├── logo.png
│   ├── food.jpg
│   └── flame.png
└── _redirects          # Netlify redirects for clean URLs
```

## Deployment

This is a pure static site. No build step is required.

### Recommended: Netlify

1. Go to [Netlify](https://app.netlify.com) and connect this GitHub repository.
2. Build settings:
   - **Build command**: (leave empty)
   - **Publish directory**: `/` (or `.`)
3. Deploy. The `_redirects` file will automatically handle:
   - `/privacy` → `/privacy.html`
   - `/terms` → `/terms.html`

### Vercel

1. Import the repository on [Vercel](https://vercel.com).
2. Framework preset: **Other** (or Static).
3. Deploy. No configuration needed.

### GitHub Pages

1. Go to repository **Settings → Pages**.
2. Source: Deploy from a branch → `main` → `/ (root)`.
3. Note: Clean URL redirects (`/privacy`, `/terms`) will **not** work automatically on GitHub Pages. Users will need to visit the `.html` versions, or you can use a custom 404.html approach if desired.

## Local Preview

Just open `index.html` in a browser, or use any static server:

```bash
npx serve .
# or
python -m http.server 8000
```

## License

Private project for Loko Cooks.
