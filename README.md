# Populate the Stars – Promo-Seite

Statische Seite zum Spiel ([../sol](../sol)). Kein Build, keine Cookies, kein Tracking. CSS, JavaScript und Schrift stehen inline im HTML, separat liegen nur Bilder.

Live: <https://ithie.github.io/populate-the-stars-promo/> – Deploy per GitHub Actions bei jedem Push auf `main` ([deploy.yml](.github/workflows/deploy.yml)).

| Datei | Inhalt |
| --- | --- |
| `index.html` | Promo-Seite |
| `legal.html` | Impressum + Datenschutz, `?lang=de` · `en` · `fr` · `es` · `pt` · `pt-BR` (sonst Browsersprache) |
| `assets/` | Icon, App-Store-Badge |
| `screenshots/` | Screenshots, eingetragen in `SCREENSHOTS` in `index.html` |

## Generierte Teile

Aus dem Spiel erzeugt, nicht von Hand ändern. Im Spiel-Ordner:

```sh
npm run export:legal   # Rechtstexte → legal.html (legal-texts:begin/end)
npm run export:sky     # Sonnensystem-Animation → index.html (sky:begin/end)
```
