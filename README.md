# Studio Tecnico Soldati — Landing page

Landing page one-page per lo Studio Tecnico Soldati (Rimini). Progettazione
architettonica e strutturale, sismica, impiantistica, catasti e urbanistica.

Sito **statico self-contained**: un unico file `index.html` con CSS e JS inline.
Nessun build, nessuna dipendenza da installare. I font arrivano da Google Fonts,
l'unica risorsa esterna oltre alla foto della hero.

## Come vederlo

Apri `index.html` con un doppio click nel browser, oppure servi la cartella:

```bash
python3 -m http.server 8000
# poi apri http://localhost:8000
```

## Come pubblicarlo

Essendo statico, va ovunque: GitHub Pages, Netlify, Vercel, o un qualsiasi
hosting che serve file. Basta caricare `index.html` (più eventuali immagini).
Per GitHub Pages: Settings → Pages → deploy dal branch, cartella `/root`.

## Cosa personalizzare

- **Foto della hero** — attualmente è un placeholder da Unsplash. Cerca
  `id="heroPhoto"` in `index.html` e cambia il `src`, oppure metti un file
  locale (es. `hero.jpg`) accanto all'`index.html` e usa `src="hero.jpg"`.
  Se l'immagine non carica, la hero resta comunque leggibile grazie a uno
  sfondo di fallback.
- **P.IVA** — segnaposto `00000000000` nel footer, da sostituire con quella reale.
- **Foto reali / logo dello studio** — quando disponibili, si possono inserire
  nelle sezioni "Studio" e nell'header.
- **Contenuti** — tutti i testi sono nel body dell'`index.html`, in italiano,
  facilmente modificabili.

## Dati dello studio (contenuti nel sito)

- Indirizzo: Vicolo San Gregorio, 22 — 47923 Rimini (RN)
- Telefono: 0541 781314 / 347 2516802
- Email: architetto_9@libero.it
- Orari: Lun–Ven 09:00–13:00 e 15:00–19:00 · Sab–Dom chiuso
- Professionisti: Arch. Paolo Soldati · Ing. Massimiliano Soldati

## Note tecniche

- Design "tecnico/blueprint": griglia modulare, tipografia Archivo + IBM Plex
  Sans/Mono, palette ink navy + carta calda + accento arancio.
- Animazioni allo scroll con `IntersectionObserver`, scroll-progress e parallax.
- Supporto tema chiaro/scuro (segue le preferenze di sistema).
- Rispetta `prefers-reduced-motion` e le regole base di accessibilità.
- Responsive fino a ~360px di larghezza.
