https://<your-github-username>.github.io/2026021802-t3mp/

# Lowpoly Cloud Explorer (GitHub Pages)

This repository now hosts a lowpoly 3D isometric-style browser demo featuring:
- A non-perspective (orthographic) isometric-style camera with a gear-menu for view angle (default **45°**), cloud spin control, and light brightness control (50% to 500%).
- A player cloud you can move with **WASD / Arrow keys** or **click/tap-to-move**.
- Opening the settings menu pauses simulation until closed.
- Procedurally generated multi-scale terrain with **large oceans**, **high ranges**, **water**, and **trees**.
- Chunk-based streaming so terrain supports effectively **unlimited travel** in any direction.
- Cloud lifecycle behavior: over water it gains sparkling vapor and grows (denser footprint), and at high elevations it darkens before rain then shrinks back toward white.
- Transparent shallow-water rendering with a lighter color palette and smoother terrain color blending.

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

```bash
python3 -m http.server 4173
```

Then open <http://localhost:4173>.

## Expansion notes

The terrain system is intentionally configured via the `CONFIG` object in `index.html` to make future scope expansion easier (biomes, resources, weather, NPCs, structures, etc.).
