# itstracker

Tv Series & Film Tracker App — app web (single-page, PWA installabile) per tenere traccia delle serie TV e dei film che guardi, con dati aggiornati in tempo reale da TMDB.

## Funzionalità

- **Libreria serie TV e film**: aggiungi titoli cercandoli su TMDB, categorie (Continua, In Pari, In Lista, In Arrivo per le serie; Visti, Da Vedere per i film), vista a griglia o a lista, filtro per genere.
- **Ricerca**: ricerca testuale o sfoglia i titoli popolari, con lo stesso filtro per genere.
- **Tracciamento episodi**: segna gli episodi visti stagione per stagione (anche tutti insieme), episodi futuri disabilitati finché non sono usciti.
- **Continua a guardare**: rail con il prossimo episodio da vedere per ogni serie in corso.
- **Swipe nella scheda dettaglio**: scorri a destra/sinistra tra le serie o i film della libreria senza chiudere e riaprire ogni volta.
- **Statistiche e achievement**: ore viste, generi preferiti, andamento mensile, obiettivi sbloccabili.
- **Anno in rassegna**: riepilogo annuale in formato storie, condivisibile.
- **Commenti sugli episodi**: thread di risposte, menzioni @, like sui commenti — commentare richiede l'accesso con Google, mettere like è aperto a tutti. Reazioni rapide (emoji) sugli episodi.
- **Profili pubblici e social**: cerca altre persone per nickname, segui/follower, feed attività degli amici, chat 1:1, notifiche (like, risposte, menzioni, messaggi) cliccabili, aggiungi alla tua libreria una serie/film visto sul profilo di un'altra persona.
- **Accesso con Google e sync cloud**: login opzionale per sincronizzare libreria e profilo tra dispositivi tramite Firebase/Firestore.
- **Import/Export**: backup e ripristino della libreria in formato JSON.
- **Tema chiaro/scuro** e installazione come PWA.

## Deploy

L'app è statica (un unico `index.html`) e viene pubblicata su GitHub Pages ad ogni push su `main` tramite GitHub Actions.

Le funzionalità social/cloud usano Firebase Authentication e Firestore. Le regole di sicurezza sono documentate in [`firestore.rules`](firestore.rules), ma **non vengono deployate automaticamente**: dopo ogni modifica a quel file va copiato manualmente il contenuto in Firebase Console → Firestore Database → Regole → Pubblica.
