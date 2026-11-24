# Demo sito, Geom. Claudio Babini (Ravenna)

Demo vetrina realizzata da Zenith Studio per un prospect: studio tecnico di un
geometra a Ravenna. Sito statico, pronto per GitHub Pages.

## File

- `index.html` : la pagina (una sola)
- `style.css` : stile
- `script.js` : menu mobile e comparse allo scroll
- `img/` : immagini (`hero.webp` e' una foto stock, da sostituire)
- `DESIGN.md` : direzione visiva
- `CNAME` : dominio di pubblicazione (ora `babini.zenith-studio.it`)

## Come vederlo in locale

Apri `index.html` nel browser, oppure:

```bash
python3 -m http.server 8000
# poi apri http://localhost:8000
```

## Pubblicazione (GitHub Pages)

Carica i file nella root del branch e attiva Pages (Settings, Pages, branch).
Il `CNAME` punta a `babini.zenith-studio.it`: cambialo o rimuovilo se usi un
altro dominio. In quel caso aggiorna anche i meta `canonical` e `og:*` in
`index.html`.

## IMPORTANTE: dati da confermare prima di andare online

Nessun dato reale di Babini era disponibile. Tutto cio' che e' segnato
"da verificare" nel sito va confermato con il cliente e sostituito in
`index.html`:

- Telefono, WhatsApp, email (ora segnaposto `0544 000000`, `347 000000`,
  `info@example.it` con link `tel:` e `wa.me` fittizi)
- Indirizzo della sede e orari di apertura
- P.IVA e numero di iscrizione al Collegio Geometri di Ravenna
- Anni di attivita'
- Elenco dei comuni serviti (ora indicativo: Ravenna, Cervia, Russi,
  Bagnacavallo, Lugo, Faenza)
- Elenco esatto dei servizi con le parole del cliente

## Immagini da sostituire

- `img/hero.webp` : foto stock (persona che disegna tavole tecniche). Va
  sostituita con una foto reale dello studio o del geometra al lavoro.

La mappa in "Dove lavoro" e' centrata su Ravenna: va ricentrata sull'indirizzo
reale una volta noto.
