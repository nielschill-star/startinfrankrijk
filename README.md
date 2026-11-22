# startinfrankrijk.nl

Wegwijzer voor Nederlanders die naar Frankrijk verhuizen, met focus op gîtes. Statische site (Astro), gehost op Cloudflare Workers (static assets). Plan en bronnen staan in het Claude-project "Website emigreren".

## Lokaal

```
npm install
npm run dev      # http://localhost:4321
npm run build    # bouwt naar dist/
```

## Inhoud

- Elke pagina staat in `src/pages/`. Pagina's met `draft` zijn nog in uitwerking en staan op `noindex`.
- Regels, drempels en bedragen alleen uit officiële bronnen. Zet bij elke wijziging de datum "laatst gecontroleerd" (`lastChecked`) bij.
- Verwijderen van `draft` pas als de pagina is gecontroleerd.

## Linkcontrole

`.github/workflows/linkcheck.yml` draait elke 1e van de maand en maakt een GitHub-issue met stuk gaande links. Hij test alleen of links werken, niet of de inhoud nog klopt. Gîte-artikelen elk halfjaar inhoudelijk nalopen.

## Openstaand voor livegang

- `src/pages/mentions-legales.astro`: uitgevergegevens invullen (staan als placeholder).
- Hostingadres van Cloudflare op de mentions-pagina staat uit het hoofd en moet nog worden gecontroleerd.
- Contactformulier kiezen (`src/pages/contact.astro`).
- "Over"-pagina: persoonlijk verhaal.
- Draft-pagina's afwerken (zie `claude/bronnen-golf-1.md` in het project).
- Cloudflare koppelen: Workers (Git-koppeling), custom domain startinfrankrijk.nl.
