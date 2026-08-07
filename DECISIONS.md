# Registro delle decisioni architetturali

Le decisioni sono registrate in ordine cronologico. Lo stato `Accettata` indica la decisione corrente; eventuali sostituzioni future dovranno essere annotate senza cancellarne la storia.

## ADR-001 — Repository separate

- **Data:** 2026-08-07
- **Decisione:** `M.A.-trading-intraday` e `M.A.-trading-swing` restano repository GitHub distinte.
- **Motivazione:** mantenere indipendenti le metodologie, i prompt e la logica specifica dei due approcci di trading.
- **Conseguenze:** modifiche e versionamento specifici avvengono nella rispettiva repository; eventuali elementi trasversali vengono valutati per il livello comune. URL e meccanismi di coordinamento fra repository sono **TBD**.
- **Stato:** Accettata

## ADR-002 — Know-how condiviso

- **Data:** 2026-08-07
- **Decisione:** il know-how e gli standard trasversali vengono mantenuti in `M.A.-trading-common`.
- **Motivazione:** offrire una fonte di verità comune ed evitare duplicazioni o divergenze fra strategie.
- **Conseguenze:** questa repository contiene documentazione, standard e decisioni comuni, ma non logica di strategia né codice applicativo. Il processo di revisione e aggiornamento è **TBD**.
- **Stato:** Accettata

## ADR-003 — Automazione locale

- **Data:** 2026-08-07
- **Decisione:** Playwright, automazione TradingView e interfaccia HTTPS sono attualmente eseguiti su un PC locale e non fanno parte di questa repository.
- **Motivazione:** rappresentare correttamente la collocazione attuale del sistema e mantenere `M.A.-trading-common` esclusivamente documentale.
- **Conseguenze:** qui si documentano architettura e know-how comuni; collocazione del codice, distribuzione, stack e configurazione dell'ambiente locale sono **TBD** e devono essere verificati altrove.
- **Stato:** Accettata

## ADR-004 — Separazione strategia/infrastruttura

- **Data:** 2026-08-07
- **Decisione:** le metodologie di trading Intraday e Swing restano nei rispettivi progetti; le soluzioni tecnologiche riutilizzabili devono essere documentate nel livello comune.
- **Motivazione:** preservare l'autonomia delle strategie e rendere riusabili, coerenti e rintracciabili le conoscenze infrastrutturali.
- **Conseguenze:** ogni nuova funzionalità deve essere classificata in base alla regola definita in [STANDARDS.md](STANDARDS.md); i confini e i contratti ancora non verificati sono marcati **TBD**.
- **Stato:** Accettata
