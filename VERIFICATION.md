# Portfolio 1.0.0 — verifica

6 novembre 2026. Sito statico HTML/CSS; non modifica Pause né altri progetti.

- Chromium a 1440, 768, 390 e 320 px, con movimento ridotto: nessun overflow orizzontale o errore JavaScript. Immagini decodificate e font locale caricati.
- Link di navigazione Progetti/Chi sono/Contatti, skip link da tastiera, ritorno dalla pagina novità e versione 1.0.0 verificati.
- Nessuna richiesta esterna al caricamento: immagini/font locali, nessun iframe, analytics o script runtime. I link esterni portano ai siti reali quando scelti dal visitatore.
- Sei destinazioni pubbliche verificate HTTP 200: florame.ai, Pause, Parola, Fiori e Piante di Nino, 17/19 Urban Bistrot, Al Jariri.
- Un solo h1 per pagina, frammenti interni, alt e dimensioni immagini, asset locali e 7 hash di provenienza verificati. Il controllo strutturale non equivale a una certificazione WCAG completa.
- Revisione visiva indipendente: **ship**, nessuna correzione materiale richiesta, su tutte e quattro le larghezze. CEO di florame.ai immediatamente leggibile, progetto principale dominante, anteprime reali e gerarchia coerente.
- Detector: testi 10/11px portati a 12px. Avviso di inset sulla fascia About è un falso positivo: il contenitore wrap interno mantiene 20px su mobile e 120px a 1440. Nessun secondo detector eseguito.
- Tutti i 7 raster hanno origine incorporata oppure sidecar supportato dal tool; scansione senza asset mancanti. Nessun testo, contatore o contenuto dei siti catturati è stato sostituito.
- Il vecchio contenuto bistrot e il file HTML erroneamente chiamato workflow vengono rimossi dal sito corrente, conservandone la cronologia Git.

## Pubblicazione verificata

- Commit del portfolio: `4dd7b37`. Pages da main:/docs, HTTPS enforced, build completata.
- Homepage HTTPS HTTP 200 con il portfolio corretto. Quindici pagine/asset pubblici corrispondono ai locali, con sola normalizzazione CRLF/LF per il testo e confronto esatto dei binari.
- Ripetuti sul sito pubblico tutti i controlli browser a 1440/768/390/320 px: nessun overflow, errore JavaScript o richiesta esterna; navigazione, tastiera, immagini e novità funzionanti.
- Le rotte indipendenti /Pause/ e /parola/ restano HTTP 200 e mostrano i rispettivi prodotti.
- Il cambio sorgente Pages da radice a docs richiede una build successiva alla configurazione: la prima build, partita dal push precedente, mostrava il README dalla vecchia sorgente. Richiesta una build dalla configurazione corretta e verificato il risultato prima di dichiararlo online.

Nessun nome completo, recapito personale o ruolo aggiuntivo inventato.
