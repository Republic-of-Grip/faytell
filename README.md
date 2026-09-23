# Faytell

Faytell is a summonable public window for chosen content. Thor decides what appears. Anyone with the URL can look. The link is shared only when he chooses to share it.

**GitHub** is the workshop: source, coordination, contribution. **GitHub Pages** is the only public window.

This is not an open generator. V0 is an empty stage and a pattern for adding pages later. Nothing on the site is sample subject matter.

Ambient listening — a page that writes itself from conversation — is a later aspiration. It is not built here.

## Public site

https://republic-of-grip.github.io/faytell/

Home explains the window. The unsummoned pattern lives at:

https://republic-of-grip.github.io/faytell/s/example/

## Local preview

From this directory:

```bash
python3 -m http.server 8080
```

Open http://127.0.0.1:8080/

## Add a summon page

1. Copy `s/example/` to `s/<slug>/`. Use a short, stable slug. Leave `s/example/` empty — it is the pattern, not a draft slot.
2. Replace the awaiting-summon copy with the chosen content. Keep the shared chrome: `assets/site.css` and the frame markup.
3. Commit to `main` and push.
4. The public URL is `https://republic-of-grip.github.io/faytell/s/<slug>/`.
5. Share that URL only when you mean to. Pushing publishes it.

Pages is served from the `main` branch at `/` (repository root). A `.nojekyll` file keeps the static files unprocessed.

## License

[MIT](LICENSE). The typefaces in `assets/fonts/` are Instrument Serif and Instrument Sans, under the SIL Open Font License (`assets/fonts/OFL-serif.txt`, `assets/fonts/OFL-sans.txt`).