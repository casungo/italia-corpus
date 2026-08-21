# PRD — Italia Corpus

Data audit: 2026-08-12
Stato: dataset pubblico a snapshot; copertura e freschezza dipendono dal manifest.

## Intento

- Utenti: ricercatori, sviluppatori e team che devono interrogare la legislazione italiana in Markdown e frontmatter strutturato.
- Job principale: scaricare o indicizzare atti canonici con riferimenti e stato temporale senza dover interpretare HTML proprietario.
- Non-obiettivi: garantire completezza o aggiornamento in tempo reale oltre quanto dimostrato dal manifest, modificare manualmente gli atti, o sostituire una fonte giuridica ufficiale.

## Maturità attuale

### Capacità del repository

Il repository distribuisce snapshot pubblici derivati dalle collezioni Normattiva. Ogni atto è un Markdown con metadati; `manifest.json` misura copertura e collezioni. `CONTRIBUTING.md` separa correttamente problemi sui dati dal codice della pipeline adiacente.

### Evidenza d'uso reale

È verificato il repository/snapshot corrente, non un servizio online o una promessa di copertura completa. La freschezza e l'ampiezza effettive devono essere lette dal manifest dello snapshot usato.

## Stato del lavoro

- Completato: formato Markdown/frontmatter, distribuzione dello snapshot e documentazione di provenienza.
- Attivo: uso downstream e segnalazioni di atti mancanti o malformati.
- Bloccato: nessun blocco del dataset osservato; la copertura non va inferita dal README.
- Congelato/indeciso: non modificare gli atti generati a mano; decidere il target di copertura e frequenza degli snapshot tramite la pipeline.

## Prossima azione / decisione owner

Definire e pubblicare il target di copertura/frequenza verificabile nel manifest, mantenendo il repository dati separato dalla pipeline.

## Audit anti-slop

### Testo

Nessun difetto confermato con confidenza almeno 75%. La duplicazione inglese/italiana è localizzazione intenzionale; le cautele sulla copertura sono necessarie.

### Codice

Non applicabile al corpus generato; gli artifact e i dati sono esclusi dalla ricerca di duplicazione o dead code.

### Design

Non applicabile: dataset e documentazione, senza interfaccia prodotto verificata.

## Fonti di evidenza

- [README.md](README.md)
- [CONTRIBUTING.md](CONTRIBUTING.md)
- `manifest.json`, indici e snapshot presenti
- Repository `../italia-corpus-script/` per la pipeline di generazione.
