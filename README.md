# abbiategrasso-data-notes

Repo personale per analisi civiche locali, prototipi rapidi e notebook su
Abbiategrasso, il territorio vicino e dataset pubblici letti in chiave locale.

Non e' una copia di DataCivicLab.
Serve a:

- esplorare filoni piu' stretti o piu' locali
- testare notebook e tagli analitici prima di portarli nel Lab
- tenere una voce personale sui dati pubblici del territorio

## Cosa entra qui

- notebook locali
- note di lavoro leggere
- grafici esportati
- fonti pubbliche usate per il singolo caso

## Cosa non entra qui

- doppioni dei repo del Lab
- contratto tecnico canonico di candidate DI
- runtime o tooling da mantenere in `toolkit`
- processi condivisi del core-team

## Struttura minima

```text
abbiategrasso-data-notes/
  notebooks/
  notes/
  figures/
```

## Primo uso consigliato

Partire con un solo caso pilota:

- un notebook
- 2-3 grafici
- una nota breve su domanda, fonte e caveat

Se un filone diventa riusabile o interessante oltre il livello locale, puo'
poi migrare o ispirare lavoro dentro DataCivicLab.

## Filone attuale

### Abbiategrasso: popolazione e consumo di suolo

Primo caso pilota gia' impostato nella repo.

Notebook principale:

- `notebooks/abbiategrasso_locale_v1.ipynb`

Materiali collegati:

- `notes/abbiategrasso-popolazione-consumo-suolo.md`
- `notes/abbiategrasso-vs-comuni-vicini.md`
- `figures/abbiategrasso_vs_comuni_suolo_per_residente.png`

Segnale iniziale:

- Abbiategrasso ha circa `32.658` residenti
- il suolo consumato 2024 e' `710,4 ha`
- il confronto con alcuni comuni vicini mostra Abbiategrasso nella fascia alta per suolo consumato per residente
- il segnale recente di incremento per residente emerge piu' di quanto ci si aspetterebbe guardando solo lo stock
