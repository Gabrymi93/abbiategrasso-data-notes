# abbiategrasso-data-notes

Analisi civiche locali, prototipi rapidi e notebook su Abbiategrasso, il
territorio vicino e dataset pubblici letti in chiave locale.

La repo ha gia' due filoni locali leggibili e un formato abbastanza stabile.

Serve a:

- esplorare filoni piu' stretti o piu' locali
- testare notebook e tagli analitici prima di portarli nel Lab
- tenere una voce personale sui dati pubblici del territorio

## Cosa entra qui

- notebook locali
- note di lavoro leggere
- grafici esportati
- fonti pubbliche usate per il singolo caso
- piccoli dataset bundled quando servono a rendere i notebook riproducibili

## Cosa non entra qui

- doppioni dei repo del Lab
- contratto tecnico canonico di candidate DI
- runtime o tooling da mantenere in `toolkit`
- processi condivisi del core-team

## Struttura minima

```text
abbiategrasso-data-notes/
  data/
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

- `data/abbiategrasso_benchmark_min.csv`
- `data/abbiategrasso_suolo_trend.csv`
- `notes/abbiategrasso-popolazione-consumo-suolo.md`
- `notes/abbiategrasso-trend-consumo-suolo.md`
- `notes/abbiategrasso-vs-comuni-vicini.md`
- `figures/abbiategrasso_suolo_trend.png`
- `figures/abbiategrasso_vs_comuni_suolo_per_residente.png`

Segnale iniziale:

- Abbiategrasso ha circa `32.658` residenti
- il suolo consumato 2024 e' `710,4 ha`
- il confronto con alcuni comuni vicini mostra Abbiategrasso nella fascia alta per suolo consumato per residente
- il segnale recente di incremento per residente emerge piu' di quanto ci si aspetterebbe guardando solo lo stock
- la serie ricostruita 2006-2024 suggerisce che il salto `2023-2024` e' molto piu' netto degli incrementi recenti precedenti

### Abbiategrasso: redditi IRPEF comunali

Secondo filone locale attivo.

Materiali collegati:

- `data/abbiategrasso_irpef_benchmark_2019_2023.csv`
- `data/abbiategrasso_irpef_sud_ovest_2019_2023.csv`
- `notebooks/abbiategrasso_irpef_v1.ipynb`
- `notebooks/abbiategrasso_irpef_sud_ovest_v1.ipynb`
- `notes/abbiategrasso-irpef-comunale.md`
- `notes/abbiategrasso-irpef-sud-ovest-milanese.md`
- `figures/abbiategrasso_irpef_trend.png`
- `figures/abbiategrasso_irpef_benchmark_2023.png`
- `figures/abbiategrasso_irpef_sud_ovest_2023.png`

Segnale iniziale:

- tra `2019` e `2023` il reddito imponibile medio per contribuente ad
  Abbiategrasso passa da circa `22,9 mila` a `25,4 mila euro`
- nel benchmark `2023`, Abbiategrasso si colloca sotto Buccinasco e Magenta,
  ma sopra Vigevano, Corsico e Rozzano
- restringendo il confronto al Sud Ovest milanese, Abbiategrasso scende nel
  gruppo centrale-basso: resta sopra Cesano Boscone, Corsico e Rozzano, ma
  sotto Magenta, Corbetta, Gaggiano e Trezzano sul Naviglio

### Abbiategrasso: finanza comunale minimale

Terzo filone locale attivo.

Materiali collegati:

- `data/abbiategrasso_finanza_minimale_2021_2025.csv`
- `notebooks/abbiategrasso_finanza_minimale_v1.ipynb`
- `notes/abbiategrasso-finanza-comunale-minimale.md`
- `figures/abbiategrasso_finanza_composizione_2021_2025.png`
- `figures/abbiategrasso_finanza_benchmark_2025.png`

Segnale iniziale:

- ad Abbiategrasso le `Imposte proprie` restano la componente principale delle
  entrate correnti tra `2021` e `2025`
- nel `2025`, `Fondi perequativi` e `Trasferimenti correnti` restano comunque
  una quota non marginale del profilo finanziario locale
- nel benchmark leggero sui sei comuni, Abbiategrasso combina una quota di
  `Imposte proprie` piu' bassa di quasi tutto il gruppo con una quota `Altro`
  piu' ampia, quindi non appare neppure come il caso piu' dipendente da
  `Fondi perequativi` e `Trasferimenti correnti`

## Note metodologiche minime

Il benchmark dei 6 comuni e' volutamente leggero.

- non e' un confronto statistico o causale
- il gruppo e' scelto per leggibilita' territoriale, non per matching rigoroso
- serve a leggere meglio la posizione relativa di Abbiategrasso, non a costruire una classifica definitiva

Le note metodologiche principali sono in:

- `notes/benchmark-locale-minimo.md`
- `notes/abbiategrasso-vs-comuni-vicini.md`
- `notes/abbiategrasso-irpef-sud-ovest-milanese.md`

## Riproducibilita'

Il notebook principale puo' leggere un CSV bundled molto piccolo in `data/`,
cosi' resta leggibile e riusabile anche fuori dal workspace del Lab.

## Convenzione minima

La repo resta volutamente leggera.

- notebook: un notebook per caso o domanda, con nome descrittivo e specifico
- note: note brevi su domanda guida, fonte, caveat e perimetro
- usare solo notebook quando basta una lettura esplorativa con codice e grafici
- usare notebook + nota quando il filone ha gia' un piccolo risultato leggibile
- evitare naming rigidi o tassonomie pesanti finche' la repo resta piccola

## Dati bundled

Alcuni notebook leggono CSV piccoli versionati in `data/`.

- servono a rendere i notebook piu' leggeri e riproducibili
- sono sottoinsiemi minimi estratti da fonti o output piu' ricchi
- non sostituiscono la fonte primaria
- quando il dato deriva dal Lab, di solito basta una riga esplicita nella nota
  del caso su origine del CSV bundled e filone o repo di provenienza

## Confine con il Lab

Questa repo resta personale quando il filone e':

- molto locale o legato ad Abbiategrasso e territorio vicino
- utile come notebook leggero o data note, senza bisogno di pipeline condivise
- ancora esplorativo o troppo stretto per diventare un caso del Lab

Un filone puo' invece ispirare o migrare verso DataCivicLab quando:

- la domanda smette di essere solo locale e diventa riusabile altrove
- emerge un pattern che vale anche per altri territori
- il dato o il metodo meritano un perimetro piu' pubblico, stabile o replicabile

La regola pratica e' semplice:

- qui resta il caso locale
- nel Lab puo' andare il pattern, la fonte o il metodo, se diventano davvero condivisibili
