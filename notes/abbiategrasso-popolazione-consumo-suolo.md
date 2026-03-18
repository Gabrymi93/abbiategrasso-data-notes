# Abbiategrasso: popolazione e consumo di suolo

## Domanda guida

Che fotografia minima possiamo ottenere su Abbiategrasso incrociando:

- popolazione residente ISTAT
- stock di suolo consumato ISPRA
- incremento piu' recente del consumo di suolo

## Fonti

- support dataset `popolazione-istat-comunale-2019-2025`
- candidate `ispra-consumo-suolo`

Entrambe le fonti sono gia' materializzate in `dataset-incubator/out/`.

## Snapshot iniziale

Valori verificati nel workspace:

- popolazione residente 2025: `32.658`
- suolo consumato 2024: `710,4 ettari`
- quota di suolo consumato 2024: `14,88%`
- incremento netto 2023-2024: `8,84 ettari`

## Perche' e' un buon primo caso

- e' strettamente locale
- usa due fonti gia' pronte nel workspace
- non richiede pipeline nuova
- permette un primo notebook leggibile senza over-engineering

## Caveat

- gli anni non coincidono perfettamente: popolazione `2025`, consumo di suolo `2024`
- e' una fotografia esplorativa, non ancora un output pubblico maturo
- per confronti territoriali piu' seri servirebbe aggiungere almeno un benchmark comunale o provinciale

## Passi successivi plausibili

1. aggiungere confronto con altri comuni del Sud Ovest milanese
2. calcolare indicatori per 1.000 residenti
3. portare poi il formato su un secondo caso locale
