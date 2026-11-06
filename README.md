# Matteo — personal portfolio

[Visit matteoawi.github.io](https://matteoawi.github.io/)

A personal portfolio featuring Matteo as CEO of florame.ai, followed by his public products, apps and websites. The product is public; its private source is not exposed.

## Current version

**1.2.0**, November 6, 2026. [Changelog](CHANGELOG.md).

## Website

The entire public site is in `docs/`. GitHub Pages serves **main:/docs**. HTML and CSS only, no application framework, build step, analytics, remote fonts or embedded websites. Outbound links open external products; GitHub hosting processes normal connection logs.

```powershell
python -m http.server 8772 --bind 127.0.0.1 --directory docs
```

Open http://127.0.0.1:8772/. The `VERSION`, changelogs and visible footer version move together when the portfolio changes.

## Content and assets

- Identity: Matteo, CEO of florame.ai. No surname, email, location or LinkedIn is inferred.
- Featured products: florame.ai, Pause and Parola.
- Websites: Fiori e Piante di Nino, 17/19 Urban Bistrot and Al Jariri Language & Culture.
- Previews are captures of the actual public websites, resized without changing page content or counts. Sources, capture timestamps and hashes are in [asset provenance](docs/assets/provenance.json).
- Onest is hosted locally with its SIL OFL license in `docs/assets/fonts/OFL.txt`.
- The monogram is original geometric SVG. Preview images and project names belong to their respective owners; their presence does not grant rights to the underlying brands or websites.

The previous unrelated bistrot page and an HTML file incorrectly placed under `.github/workflows/static.yml` were retired. Their history is preserved in Git. The real bistrot website stays at its own domain. Other project repositories and deployments are not modified.

## Updating

Fetch and merge `origin/main` before publishing; preserve work from other computers, never force push. Work in a `codex/` branch when useful, verify desktop/mobile, keyboard and real outbound links, update version/changelog, then commit and push to main. Site publication is independent from Android releases.

Product truth is in `PRODUCT.md`; visual tokens and components are documented in `DESIGN.md`. Verification records belong in `VERIFICATION.md`. The development-only direction brief stays outside the deployed docs folder.

If the Pages source folder changes, request a fresh Pages build after saving the new source. Verify the deployed root shows the actual portfolio HTML, rather than the README fallback from an earlier root build. Normal updates keep main:/docs unchanged.
