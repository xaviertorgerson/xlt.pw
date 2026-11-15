# xlt.pw

Xavier Torgerson's personal site and writing, served by GitHub Pages from this repo (`CNAME` is
`xlt.pw`; Cloudflare sits in front). Plain HTML and one stylesheet, nothing to build.

## Add a post

1. Copy `writing/_post-template.html` to `writing/<slug>.html` and fill in the capitals.
2. Add it, newest first, to the lists in `index.html` and `writing/index.html` (replace the "Nothing
   posted yet" line the first time), and as an `<entry>` in `feed.xml`; set the feed's `<updated>`.
3. Commit and push. Pages publishes in about a minute.

## What used to be here

Until 2026-11-15, xlt.pw hosted the Handshake landing page proof of concept, its demo screens, an
earlier "ProLink" draft and an old Variadic Group pitch. They are kept, not lost:

- the Handshake pages: the private `Handshake` repo, branch `docs/landing-poc`, `docs/landing-poc/`;
- the pitch: the private `variadic-group` repo, `docs/archive/`;
- all of them: this repo's history (`git log --diff-filter=D --stat`).

`storytelling.html` (The Architecture of Story) stays at its address.

The display face is Funnel Display, self-hosted under the SIL Open Font License (`fonts/`).
