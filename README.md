# itstracker

Tv Series & Film Tracker App — app web (single-page, PWA installabile) per tenere traccia delle serie TV e dei film che guardi, con dati aggiornati in tempo reale da TMDB.

## Funzionalità

- **Libreria serie TV e film**: aggiungi titoli cercandoli su TMDB, vista a griglia o a lista.
- **Tracciamento episodi**: segna gli episodi visti stagione per stagione, con episodi futuri disabilitati finché non sono usciti.
- **Continua a guardare**: rail con il prossimo episodio da vedere per ogni serie in corso.
- **In arrivo**: prossimi episodi/uscite delle serie in libreria.
- **Statistiche**: ore viste, generi preferiti (grafico a ciambella), andamento mensile.
- **Achievement**: obiettivi sbloccabili in base alle abitudini di visione.
- **Commenti e like**: ogni serie ha una sezione commenti — possono commentare solo gli utenti loggati con Google, mentre i like sono aperti a tutti, anche senza accesso.
- **Accesso con Google e sync cloud**: login opzionale per sincronizzare la libreria tra dispositivi tramite Firebase/Firestore.
- **Import/Export**: backup e ripristino della libreria in formato JSON.
- **Tema chiaro/scuro** e installazione come PWA.

## Deploy

L'app è statica (un unico `index.html`) e viene pubblicata su GitHub Pages ad ogni push su `main` tramite GitHub Actions.
