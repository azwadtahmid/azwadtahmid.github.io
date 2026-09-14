# azwadtahmid.github.io

Personal portfolio — [azwadtahmid.github.io](https://azwadtahmid.github.io)

A single self-contained `index.html`. No build step, no dependencies beyond the Google Fonts
stylesheet. Edit the file, commit, push — GitHub Pages redeploys automatically.

## Structure

The page is organised as a pipeline — input, process, system, output — with the flagship
project (Synthetiq Redact) rendered as a scroll-driven four-stage apparatus.

- Typography: Archivo (display), Newsreader (body), IBM Plex Mono (data)
- Full light and dark themes, driven by `prefers-color-scheme` and a `data-theme` override
- Motion is progressive: entrance animation only runs when JS is present and
  `prefers-reduced-motion` is not set, so the page is fully readable without either
- Scroll-driven effects use native CSS `animation-timeline`, behind `@supports`

## Local preview

Open `index.html` directly in a browser, or serve it:

```bash
python -m http.server 8000
```

## Custom domain

Add a `CNAME` file containing the bare domain, point a DNS `ALIAS`/`ANAME` record at
`azwadtahmid.github.io`, then enable "Enforce HTTPS" in the repository's Pages settings.
