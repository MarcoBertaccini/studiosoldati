# DESIGN.md — Geom. Claudio Babini, Ravenna

Direzione visiva della demo. Principi presi nello spirito di un buon sito per
studi tecnici (il riferimento geometranet.it non era raggiungibile), non un clone.
Gerarchia: regole della skill demo-sito-cliente > questo file > altre skill.

## Soggetto e obiettivo
Studio tecnico di un geometra a Ravenna. Pubblico: privati e piccole imprese del
territorio che hanno bisogno di pratiche concrete (catasto, edilizia, APE,
successioni). Lavoro primario della pagina: **far telefonare**. Tono: competente,
locale, diretto, senza fronzoli.

## Colore (palette base)
- `--paper`  #F3F2EE  fondo pietra chiaro, freddo quanto basta (NON il cream cliché)
- `--ink`    #1C2A30  ardesia profonda, testo principale e fasce scure
- `--slate`  #5E6A70  testo secondario
- `--line`   #D9D4C8  filetti e bordi, sabbia tenue
- `--green`  #1F6B52  accento unico (territorio/topografia): bottoni, link, dettagli
- `--green-d`#184F3E  verde hover
Un solo accento. Nessun gradiente decorativo, nessun glow.

## Tipografia (2 famiglie, Google Fonts)
- **Fraunces** (serif): titoli e numeri di sezione. Peso 500/600, carattere caldo
  ma serio. Usata come elemento visivo, non solo contenitore.
- **Hanken Grotesk** (sans): corpo, navigazione, bottoni, etichette. Molto leggibile
  (pubblico anche non giovane).
Scala tipografica definita, interlinea generosa sul corpo, misura < 70 caratteri.
Niente maiuscolo tracciato come eyebrow sopra ogni sezione.

## Layout
Editoriale, allineato a sinistra, margini ampi, ogni sezione impaginata in modo
diverso dalla precedente (mai tre griglie di card identiche di fila).

```
HEADER sticky:  [Geom. Babini]                 [nav]        [ Chiama ora ]
HERO split:     | titolo + cosa fa + zona |   | foto tecnica inquadrata |
                | CTA telefono + whatsapp |
SERVIZI 2x2:    quattro aree con pratiche reali elencate come testo (no pill-tag)
METODO:         1 --- 2 --- 3 --- 4  (sequenza reale: marker numerati ammessi)
CHI E':         blocco-dichiarazione + dati chiave [DA VERIFICARE]
ZONA (fascia scura): elenco comuni + mappa
CONTATTI (scura): telefono grande + whatsapp + email + orari + indirizzo + mappa
FOOTER:         nome, P.IVA, Albo, privacy
```

## Movimento
Un solo momento d'ingresso leggero sulla hero. Fade/rise discreto sugli header di
sezione (non su ogni elemento). Hover su bottoni e link. `prefers-reduced-motion`
rispettato. Nessuna animazione gratuita.

## Immagini
Una sola fotografia forte nella hero (persona che disegna tavole tecniche con lo
scalimetro: strumento da geometra). Stock, da sostituire con foto reali dello
studio. Nessuna persona stock spacciata per Babini o per il team. Il resto della
pagina vive di tipografia, spazio e dettagli geometrici in CSS.

## Scrittura
Italiano concreto e locale. Niente trattini lungo/medio nel testo. Niente strutture
da AI ne' parole vuote. Le CTA dicono cosa fanno ("Chiama lo studio"). Tutto cio'
che non e' confermato e' marcato [DA VERIFICARE] in modo visibile.
