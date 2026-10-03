# Website Koninklijke Schaakclub Groeninge Kortrijk

Statische site gebouwd met [Hugo](https://gohugo.io), automatisch gepubliceerd via GitHub Pages.

## Iets wijzigen

1. Open het bestand in `content/` (bv. `content/kalender.md`) en pas de tekst aan (Markdown). Dit kan ook rechtstreeks op github.com via het potlood-icoon.
2. Commit naar `main`. De GitHub Action bouwt en publiceert de site automatisch (±1 minuut).

| Pagina | Bestand | URL |
|---|---|---|
| Home | `content/_index.md` | `/` |
| Kalender | `content/kalender.md` | `/kalender/` |
| Clubkampioenschap | `content/clubkampioenschap.md` | `/clubkampioenschap/` |
| Opleiding | `content/opleiding.md` | `/opleiding/` |
| Lid worden | `content/lid-worden.md` | `/lid-worden/` |
| Contact/Info | `content/contact.md` | `/contact/` |

- Afbeeldingen: zet ze in `static/images/` (liefst < 1500 px breed) en verwijs ernaar met `/images/naam.jpg`.
- Menu, adres, telefoon, formulier-URL's: `hugo.toml`.
- De oude URL's (`/galerij`, `/teamschema`, `/sponsors`, `/lidworden`) sturen automatisch door via `aliases` in de front matter.

## Lokaal bekijken

    hugo server

## Formulieren

GitHub Pages heeft geen server. De formulieren (contact, lid worden) werken via [Formspree](https://formspree.io): maak een formulier aan, plak de URL in `contactFormEndpoint` / `memberFormEndpoint` in `hugo.toml`. Zolang die leeg zijn, worden de formulieren verborgen.

## Domein

`static/CNAME` bevat `www.schaakclubkortrijk.be`. Zie de GitHub Pages-instellingen van de repo voor de DNS-instructies.
