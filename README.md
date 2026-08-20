# Web Artifacts

A collection of small, standalone HTML/JS tools, served as a static site via GitHub Pages.

## Structure

```
.
├── index.html              # landing page listing all artifacts
├── .nojekyll                # disable Jekyll processing on GitHub Pages
└── artifacts/
    └── mic-monitor/
        └── index.html       # live microphone input level meter
```

Each artifact lives in its own folder under `artifacts/` as a self-contained `index.html` (no build step, no dependencies), so it's reachable at `artifacts/<name>/` once Pages is enabled.

## Adding a new artifact

1. Create `artifacts/<name>/index.html`.
2. Add a link to it from the root `index.html`.
3. Commit and push — GitHub Pages redeploys automatically.

## Live site

Once GitHub Pages is enabled (Settings → Pages → Deploy from branch `main` / root), the site is served at:

`https://<your-username>.github.io/<repo-name>/`
