# M.A. Trading — documentazione comune

Questa repository è la fonte di verità per il **know-how, gli standard e le decisioni architetturali comuni** dell'ecosistema M.A. Trading. Il suo contenuto è documentale: non ospita codice applicativo né implementazioni delle strategie.

## Relazione con i progetti di trading

- `M.A.-trading-intraday` rimane un progetto e una repository indipendente per metodologia, prompt e logica specifici dell'operatività Intraday.
- `M.A.-trading-swing` rimane un progetto e una repository indipendente per metodologia, prompt e logica specifici dell'operatività Swing.
- `M.A.-trading-common` raccoglie soltanto ciò che è trasversale e potenzialmente riutilizzabile dalle due strategie.

I collegamenti esatti alle repository Intraday e Swing sono **TBD**. I nomi sopra identificano i progetti, non intendono indicare URL già verificati.

## Sistema locale di automazione

Su un PC locale è in esecuzione un sistema che automatizza TradingView tramite Playwright, acquisisce screenshot, avvia analisi multi-asset, passa le immagini a ChatGPT e rende disponibili avvio e risultati tramite un'interfaccia HTTPS utilizzabile da dispositivi remoti.

Il codice di Playwright e dell'interfaccia HTTPS **non si trova in questa repository**. Qui vengono documentati soltanto il ruolo architetturale del sistema, il know-how comune e le decisioni condivise; collocazione e repository del codice locale sono **TBD**.

## Principio di separazione

Le regole, i prompt e la logica propri di Intraday o Swing appartengono ai rispettivi progetti. Automazione, acquisizione, interfacce, osservabilità e altre soluzioni infrastrutturali riutilizzabili sono candidate al livello comune, dove vengono documentate senza duplicare la logica delle strategie.

## Indice

- [Architettura dell'ecosistema](ARCHITECTURE.md)
- [Know-how dell'automazione](AUTOMATION.md)
- [Interfaccia HTTPS locale](INTERFACE.md)
- [Standard comuni](STANDARDS.md)
- [Registro delle decisioni](DECISIONS.md)
