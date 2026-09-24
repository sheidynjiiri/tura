# Tũra Cabins website

Static site for Tũra Cabins: plain HTML, CSS and a little JavaScript. No build step.

## Pages

| Path | File |
| --- | --- |
| `/` | `index.html` (guests: cabins, places, FAQ, waitlist) |
| `/host/` | `host/index.html` (landowner partnership) |
| `/thanks/` | `thanks/index.html` (shown after a form is sent) |
| 404 | `404.html` |

Styles live in `assets/css/styles.css`, scripts in `assets/js/main.js`, images in `assets/img/`.
The illustrations in `assets/img/*.svg` are placeholders: swap them for real photos (same filenames, or update the `src` in the HTML).

## Editing

Open the HTML file, change the text, commit and push to `main`. Netlify redeploys automatically.

To preview locally:

```sh
python3 -m http.server 8000
# then open http://localhost:8000
```

## Forms

The waitlist form (home page) and the landowner form (`/host/`) use [Netlify Forms](https://docs.netlify.com/forms/setup/).
Submissions appear in the Netlify dashboard under **Forms**, where you can also set up email notifications.

## Deploying

`netlify.toml` tells Netlify to publish the repo root as-is. Link the Netlify site to this GitHub repo and every push to `main` goes live.
