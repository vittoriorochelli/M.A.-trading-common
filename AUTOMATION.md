# Know-how comune dell'automazione

## Ambito

Questo documento organizza il know-how trasversale del sistema locale. Non contiene codice né regole operative specifiche Intraday o Swing. Per le convenzioni condivise vedere [STANDARDS.md](STANDARDS.md).

## Playwright

Playwright è utilizzato sul PC locale per automatizzare TradingView. Linguaggio, versione, browser, modalità di avvio e configurazione effettivi: **TBD**.

## Accesso a TradingView

Il sistema accede a TradingView durante l'automazione. Procedura di autenticazione, gestione delle credenziali, prerequisiti dell'account e comportamento in caso di richiesta di login: **TBD**.

## Gestione sessione

Persistenza, rinnovo, scadenza, isolamento e verifica della sessione browser: **TBD**. Le credenziali o i dati sensibili non devono essere documentati in chiaro in questa repository.

## Selezione asset

È prevista l'analisi multi-asset. Fonte dell'elenco, identificatori, validazione, ordine e gestione degli asset non disponibili: **TBD**.

## Selezione timeframe e layout

Modalità di scelta e verifica di timeframe e layout TradingView: **TBD**. Le regole proprie di Intraday o Swing devono rimanere nei rispettivi progetti.

## Acquisizione screenshot

Gli screenshot vengono acquisiti automaticamente e passati all'analisi. Area catturata, risoluzione, formato, naming, controlli di completezza, metadati, destinazione e politica di conservazione: **TBD**.

## Esecuzione multi-asset

Il sistema può lanciare analisi su più asset. Sequenzialità o parallelismo, limiti, ordinamento, isolamento dei singoli job e criteri di completamento: **TBD**.

## Passaggio degli screenshot all'analisi

Gli screenshot sono forniti a ChatGPT per l'analisi. Meccanismo di trasmissione, modello, associazione fra immagini e asset, prompt, limiti e formato della risposta: **TBD**. I prompt specifici devono essere mantenuti nei progetti Intraday o Swing.

## Gestione timeout

Devono essere distinti, dove applicabile, i timeout di navigazione, caricamento grafico, acquisizione, analisi e richiesta complessiva. Valori, criteri di rilevamento e comportamento allo scadere: **TBD**.

## Gestione errori

Gli errori dovranno essere attribuibili almeno alla fase e all'asset interessati, senza esporre segreti. Tassonomia, messaggi destinati all'utente, propagazione e criteri di esito parziale: **TBD**.

## Logging

I log dovranno permettere di ricostruire un'esecuzione senza includere credenziali o contenuti sensibili non necessari. Livelli, formato, destinazione, correlazione, retention e redazione dei dati: **TBD**.

## Retry

L'opportunità di ripetere operazioni transitorie deve evitare duplicazioni o risultati ambigui. Operazioni ritentabili, numero di tentativi, backoff e condizioni di arresto: **TBD**.

## Stato dell'esecuzione

Il sistema espone lo stato necessario alla consultazione remota. Modello degli stati, avanzamento per asset, persistenza e recupero dopo un'interruzione: **TBD**.

## Elementi da verificare sull'implementazione reale

Prima di trasformare queste sezioni in standard vincolanti occorre rilevare l'implementazione locale effettiva. In particolare restano **TBD** stack e versioni, ciclo di sessione, pipeline di acquisizione, contratto con ChatGPT, modello di esecuzione, timeout, retry, logging e stati.
