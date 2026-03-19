# Abbiategrasso: redditi IRPEF comunali

Secondo filone locale della repo.

## Domanda guida

Come si muove Abbiategrasso tra `2019` e `2023` sul reddito imponibile medio
per contribuente, e dove si colloca rispetto ad alcuni comuni gia' usati nel
benchmark territoriale?

## Fonte

- base bundled nella repo: `data/abbiategrasso_irpef_benchmark_2019_2023.csv`
- origine del dato: [`dataciviclab/preanalysis/irpef-comunale-2019-2023`](https://github.com/dataciviclab/dataciviclab/tree/main/preanalysis/irpef-comunale-2019-2023)
- fonte pubblica primaria: MEF / Finanze, dati comunali IRPEF

Il CSV bundled e' un estratto minimo derivato dal lavoro gia' fatto nel Lab e
serve solo a rendere questo notebook locale leggero e riproducibile.

## Perimetro minimo

- anni: `2019-2023`
- comuni: Abbiategrasso, Magenta, Vigevano, Buccinasco, Rozzano, Corsico
- indicatori usati:
  - `reddito_imponibile_medio_per_contribuente_eur`
  - `addizionale_comunale_media_per_contribuente_eur`
  - `numero_contribuenti`

## Segnali iniziali

- ad Abbiategrasso il reddito imponibile medio per contribuente passa da circa
  `22,9 mila` a `25,4 mila euro` tra `2019` e `2023`
- la crescita nel periodo vale circa `+11,1%`
- nel benchmark `2023`, Abbiategrasso sta sotto Buccinasco e Magenta, ma sopra
  Vigevano, Corsico e Rozzano

## Caveat minimi

- il dataset riguarda i contribuenti IRPEF, non tutti i residenti
- non e' una misura diretta di ricchezza complessiva o patrimonio
- il benchmark dei sei comuni resta una scelta di leggibilita', non un matching
  rigoroso
