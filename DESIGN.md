---
name: Portfolio di Matteo
description: Una raccolta personale di app e siti pubblici da provare.
colors:
  paper: "#eaf1f7"
  ink: "#183c43"
  muted: "#4b626c"
  blue: "#284bd4"
  rule: "#bdcdd5"
  mint: "#dcebd0"
  green: "#193f33"
  white: "#fff"
  primary-hover: "#1a39ab"
  round-hover: "#2e5b49"
  about-heading: "#eff6ec"
  about-copy: "#d7e5d8"
  arrow-surface: "#dae5ee"
typography:
  display:
    fontFamily: "Onest, ui-sans-serif, system-ui, sans-serif"
    fontSize: "clamp(42px, 6.7vw, 88px)"
    fontWeight: 500
    lineHeight: 1.07
    letterSpacing: "-0.04em"
  headline:
    fontFamily: "Onest, ui-sans-serif, system-ui, sans-serif"
    fontSize: "clamp(29px, 3.8vw, 46px)"
    fontWeight: 500
    lineHeight: 1.07
    letterSpacing: "-0.04em"
  title:
    fontFamily: "Onest, ui-sans-serif, system-ui, sans-serif"
    fontSize: "30px"
    fontWeight: 600
    lineHeight: 1.1
    letterSpacing: "-0.035em"
  body:
    fontFamily: "Onest, ui-sans-serif, system-ui, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "Onest, ui-sans-serif, system-ui, sans-serif"
    fontSize: "14px"
    fontWeight: 500
    lineHeight: 1.6
rounded:
  mount: "16px"
  control: "10px"
  mobile-product: "12px"
  circle: "50%"
spacing:
  page-inset: "clamp(20px, 4.5vw, 64px)"
  columns: "36px"
  tablet-columns: "24px"
  section: "99px"
  tablet-section: "74px"
  mobile-section: "61px"
components:
  button-primary:
    backgroundColor: "{colors.blue}"
    textColor: "{colors.white}"
    rounded: "{rounded.control}"
    padding: "16px 23px"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.white}"
  text-link:
    textColor: "{colors.ink}"
    typography: "{typography.label}"
  round-link:
    backgroundColor: "{colors.green}"
    textColor: "{colors.mint}"
    rounded: "{rounded.circle}"
    width: "57px"
    height: "57px"
  round-link-hover:
    backgroundColor: "{colors.round-hover}"
  website-row:
    textColor: "{colors.ink}"
    padding: "28px 0"
---

# Design System: Portfolio di Matteo

## Overview

**Creative North Star: "Una raccolta di prodotti reali"**

Il portfolio è un tavolo di progetti selezionati: carta azzurra, inchiostro verde scuro e immagini dei prodotti realmente online. Il titolo «Matteo. Costruisco prodotti.» introduce una presentazione personale, seguita da Pause, Parola e tre siti pubblici. I testi e le etichette rimangono in italiano; ruoli aziendali e marchi esclusi dal perimetro corrente non compaiono sul frontend, nei metadati o nelle immagini pubblicate.

La composizione è ariosa ma diretta. Titoli grandi, descrizioni brevi e collegamenti espliciti permettono di capire e aprire ogni prodotto. Le catture reali portano la varietà visiva, mentre il contenitore del portfolio mantiene una sola famiglia tipografica e controlli coerenti.

**Key Characteristics:**
- Carta azzurra, inchiostro verde scuro e azioni blu.
- Onest locale, titoli ampi e descrizioni brevi in italiano.
- Catture reali montate su superfici morbide, righe web delimitate da filetti.
- Collegamenti semantici, focus visibile e movimento contenuto.

## Colors

La palette separa le azioni blu dalla carta azzurra e dalla fascia biografica verde. I colori normativi seguono il CSS conservato; le varianti senza istanze correnti non costituiscono sezioni da reintrodurre.

### Primary
- **Blu azione** (`blue`): parola «prodotti.» nel titolo, azioni principali, focus e frecce dei siti; `primary-hover` ne scurisce lo stato hover.

