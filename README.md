# Faros – Netlify/GitHub prosjekt (Final baseline 2025-08-26)

Dette er en **ryddet baseline** etter flere iterasjoner. Den er laget for at vi enkelt kan jobbe videre i **GitHub** og få **autodeploy** i Netlify – uten zip-dans.

## ✅ Hva som er bra (fra tidligere versjoner)
- **Struktur**: enkel landingsside med seksjoner (Hero → Verdier → Founder → Caser → CTA → Kontakt → Footer)
- **Responsiv**: grid-stacking på mobil (knapper ligger side‑om‑side og “stacker” med `gap`)
- **Kontaktskjema**: Netlify Forms er aktivert (se `<form name="kontakt" ...>`)
- **Fargepalett**: balansert (blå trygghet, turkis fremdrift, varm sand, peach-aksent)
- **“Om meg” tydelig**: rørlegger + selger/markedsfører + håndverker løftes i hero og i egen seksjon
- **Ingen skeiv topplinje**: fjernet problematisk header/meny inntil vi har en bedre

## ❗Hva som ikke var bra (og er fikset/parkert)
- **Knapper oppå hverandre** → nå løst med `display:flex; flex-wrap:wrap; gap:12px;`
- **For maskulint uttrykk** → varmet med `--sand` og `--peach` (uten å miste seriøsitet)
- **Skeiv nav/meny** → fjernet for nå (kommer tilbake med bedre layout senere)
- **Spredte tekster** → samlet og strammet opp copy (tydelig verdiforslag)

## 🔧 Hvordan jobbe videre (GitHub → Netlify)
1. Endre tekst i `index.html`. Farger/typografi i `styles.css` (variabler øverst).
2. Commit til GitHub → Netlify deployer automatisk.
3. Bytt case-bilder ved å legge inn `<img src="/assets/bilde.jpg" alt="">` i stedet for `.case__thumb`.

## 🧩 TODO (neste små forbedringer)
- [ ] Legge til **/takk**-side for skjema (Netlify redirect)
- [ ] Legge inn ekte bilder (casedelen)
- [ ] Lage enkel **header** med logo + “Book en prat” (mobil-sikker)
- [ ] Fikse favicon/logo til endelig versjon
- [ ] Legge inn schema.org (LocalBusiness) for bedre SEO

## 🎨 Palett
```css
--blue:#0B2E59;       /* trygghet */
--turquoise:#00B4D8;  /* fremdrift */
--sand:#F7E9D7;       /* varme */
--peach:#FF8FA3;      /* vennlig aksent */
--hero:#F4FBFF;
--text:#1a2433;
--muted:#5b6b7a;
```

## 📝 Changelog (kort)
- Final baseline: knappelayout, om‑meg copy, balansert palett, fjernet skeiv header.
