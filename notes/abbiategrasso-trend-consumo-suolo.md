# Abbiategrasso: trend storico del consumo di suolo

## Domanda guida

Il segnale `2023-2024` visto nel primo notebook e' solo un episodio recente o
si inserisce in un trend piu' lungo?

## Fonte e metodo

La serie e' ricostruita a partire dal file ISPRA `Comuni_2006_2024`.

Il file bundled usato qui non e' una nuova fonte autonoma: e' una rielaborazione
locale molto leggera del filone
[DataCivicLab](https://github.com/dataciviclab) su consumo di suolo ISPRA,
tenuta piccola solo per rendere il notebook riproducibile in questa repo.

Punto di partenza:

- stock di suolo consumato `2024`: `710,4 ha`

Poi, andando a ritroso, lo stock dei singoli anni-soglia e' stimato sottraendo
gli incrementi netti riportati da ISPRA:

- `2006-2012`
- `2012-2015`
- `2015-2016`
- `2016-2017`
- `2017-2018`
- `2018-2019`
- `2019-2020`
- `2020-2021`
- `2021-2022`
- `2022-2023`
- `2023-2024`

Questo vuol dire che la serie qui non e' annuale perfetta per tutto il periodo:

- fino al `2015` usa anche intervalli pluriennali
- dal `2015` in poi la lettura diventa molto piu' fine

## Segnale che emerge

La traiettoria ricostruita e' abbastanza stabile fino al `2023`.

Valori chiave:

- stock stimato `2006`: `675,31 ha`
- stock stimato `2023`: `701,56 ha`
- stock `2024`: `710,4 ha`

Quindi:

- tra `2006` e `2023` Abbiategrasso accumula circa `26,25 ha`
- nel solo passaggio `2023-2024` aggiunge `8,84 ha`

Questo non basta da solo a spiegare il perche' del salto, ma rafforza una
lettura semplice:

- il `2023-2024` non sembra un incremento qualsiasi dentro una serie uniforme
- sembra invece una variazione recente molto piu' marcata del profilo medio
  osservato negli anni immediatamente precedenti

## Materiali collegati

- `data/abbiategrasso_suolo_trend.csv`
- `figures/abbiategrasso_suolo_trend.png`

## Caveat

- e' una ricostruzione leggera, non una serie storica ufficiale ripubblicata da
  ISPRA
- usa gli incrementi netti disponibili nel file sorgente per tornare indietro
  dal valore `2024`
- la serie puo' includere anche piccoli incrementi netti negativi, compatibili
  con casi di riduzione o desigillazione netta
- per capire le cause del salto recente servirebbero altre fonti o un livello
  territoriale piu' dettagliato
