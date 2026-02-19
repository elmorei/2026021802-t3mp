https://<your-github-username>.github.io/2026021802-t3mp/

# Flags! GitHub Page

This repo contains a single-page GitHub Pages site with:
- A bouncing **"Flags!"** heading.
- Click-to-change heading color.
- A full-screen, animated **4D simplex noise** background.

## Steps to take the page live after merge

1. Push the merge commit to your default branch (for example `main`).
2. In GitHub, open **Settings → Pages**.
3. Under **Build and deployment**, set:
   - **Source**: `Deploy from a branch`
   - **Branch**: your default branch (for example `main`)
   - **Folder**: `/ (root)`
4. Save the settings and wait for deployment to complete.
5. Visit the URL at the top of this README.

## Local preview

You can run a local web server from the repository root:

```bash
python3 -m http.server 4173
```

Then open <http://localhost:4173>.
