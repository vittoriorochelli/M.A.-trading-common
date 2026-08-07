# Interfaccia HTTPS locale

## Finalità

L'interfaccia HTTPS, eseguita sul PC locale, consente a un dispositivo remoto di avviare le analisi e consultarne i risultati. Il suo codice non è incluso in questa repository.

## Lancio remoto delle analisi

L'avvio è possibile da remoto tramite l'interfaccia. Comandi disponibili, ciclo della richiesta, gestione delle esecuzioni concorrenti e conferme all'utente: **TBD**.

## Scelta del tipo di analisi

L'interfaccia deve distinguere la richiesta Intraday da quella Swing senza incorporarne la metodologia. Modalità di scelta, valori ammessi e validazione: **TBD**.

## Scelta degli asset

La possibilità per l'utente di scegliere gli asset, nonché origine delle opzioni, limiti e validazione, è **TBD**.

## Stato dell'esecuzione

L'interfaccia rende consultabile lo stato del lavoro. Stati mostrati, aggiornamento, granularità per asset, progressi e storico: **TBD**.

## Risultati

I risultati sono visualizzabili da PC remoto o smartphone. Struttura, ordinamento, persistenza, scadenza, esportazione e associazione all'esecuzione: **TBD**.

## Errori

Gli errori devono essere presentati in modo comprensibile e correlabili all'esecuzione, senza rivelare dati sensibili. Codici, messaggi, possibilità di ripetizione e dettaglio esposto: **TBD**.

## Utilizzo desktop

È previsto l'accesso da PC remoto. Browser supportati, layout, funzioni disponibili e requisiti di accessibilità: **TBD**.

## Utilizzo smartphone

È prevista la consultazione da smartphone. Comportamento responsive, browser supportati e possibili differenze funzionali rispetto al desktop: **TBD**.

## Sicurezza e autenticazione

L'esposizione avviene tramite HTTPS. Meccanismo di autenticazione, autorizzazioni, gestione certificati, protezione della rete, sessioni utente, audit e gestione dei segreti: **TBD**. Nessuna porta o modalità di esposizione è stabilita in questo documento.

## Comunicazione con il motore locale

L'interfaccia inoltra le richieste al motore locale e ne recupera stato e risultati. API, protocollo interno, formato dei messaggi, gestione asincrona e confini di processo: **TBD**.

Per la collocazione nel sistema vedere [ARCHITECTURE.md](ARCHITECTURE.md); per gli standard ancora da consolidare vedere [STANDARDS.md](STANDARDS.md).
