# Janus — Generatore del manuale operativo dello studente

Applicazione web dell'Istituto Janus per costruire un piano didattico personalizzato e generare il relativo manuale operativo in formato Word.

## Utilizzo

La versione pubblicata con GitHub Pages funziona direttamente dal browser: non richiede installazione, Terminale o server locale.

1. Aprire l'indirizzo GitHub Pages dell'app.
2. Connettere il proprio account Google Workspace dell'Istituto Janus.
3. Scegliere l'indirizzo di studi e compilare i parametri del percorso.
4. Controllare la capacità e la percentuale di copertura.
5. Generare e scaricare il manuale Word.

L'accesso ai cataloghi Google Sheets è in sola lettura. L'app non invia i dati dello studente a un database Janus: i dati inseriti vengono utilizzati nel browser per generare il documento scaricato.

## Accesso

L'app è destinata agli account Google Workspace autorizzati dell'organizzazione `istitutojanus.it`. I singoli Fogli devono essere condivisi con i tutor che li utilizzano.

## Sicurezza

- Il client secret OAuth non deve mai essere pubblicato.
- Il client ID OAuth web è un identificatore pubblico e può essere configurato nell'app.
- L'ambito Google richiesto è esclusivamente `spreadsheets.readonly`.
- Non inserire dati reali degli studenti nei test o nel repository.

## Manutenzione

Le modifiche ai cataloghi Google Sheets sono disponibili usando **Aggiorna catalogo** e non richiedono una nuova pubblicazione dell'app. Le modifiche a `index.html` richiedono invece un nuovo commit su GitHub; GitHub Pages pubblicherà automaticamente la versione aggiornata.