### Secondary
- **Verde bosco** (`green`): fondo della sezione biografica; `round-hover` resta una variante CSS del controllo circolare generico senza istanze nella pagina corrente.
- **Menta campione** (`mint`): token CSS conservato per il controllo circolare generico; nessun grande campo menta è presente nella pagina corrente.

### Neutral
- **Carta azzurra** (`paper`): sfondo continuo della pagina.
- **Inchiostro petrolio** (`ink`): titoli e testo principale.
- **Ardesia leggibile** (`muted`): descrizioni e metadati sulla carta.
- **Filetto freddo** (`rule`): separatori di intestazione, siti e piè di pagina.
- **Bianco** (`white`): testo delle azioni blu e del link nella biografia.
- **Testo inverso** (`about-heading`, `about-copy`): titoli e corpo sulla biografia scura.
- **Disco azzurro** (`arrow-surface`): fondo a riposo delle frecce dei siti.

**The Action Color Rule.** Il blu identifica azioni e accenti di orientamento; il verde scuro definisce la fascia biografica.

## Typography

**Display Font:** Onest, con fallback ui-sans-serif, system-ui, sans-serif.
**Body Font:** Onest, con gli stessi fallback.

Il font variabile è servito localmente da `docs/assets/fonts/onest.woff2`, con pesi disponibili da 100 a 900 e `font-display: swap`. Titoli bilanciati e tracking serrato danno carattere senza cambiare famiglia.

### Hierarchy
- **Display**: ruolo `display` per il titolo personale; a 1500px e oltre passa a 96px. A 850px e sotto usa `clamp(42px, 7.9vw, 72px)`; a 560px e sotto usa `clamp(36px, 8.7vw, 49px)` con interlinea 1.1.
- **Headline**: ruolo `headline` per le sezioni. A 560px e sotto i titoli delle sezioni progetti sono 31px, la biografia 32px e il contatto 38px.
- **Title**: ruolo `title` per le app; 28px su mobile. I titoli delle righe web sono 25px, poi 22px entro 850px.
- **Body**: ruolo `body` come base; le descrizioni app usano 15px/1.75 e una misura massima di 47ch, poi 14px entro 850px. Le descrizioni web scendono da 14px a 13px su mobile.
- **Label**: ruolo `label` per navigazione e collegamenti testuali; i metadati sono 12px. I pulsanti passano a 14px entro 850px e 13px entro 560px. Nessuna trasformazione sistematica in maiuscolo.

## Layout

Il contenitore centra il contenuto con larghezza `min(100% - var(--pad)*2, 1200px)` e inset fluido dal token `page-inset`. A 1440px il contenuto occupa 1200px, con margini laterali di 120px. La biografia attraversa lo schermo, mantenendo il testo nel contenitore.

Sul desktop l'introduzione abbina testo a sinistra e azioni a destra; due app condividono una griglia a colonne uguali. Le righe dei siti usano testo, miniatura da 245px e freccia, con gap di 36px. La biografia ha due colonne e gap di 72px. La distanza superiore delle sezioni usa il token `section`, con un'eccezione corrente: la prima sezione app usa `padding-top: 20px` a tutte le larghezze per avvicinarsi all'introduzione.

- **Entro 850px (stato CSS per 768px):** griglia app ancora a due colonne, gap di 24px; metadati sotto i nomi. Miniature web da 190px, frecce da 36px e gap di 20px. La biografia conserva due colonne, con gap di 34px. Le sezioni usano `tablet-section`; il footer può andare a capo.
- **Entro 560px (stato CSS per 390px):** marchio solo SVG e navigazione testuale compatta; introduzione e contatto impilati. Le azioni introduttive condividono una riga quando c'è spazio e possono andare a capo. App e biografia passano a una colonna; i siti mantengono testo e freccia, nascondendo la miniatura. Le sezioni usano `mobile-section`.
- **Entro 360px (stato CSS per 320px):** le azioni introduttive possono andare su righe separate. L'inset minimo rimane 20px e l'ordine del contenuto non cambia. Le ulteriori regole CSS del controllo circolare non hanno istanze nella pagina corrente.

