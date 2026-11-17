# GTA VI — SK countdown

A standalone Slovak countdown page. It uses plain HTML, CSS, and JavaScript; there is no build step. Keep `favicon.svg`, `tiktok-bg.webp`, `og-preview.jpg`, `affiliate-gta.png`, and `affiliate-vinyl.webp` beside `index.html` when deploying. Trailer embeds load from YouTube, and the other video links point to Rockstar’s official pages.

## Preview locally

Serve the folder over HTTP so the YouTube player receives a page referrer. Opening `index.html` directly as a `file://` URL can produce YouTube Error 153.

From this folder, run:

```powershell
python -m http.server 8000
```

Then open `http://localhost:8000` in your browser. GitHub Pages serves the page over HTTPS, so its embedded players receive the site origin there as well.

## Publish with GitHub Pages

1. Create a GitHub repository and put `index.html` at the repository root.
2. In the repository, open **Settings → Pages**.
3. Choose **Deploy from a branch**, select the branch you publish from, and choose the root folder.
4. After GitHub Pages publishes the site, add your custom domain in the Pages settings and follow GitHub’s DNS instructions at your domain provider.

The launch countdown targets midnight on November 19, 2026 in the Europe/Bratislava time zone. The TikTok panel targets November 18, 2026 at 14:00 in the same time zone. Update those values in `index.html` if the schedule changes.
