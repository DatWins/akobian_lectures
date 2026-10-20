# GM Varuzhan Akobian Lectures

A small [Hugo](https://gohugo.io/) site that lists chess lecture videos in seven areas:
Openings, MiddleGame, Endgame, Game Analysis, Tactics, Beginners, Non-Beginners.

## Edit the links

All lecture links live in `data/lectures.json`. Each category has an `items` list with
`number`, `title`, `url` and `duration`. The page is generated from that file, so no template edits are needed.

## Run locally

```
hugo server
```

## Build

```
hugo --minify
```

The output goes to `public/`. Set `baseURL` in `hugo.toml` to your site address before deploying.
