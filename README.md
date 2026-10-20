# GM Varuzhan Akobian Lectures

A one-page [Hugo](https://gohugo.io/) site (theme: [hugo-scroll](https://github.com/zjedi/hugo-scroll), same as the essentiallinks sample)
listing chess lecture videos in seven areas: Openings, Middlegame, Endgame, Game Analysis, Tactics, Beginners, Non-Beginners.

- Side menu on desktop, sticky scrolling menu on phones and tablets.
- Each area is one file in `content/en/homepage/` (`01-openings.md` ... `07-non-beginners.md`). Add a lecture by adding a `- [Title - 12:34](https://youtube.com/...)` line.
- Cover text and picture: `content/en/_index.md` and `assets/images/cover-image.jpg`.
- Style tweaks: `layouts/partials/custom_head.html`.

## Run locally

Needs Hugo **extended** 0.147 or newer. Clone with submodules (the theme is a submodule):

```
git clone --recurse-submodules https://github.com/DatWins/akobian_lectures
cd akobian_lectures
hugo server
```

## Deploy

Pushing to `main` publishes to GitHub Pages through `.github/workflows/hugo.yaml`.
In the repo's Settings → Pages, set the source to "GitHub Actions".
