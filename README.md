# Tab Light — beta website

Tab Light is a single-file, responsive HTML prototype for thematic Qur’an study and research literacy. This release uses `index.html` from the supplied Downloads file. It is a front-end demo; do not use it for fatwa or as a verified academic database.

## GitHub Pages

1. In GitHub, create a repository named `tab-light`.
2. Upload `index.html` and commit it to the `main` branch.
3. Open **Settings → Pages**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
4. Wait for GitHub Pages to finish publishing; its public URL will appear in Settings → Pages.

## Beta limitations

- The Zayed backend is not included in this static website release. GitHub Pages cannot run the Node/Express server. Deploy it separately to an HTTPS host and configure its CORS allowlist before connecting it.
- No API key, account registration, or admin credentials should be added to this repository.
- Sample Qur’an/tafsir references, journal indexing, prayer data, and language labels require expert and source verification before public educational use.
- A public repository and Pages site can be viewed by anyone with the link. Do not collect sensitive test data.
