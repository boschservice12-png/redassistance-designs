# Modul Sezonier Roți — Landing Page

**Slug:** `sezonier-roti`
**Verzió:** v1
**Élő URL:** https://boschservice12-png.github.io/redassistance-designs/live/sezonier-roti/

## Cél

Üzletszerzési landing oldal a RedAssistance Modul Sezonier Roți modulhoz. Célközönség: román szerviz-tulajdonosok és recepcionisok, akik szezonális kerékcserét és kerékraktározást kezelnek.

## Üzleti üzenet

> "Planifică sezonul. Nu atinge istoricul."

Pozicionálás: ez NEM helyettesít semmit a meglévő RPW workflow-ban — kiegészíti. Külön modul, ugyanaz a VIN- és ügyfél-adatbázis.

## Tartalmi struktúra

1. **Hero** — főüzenet + 2 CTA (implementare + flux)
2. **Problémák (4 db)** — fájdalompontok a szerviz napi gyakorlatából
3. **Caracteristici (6 db)** — modul-funkciók kártyákban
4. **Cum funcționează (4 lépés)** — recepție → stocare → sezon → predare
5. **Integrare RedAssistance** — VIN-koherencia kód-snippet stílusban
6. **CTA záró** — 14 nap implementáció
7. **Footer** — copyright + design verzió

## Konverziós pontok

- **Primary CTA:** `mailto:ferenc@redassistance.net` — implementáció érdeklődéshez
- **Secondary CTA:** demo érdeklődés (jelenleg `#` placeholder, később bekötendő Calendly-re vagy más booking link-re)

## Technikai

- Single HTML fájl, **self-contained**
- Inline CSS és inline SVG (logo + 6 ikon)
- Külső függőség: Geist + Geist Mono Google Fonts CDN-ről
- Mobile breakpoint-ok: 920px (tablet), 560px (mobile)
- Méret: ~14 KB unminified

## Módosítási útmutató

- A brand szín csere a `:root { --ra-red: ... }` változón keresztül megy — automatikusan minden komponens átveszi
- Új feature-kártya: másold a `.ra-feature` div blokkját, cseréld a SVG ikont és a szöveget
- Új lépés: másold a `.ra-step` blokkot, frissítsd a `.ra-steps` `grid-template-columns` értékét
- A 7. lépésnél (CTA) a `mailto:` link a tényleges e-mail-re mutasson, és NE hagyd a `#` placeholder-en a demo CTA-t

## Verziók

| Verzió | Dátum | Változás |
|---|---|---|
| v1 | 2026-05-22 | Initial release |
