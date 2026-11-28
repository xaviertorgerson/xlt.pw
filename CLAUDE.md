# xlt.pw

This repo is a hosting mechanism, not a place where projects are documented.

- Each project lives in its own repo, and that repo's README is where the project describes itself:
  what it is, why it exists, how it works, and how to publish it to `xlt.pw`.
- A project folder in this repo (`downtown-101/`, `murmuration/`, `shadowlite/`) is a published copy
  of files from the project's repo. Do not edit the copy here; change the project's repo and copy
  the files over.
- When adding a project, add its folder, one line in the Projects list in `index.html`, its address in
  `sitemap.xml` and one line in `llms.txt`. Do not add a section about it to this repo's `README.md`.
- This README covers only the site itself: how it is served and how to add a post.
- Every page can be found: a title that says what it is, a description, a canonical address, link-preview
  tags with an image (`og.png` when the page has none of its own), and a line in `sitemap.xml` and
  `llms.txt`. A page whose content is drawn by a script also carries that content as plain HTML.
- Every page leads home: a project page credits Xavier Torgerson with a link to `https://xlt.pw`, and the
  home page links to every project and to Variadic Group (`https://variadicgroup.com`), which links back.
- A project is published at one address. If it moves to its own domain, its folder here goes and the
  Projects list links to the new address.
- Nothing on the site is invented: no made-up numbers, testimonials or claims. No trackers or ads.
- Changes go in on a branch through a pull request to `main`. GitHub Pages publishes `main`.
