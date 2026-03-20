# Abbiategrasso: rifiuti urbani e raccolta differenziata

Quarto filone locale attivo della repo.

## Domanda guida

Come si posiziona Abbiategrasso su raccolta differenziata (%) e costo del
servizio rifiuti per abitante rispetto ai comuni gia' usati nel benchmark locale?

## Fonte

- base bundled nella repo:
  - `data/abbiategrasso_rifiuti_benchmark_2023.csv`
  - `data/abbiategrasso_rifiuti_trend.csv`
- origine del dato: mart `ispra-ru-costi-kg` di [DataCivicLab](https://github.com/dataciviclab)
- fonte pubblica primaria: ISPRA Catasto Rifiuti Urbani

## Perimetro

- anno benchmark: 2023
- trend: 2021-2024 per Abbiategrasso
- comuni benchmark RD%: 9 comuni del Sud Ovest milanese e dintorni
- comuni benchmark costi: 6 comuni (Corbetta, Trezzano, Rozzano assenti per mancanza dati ISPRA)

## Segnali principali

**Raccolta differenziata 2023:**
Abbiategrasso e' al 71.4%, gruppo medio-alto, 4a su 9.
Corbetta guida il gruppo (84.8%), Rozzano chiude (49.0%).
Tutti e 9 i comuni superano la soglia del 65% tranne Rozzano.

**Costo del servizio 2023:**
Tra i 6 comuni con dati disponibili, Abbiategrasso ha il costo piu' alto: 146.76 euro/abitante.
Corsico e' il piu' contenuto (101.40 euro/ab), Magenta si colloca nel mezzo (134.39 euro/ab).

**Trend 2021-2024:**
- RD%: picco nel 2022 (73.7%), poi discesa al 69.6% nel 2024
- Costo: minimo nel 2022 (143.66 euro/ab), rimbalzo a 166 euro/ab nel 2024
- Andamento speculare: l'anno migliore su differenziata coincide con il costo piu' basso

**Tensione da leggere:**
RD% nella media del gruppo, ma costo tra i piu' alti. Non necessariamente un problema
(dipende dal gestore, dalla densita', dalla composizione del rifiuto), ma e' il dato
da tenere sott'occhio nel tempo.

## Caveat

- Corbetta, Trezzano sul Naviglio e Rozzano non hanno dati di costo disponibili
  nel mart ISPRA 2023: non e' chiaro se per assenza di rilevazione o ritardo
- Il dato 2024 potrebbe essere una stima provvisoria (ISPRA aggiorna con un anno di ritardo)
- Il benchmark e' leggero: sei comuni scelti per coerenza con gli altri filoni,
  non per matching statistico rigoroso

## Collegamento con altri filoni

- benchmark comuni: coerente con `abbiategrasso-irpef-comunale` e `abbiategrasso-finanza-comunale-minimale`
- filone rifiuti nel Lab: discussion #22 e notebook matteocavo v1 in `dataset-incubator`
