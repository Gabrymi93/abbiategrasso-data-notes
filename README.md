# abbiategrasso-data-notes

Domande sui dati pubblici di Abbiategrasso e del territorio vicino.

Questa repo raccoglie analisi civiche locali basate su fonti aperte: bilanci comunali,
rifiuti, redditi, consumo di suolo. I dati vengono da fonti pubbliche nazionali
(ISTAT, Banca d'Italia, ISPRA, MEF) letti in chiave locale.

È un progetto personale, non una piattaforma ufficiale. I risultati sono indicativi
e i limiti sono sempre dichiarati.

## Analisi disponibili

### Consumo di suolo (2006-2024)

Abbiategrasso ha consumato 710 ettari di suolo nel 2024, tra i valori più alti
per abitante nel confronto con i comuni vicini. Il salto 2023-2024 è più netto
di qualsiasi incremento precedente nella serie dal 2006 a oggi.

Fonte: ISPRA. [Note metodologiche](notes/abbiategrasso-popolazione-consumo-suolo.md)

### Redditi IRPEF (2019-2023)

Tra il 2019 e il 2023 il reddito imponibile medio ad Abbiategrasso è cresciuto
da 22.900 a 25.400 euro per contribuente. Nel confronto con i comuni del Sud Ovest
milanese, Abbiategrasso si colloca nella fascia centrale: sopra Corsico e Rozzano,
sotto Magenta, Corbetta e Gaggiano.

Fonte: MEF/Dipartimento delle Finanze. [Note metodologiche](notes/abbiategrasso-irpef-comunale.md)

### Raccolta differenziata e costo del servizio (2021-2024)

La raccolta differenziata è al 69,6% nel 2024, in calo dal picco del 73,7% nel 2022.
Il costo del servizio rifiuti per abitante, 147 euro nel 2023, è il più alto tra i
comuni del Sud Ovest milanese con dati disponibili. Dal 2022 in poi i due indicatori
hanno divergito: meno differenziata, costo più alto.

Fonte: ISPRA. [Note metodologiche](notes/abbiategrasso-rifiuti-raccolta-differenziata.md)

### Finanza comunale (2021-2025)

**Entrate:** le imposte proprie (IMU, addizionale IRPEF) restano la componente
principale delle entrate correnti. La dipendenza da trasferimenti esterni è nella
media del gruppo di confronto.

**Uscite:** la spesa più alta è per l'acquisto di beni e servizi (49% nel 2025),
che include i contratti per rifiuti, mense scolastiche, asilo nido e assistenza
sociale. La quota personale (22,9%) è la più alta tra i sei comuni del benchmark.
Il totale uscite è cresciuto del 15% in quattro anni (da 25,1 a 28,9 milioni di euro).

Fonte: SIOPE, Banca d'Italia. [Note metodologiche](notes/abbiategrasso-finanza-comunale-minimale.md)

## Suggerisci un'analisi

Hai una domanda sui dati pubblici di Abbiategrasso?
[Apri una issue](https://github.com/Gabrymi93/abbiategrasso-data-notes/issues/new) per segnalarla.

Non serve saper programmare. Basta descrivere la domanda e indicare, se la conosci,
la fonte pubblica di riferimento.

## Sul metodo

I confronti usano un gruppo ristretto di comuni vicini (da 6 a 9 secondo il filone),
scelto per leggibilità territoriale. Non è un'analisi statistica rigorosa: serve a
leggere meglio la posizione relativa di Abbiategrasso, non a costruire classifiche.

I limiti specifici di ogni analisi sono descritti nelle note metodologiche collegate.

## Esplorare il codice

I notebook si trovano in `notebooks/`, i dati di supporto in `data/`, i grafici in `figures/`.
Ogni filone ha una nota in `notes/` con domanda guida, fonte, caveat e perimetro.

I dati in `data/` sono sottoinsiemi minimi estratti da fonti pubbliche o dai mart di
[DataCivicLab](https://github.com/dataciviclab), e servono a rendere i notebook
riproducibili senza dipendenze esterne.

## Progetto collegato

Questa repo fa parte dell'ecosistema [DataCivicLab](https://github.com/dataciviclab),
un laboratorio civico open source sui dati pubblici italiani. I filoni che nascono
qui possono ispirare o migrare verso il Lab quando la domanda diventa riusabile
oltre il contesto locale.
