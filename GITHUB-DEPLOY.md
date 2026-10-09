# GitHub deployment — UCC v7.2.7

Repository target: `Kid-klever/WWE-2k26-Universe-Mode-Control-Center`

The GitHub connector available in this chat can read the repository but currently returns `403 Resource not accessible by integration` on write operations. Until that permission is repaired, deploy this package manually.

## Upload
1. Open the repository on GitHub.
2. Upload/replace `index.html` at the repository root.
3. Upload the entire `assets/` directory and `.nojekyll`.
4. Keep `README.md` and `docs/` if you want the release documentation in the repository.
5. The old root `app.js`, `data.js`, and `styles.css` are no longer referenced by v7.2.7. They can be deleted after the new build is verified.
6. In **Settings → Pages**, publish from the `main` branch and `/ (root)`.

No npm install or build command is required. All paths are relative so the site works from a GitHub Pages repository subpath.
