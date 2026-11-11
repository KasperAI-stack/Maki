# Kasper til BoligPortal

En personlig landingpage til ansøgningen som Digital Marketing Team Lead hos BoligPortal. Forsiden er bygget på koden fra Klean-siden (repoet Klean), som bygger på hey-kasper.dk, med ny tekst, BoligPortals orange (#FF6633) og BoligPortals logo. Forsiden bruger Geist og Instrument Serif ligesom de andre ansøgningssider, og CV og ansøgning bruger Figtree ligesom PDF'erne.

## Mappen

- site/: selve hjemmesiden. Det er kun denne mappe, der kommer online.
  - index.html: forsiden med al teksten, i samme opbygning som Klean: hero med agentvælgeren, problemet (flowet med "Byg motoren ind"), værktøjer, sådan vil jeg arbejde (90-dagesplanen), om mig, det har jeg bygget (med HeyOtto Studio og Tasks), citat, FAQ og kontakt.
  - cv.html og ansoegning.html: CV'et og ansøgningen bygget op som PDF'erne i assets/pdf/. Ret teksten begge steder.
  - 404.html: siden, der vises, hvis adressen er forkert
  - css/styles.css: farver og design. Farverne står øverst under `:root`.
  - js/main.js: små forbedringer, fx agentvælgeren i toppen og temaknappen
  - assets/boligportal-logo.svg: BoligPortals logo
  - assets/og-image.jpg: billedet, der vises, når linket deles på LinkedIn eller i en mail
  - assets/dokument/: Kaspers foto og skærmbillederne af HeyOtto
- netlify.toml: fortæller Netlify, at site/ skal publiceres, hvis siden en dag skal ligge dér.

## Linket

Siden ligger på GitHub Pages: https://kasperai-stack.github.io/boligportalen/ (repoets navn). CV'et og ansøgningen linker til https://kasperai-stack.github.io/boligportal/, så enten skal repoet omdøbes til boligportal, eller linket i PDF'erne skal rettes. Workflowet finder selv repoets navn.

Den bliver opdateret automatisk, hver gang der pushes (se .github/workflows/pages.yml). Første gang skal GitHub Pages slås til én gang: Settings → Pages → Source: "GitHub Actions".

## Se siden på din egen computer

1. Åbn en terminal i mappen.
2. Skriv `npx serve site` og åbn adressen, der vises i terminalen.

## Godt at vide

- Siden skal ikke kunne findes på Google. Den har `noindex` i HTML'en, i netlify.toml og i robots.txt.
- Der er ingen Google Tag Manager, cookies eller formular på siden. Kontakt sker via "Kald til samtale" (mail til kasmussen80@gmail.com) og telefon.
- Teksten følger Kaspers stemme og briefen: dansk, "I" og "jer" til BoligPortal, ingen tankestreger, kun tal fra afsnittet Beviser og intet om, at agenterne kører hos BoligPortal i dag.
- Tekst på orange er mørk (#2B2A35), fordi hvid tekst på BoligPortals orange er for svag at læse.
