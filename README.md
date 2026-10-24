# Faytell

A window for what a comment field can't hold.

When I'm part of a conversation somewhere else, like a newspaper's comment section or a forum thread, the format often allows only plain text. Faytell is where the rest goes: a picture, a film, an infographic or a longer line of reasoning. Each page holds one thought, carries a date and links back to the conversation it belongs to. I post the link there.

Nothing here is generated. Every page is put up by hand, on purpose.

- **Site:** https://republic-of-grip.github.io/faytell/
- **Page template:** https://republic-of-grip.github.io/faytell/s/example/

## Add a page

1. Copy `s/example/` to `s/<slug>/`. Use a short, lowercase name with hyphens, e.g. `s/heat-pumps/`.
2. Open `s/<slug>/index.html` and replace the "Your ..." placeholders. Delete any blocks you don't need: image, video, quote, sources.
3. Put the page's images and videos in the same folder.
4. Fill in the `og:` lines at the top. They decide how the link looks when pasted into a comment field or chat.
5. Delete the `robots` line, which is only there to keep the template out of search engines.
6. Commit and push to `main`. The page is live at `https://republic-of-grip.github.io/faytell/s/<slug>/` a minute or two later.

Keep drafts in `drafts/`. Git ignores that folder, so drafts never get published.

## Before you push

- **Pushing to `main` publishes.** The repository is public, so a pushed page can be found even if you never share its link.
- **Deleting a page doesn't erase it.** It disappears from the site, but stays in the repository's history. Only push what you're fine with being public for good.
- **If bots help write pages,** let them open a pull request and merge it yourself. A branch protection rule on `main` can enforce that.

## Preview locally

```bash
python3 -m http.server 8080
```

Then open http://127.0.0.1:8080/. The 404 page uses `/faytell/` paths, so it only looks right on the live site.

Pages is served from the `main` branch, repository root. The `.nojekyll` file tells GitHub to serve the files as they are.

## License

[MIT](LICENSE). The typefaces in `assets/fonts/` are Instrument Serif and Instrument Sans, under the SIL Open Font License (`assets/fonts/OFL-serif.txt`, `assets/fonts/OFL-sans.txt`).
