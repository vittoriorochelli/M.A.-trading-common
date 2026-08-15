# M.A. Trading — North Star

## Scopo

M.A. Trading ha l'obiettivo di costruire sistemi di trading che, se validati da risultati reali sufficientemente robusti, possano contribuire all'indipendenza economica dal lavoro tradizionale.

L'orizzonte obiettivo attuale è il **10 agosto 2027**. Questa data è un target di progetto, non un vincolo che possa giustificare scorciatoie, trading forzato o riduzione degli standard di validazione.

## Vincoli reali di progettazione

I sistemi devono essere utilizzabili anche in condizioni di:

- energia personale disponibile limitata;
- tempo frammentato;
- attenzione non continuativa;
- impegni di lavoro imprevedibili.

Il progetto non deve presupporre un utente futuro con più tempo, più energia o più disciplina di quella realisticamente disponibile. Deve invece ridurre progressivamente la quantità di attenzione umana necessaria.

## Quattro dimensioni di adeguatezza

Ogni sistema deve essere valutato su quattro dimensioni distinte:

1. **Edge** — esiste un vantaggio statistico reale e verificabile?
2. **Execution** — il vantaggio può essere applicato con sufficiente disciplina, coerenza e affidabilità?
3. **Economics** — capitale, rischio, rendimento e drawdown possono sostenere l'obiettivo economico reale?
4. **Personal Sustainability** — il sistema è compatibile con il tempo, l'energia e l'attenzione realmente disponibili?

Un sistema profittevole ma incompatibile con la vita reale dell'utente non è un sistema adeguato.

## Ruolo strategico dei due sistemi

### Swing / Multi-day

Lo Swing è il **candidato principale a diventare il motore economico del progetto**.

Lo sviluppo deve privilegiare:

- bassa frequenza decisionale;
- movimenti e orizzonti operativi più ampi;
- elevata selettività;
- monitoraggio e refresh automatici;
- riduzione delle verifiche manuali ripetitive;
- follow-up e validazione dei setup il più possibile automatici;
- minimo intervento umano compatibile con la robustezza del sistema.

Non ottimizzare lo Swing per produrre più segnali se questo aumenta il carico umano, la pressione o la frequenza di decisione senza un miglioramento dimostrabile dell'edge.

### Intraday

L'Intraday è un **motore complementare, selettivo e opportunistico**. Deve rimanere capace, robusto e utilizzabile, ma non deve trasformarsi in un secondo lavoro.

Lo sviluppo deve privilegiare:

- osservazione automatica del mercato;
- acquisizione automatica degli input;
- routing e refresh automatici;
- filtro multi-asset rigoroso;
- eliminazione automatica delle situazioni non interessanti;
- monitoraggio dei setup già individuati;
- coinvolgimento dell'utente soltanto quando esiste una reale ragione operativa per richiederne l'attenzione.

`NESSUN ASSET TRADABILE` è un risultato corretto e utile. Il sistema non deve essere ottimizzato per aumentare artificialmente la frequenza dei trade.

## Principio di sviluppo

**Meno nuove funzionalità, più autonomia.**

Ogni modifica proposta deve essere valutata anche con queste domande:

- migliora realmente l'edge o la qualità delle evidenze?
- riduce o aumenta le azioni manuali richieste?
- riduce o aumenta la necessità di monitoraggio continuo?
- semplifica o complica l'uso reale del sistema?
- migliora la possibilità di test, follow-up e report automatici?

Una funzione tecnicamente sofisticata non è automaticamente un miglioramento.

## Human Load Test

Per le decisioni di sviluppo può essere usato un indicatore qualitativo di carico umano:

- `+2` — riduce fortemente il carico umano;
- `+1` — riduce il carico umano;
- `0` — neutro;
- `-1` — aumenta il carico umano;
- `-2` — aumenta fortemente la dipendenza dall'intervento umano.

Questo indicatore **non è uno score di trading** e non modifica scoring, hard veto, trigger o criteri di esecuzione. Serve esclusivamente come criterio di architettura e priorità di sviluppo.

Le modifiche con valutazione `-1` o `-2` richiedono una motivazione esplicita e un beneficio sufficientemente importante da giustificare il maggior carico umano.

## Principi non negoziabili

- La scadenza economica non può ridurre gli standard di validazione.
- L'automazione non deve rendere più permissivi i criteri di trading.
- L'automazione deve ridurre lavoro ripetitivo e dipendenza dall'attenzione umana senza inventare informazioni o segnali.
- La frequenza dei trade non è un obiettivo in sé.
- La capacità di dire `NO_TRADE`, attendere o non disturbare l'utente è parte del valore del sistema.
- Questo documento governa la direzione di sviluppo dell'ecosistema; non sostituisce le regole operative specifiche contenute nelle repository Intraday e Swing.
