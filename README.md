# Kasper til Maki

En personlig landingpage til ansøgningen som AI & Automation Specialist hos Maki A/S. Siden er bygget på koden fra hey-kasper.dk (repoet heykasper) med ny tekst, Makis røde farver og Makis logo.

## Mappen

- site/: selve hjemmesiden. Det er kun denne mappe, der kommer online.
  - index.html: forsiden med al teksten
  - 404.html: siden, der vises, hvis adressen er forkert
  - css/styles.css: farver og design. Makis farver står øverst under `:root`.
  - js/main.js: små forbedringer, fx agentvælgeren i toppen og temaknappen
  - assets/maki-logo.svg: Makis logo i rød (#BB252B)
  - assets/og-image.jpg: billedet, der vises, når linket deles på LinkedIn eller i en mail
- netlify.toml: fortæller Netlify, at site/ skal publiceres.

## Linket

Siden ligger på GitHub Pages: https://kasperai-stack.github.io/Maki/

Den bliver opdateret automatisk, hver gang der pushes (se .github/workflows/pages.yml). Første gang skal GitHub Pages slås til én gang: Settings → Pages → Source: "GitHub Actions".

## Se siden på din egen computer

1. Åbn en terminal i mappen.
2. Skriv `npx serve site` og åbn adressen, der vises i terminalen.

## Publicér via Netlify

1. Log ind på netlify.com, vælg "Add new site" og derefter "Import an existing project".
2. Vælg repoet Maki og den gren, siden ligger på. Netlify læser netlify.toml og publicerer site/ automatisk.
3. Når siden er online, så ret `og:image` i toppen af site/index.html til den fulde adresse, fx `https://dit-navn.netlify.app/assets/og-image.jpg`. Ellers viser LinkedIn ikke billedet, når linket deles.

## Godt at vide

- Siden skal ikke kunne findes på Google. Den har `noindex` i HTML'en, i netlify.toml og i robots.txt.
- Der er ingen Google Tag Manager, cookies eller formular på siden. Kontakt sker via Kaspers Google-kalender, mail og telefon.
- Teksten følger Kaspers stemme: dansk, "I" og "jer" til Maki, ingen tankestreger og ingen opdigtede tal.
