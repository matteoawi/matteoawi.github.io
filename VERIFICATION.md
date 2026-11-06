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

La pubblicazione GitHub Pages e la verifica HTTPS saranno registrate dopo l’effettivo deployment. Nessun nome completo, recapito personale o ruolo aggiuntivo inventato.