**The Content Order Rule.** Conservare nome e presentazione personale, azione verso i progetti, app personali, siti pubblici, biografia e contatto in un ordine leggibile anche quando le colonne si impilano.

## Elevation & Depth

Le superfici correnti sono piatte: carta, fascia scura e filetti definiscono le aree, senza ombre di elevazione applicate. Le ombre già presenti nelle immagini dei prodotti restano parte delle catture e non diventano token del portfolio. Il CSS conserva regole senza istanze per vecchi montaggi: non sono una richiesta di reintrodurre quei contenuti.

## Shapes

I montaggi principali usano il raggio `mount`; i controlli rettangolari il raggio `control`. Su mobile le immagini app adottano `mobile-product`. Le anteprime web hanno raggio 9px. Le frecce delle righe web sono dischi; il CSS conserva inoltre un controllo circolare generico senza istanze correnti. I filetti sono sottili (1px), senza cornici pesanti.

## Components

### Azione principale
Un collegamento HTML a fondo blu, testo bianco e freccia SVG. Altezza minima 56px sul desktop, 50px su mobile; padding e raggi seguono `button-primary`. L'hover scurisce il fondo con transizione di colore di 0.2s. Il testo spiega la destinazione: «Scopri i progetti» porta a `#progetti`, «Il mio profilo GitHub» apre il profilo pubblico.

### Collegamenti testuali e navigazione
Navigazione con etichette «Progetti», «Chi sono», «Contatti», senza menu nascosto. Le aree dei link di navigazione e dei link testuali ricorrenti hanno altezza minima 44px. L'hover aggiunge sottolineatura; il focus tastiera ha contorno blu da 3px con offset 6px. Nella fascia verde il contorno diventa chiaro. Il link «Vai al contenuto» appare al focus e porta al main. I controlli solo icona hanno nomi accessibili; le frecce decorative sono SVG nascosti alla tecnologia assistiva. Questi sono comportamenti osservati nel codice, non una dichiarazione di audit WCAG completo.

### Controllo circolare generico conservato
La variante CSS `round-link` resta documentata come componente senza istanze nella pagina corrente: fondo verde, freccia menta, hover più chiaro e nome accessibile. La sua presenza nel sistema non autorizza sezioni o marchi esclusi dal frontend.

### Prodotti personali
Immagini con rapporto 1.44, testo esterno al montaggio e link esplicito sotto la descrizione. Non esiste uno sfondo separato per l'intera scheda. Su dispositivi con hover la cattura cresce appena (scala 1.015) in 0.5s, senza muovere il contenitore.

### Righe dei siti
L'intera riga è un collegamento: titolo, descrizione, dominio, eventuale miniatura e freccia. All'hover il titolo viene sottolineato e il disco passa da azzurro a blu con freccia bianca. Su mobile la miniatura è nascosta, lasciando titolo e destinazione leggibili.

### Movimento e autonomia
L'introduzione ha un solo ingresso di 0.65s, con traslazione verticale da 10px a zero e curva `cubic-bezier(.16, 1, .3, 1)`. Non c'è animazione continua. Lo scorrimento degli anchor è fluido. Con `prefers-reduced-motion: reduce`, scorrimento, animazioni e transizioni diventano immediati. La pagina è statica: nessuno script di tracking, form o dipendenza da un servizio di analytics nell'HTML documentato.

## Do's and Don'ts

### Do:
- **Do** mantenere la presentazione personale di Matteo e le etichette in italiano.
- **Do** usare catture reali dei prodotti e descrizioni verificabili.
- **Do** conservare link semantici, nomi accessibili, focus visibile e preferenza di movimento ridotto.
- **Do** far adattare righe e colonne alla larghezza senza cambiare l'ordine narrativo.

### Don't:
- **Don't** sostituire le anteprime reali con risultati, metriche o testimonianze inventate.
- **Don't** reintrodurre ruoli aziendali, marchi esclusi o codice privato nel frontend, nei metadati o nelle immagini pubblicate.
- **Don't** aggiungere movimento continuo o obbligare l'animazione con movimento ridotto attivo.
- **Don't** introdurre tracker o contatti personali non approvati.
