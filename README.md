# xlt.pw

Xavier Torgerson's personal site and writing, served by GitHub Pages from this repo (`CNAME` is
`xlt.pw`; Cloudflare sits in front). Plain HTML and one stylesheet, nothing to build.

## Hosted projects

This repo is only the mechanism that puts projects on `xlt.pw`. A project folder here (for example
`downtown-101/`) is a published copy of files from that project's own repo. The project's repo is
where it is developed and where it describes itself: what it is, why it exists, how to run it and
how to publish it. New projects get a folder and a line in the Projects list on the home page, and
nothing in this README.

## Being found

`robots.txt` allows everything and names `sitemap.xml`. `sitemap.xml` lists every page; `llms.txt` is
the same map in prose for AI assistants. A new page or post goes in both. `og.png` is the link preview
for the home page and any page without its own.

## Add a post

1. Copy `writing/_post-template.html` to `writing/<slug>.html` and fill in the capitals.
2. Add it, newest first, to the lists in `index.html` and `writing/index.html` (replace the "Nothing
   posted yet" line the first time), and as an `<entry>` in `feed.xml`; set the feed's `<updated>`.
3. Commit and push. Pages publishes in about a minute.

## Murmuration

`murmuration/` is a copy of two files, `index.html` and `og.png`, from the public
[`murmuration`](https://github.com/xaviertorgerson/murmuration) repo, which is where the page is
developed. Don't edit the copy here. To bring it up to date after that repo changes:

```sh
cp ../murmuration/index.html ../murmuration/og.png murmuration/
git add murmuration && git commit -m "murmuration: sync with the murmuration repo" && git push
```

The page's canonical address, and the address in its link preview, is `https://xlt.pw/murmuration/`.

## Shadowlite

`shadowlite/` is a copy of two files from the private
[`shadowlite`](https://github.com/xaviertorgerson/shadowlite) repo, which is where the game is
developed: `index.html` (that repo's built `dist/index.html`, the whole game in one file) and
`og.png`. Don't edit the copy here. To bring it up to date after that repo changes:

```sh
(cd ../shadowlite && npm run build)
cp ../shadowlite/dist/index.html ../shadowlite/og.png shadowlite/
git add shadowlite && git commit -m "shadowlite: sync with the shadowlite repo" && git push
```

The page's canonical address, and the address in its link preview, is `https://xlt.pw/shadowlite/`.

## What used to be here

Until 2026-11-15, xlt.pw hosted the Handshake landing page proof of concept, its demo screens, an
earlier "ProLink" draft and an old Variadic Group pitch. They are kept, not lost:

- the Handshake pages: the private `Handshake` repo, branch `docs/landing-poc`, `docs/landing-poc/`;
- the pitch: the private `variadic-group` repo, `docs/archive/`;
- all of them: this repo's history (`git log --diff-filter=D --stat`).

`storytelling.html` (The Architecture of Story) stays at its address.

The display face is Funnel Display, self-hosted under the SIL Open Font License (`fonts/`).
