# Standard comuni dell'ecosistema

## Stato del documento

Questo documento stabilisce i principi comuni già decisi e identifica come **TBD** le convenzioni che richiedono verifica o una decisione esplicita. Non impone scelte tecniche arbitrarie.

## Naming

I nomi ufficiali delle repository sono `M.A.-trading-common`, `M.A.-trading-intraday` e `M.A.-trading-swing`. Convenzioni per componenti, job, file e campi: **TBD**.

## Asset

Formato canonico dei simboli, gestione di exchange/mercato, alias e validazione: **TBD**. Una futura convenzione dovrà evitare ambiguità fra asset omonimi.

## Timeframe

Formato canonico, valori ammessi e mapping con TradingView: **TBD**. La scelta metodologica dei timeframe rimane specifica delle strategie.

## Screenshot

Naming, formato, risoluzione, metadati, controlli di qualità, percorso e retention: **TBD**. Ogni futura convenzione dovrà consentire di ricondurre uno screenshot a esecuzione, asset e contesto senza inserire segreti nel nome file.

## Struttura delle cartelle

La root di questa repository contiene i documenti comuni collegati dal [README](README.md). La struttura del software locale, degli output e delle repository di strategia: **TBD** e fuori dall'ambito di questo documento finché non verificata.

## Identificazione delle esecuzioni

Formato e generazione dell'identificatore, unicità, correlazione multi-asset e propagazione fra interfaccia, automazione, log e risultati: **TBD**.

## Formato dei risultati

Schema, campi comuni, rappresentazione degli esiti parziali, versionamento e formati di visualizzazione o esportazione: **TBD**. Il contenuto analitico specifico resta responsabilità di Intraday o Swing.

## Gestione degli errori

Gli errori comuni devono essere correlabili all'esecuzione e alla fase, comprensibili e privi di segreti. Tassonomia, codici, severità e contratto di propagazione: **TBD**.

## Logging

I log comuni devono supportare diagnosi e correlazione senza registrare credenziali o dati sensibili non necessari. Formato, livelli, destinazione, retention e regole dettagliate di redazione: **TBD**.

## Compatibilità Intraday/Swing

Le capacità comuni devono poter servire entrambe le strategie senza costringerle a condividere metodologia, prompt o logica. Eventuali differenze devono essere espresse attraverso confini o configurazioni espliciti; il relativo contratto è **TBD**.

## Separazione tra strategia e infrastruttura

- Metodologia, prompt, segnali, criteri decisionali e logica specifica appartengono alla repository della strategia interessata.
- Automazione e servizi condivisibili appartengono al livello infrastrutturale; in questa repository se ne documentano know-how, standard e decisioni, non il codice.
- Un documento comune può descrivere il contratto tra i livelli, ma non deve duplicare o ridefinire le strategie.

## Quando una funzionalità è candidata al livello comune

> Se una soluzione riguarda automazione, acquisizione dati, TradingView, Playwright, interfaccia remota, visualizzazione risultati, logging, error handling o infrastruttura ed è potenzialmente utilizzabile da più strategie, deve essere considerata candidata al livello comune.

La candidatura non rende automaticamente la soluzione uno standard. Prima dell'adozione occorre:

1. verificare che non incorpori logica specifica di una strategia;
2. valutarne il riuso effettivo o potenziale da parte di più strategie;
3. documentare responsabilità, impatti e punti ancora **TBD**;
4. registrare in [DECISIONS.md](DECISIONS.md) le scelte architetturali rilevanti;
5. mantenere il codice applicativo nella sua sede appropriata, non in questa repository documentale.
