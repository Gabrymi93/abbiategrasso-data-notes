# Abbiategrasso: finanza comunale minimale

Terzo filone locale candidato della repo.

## Domanda guida

Su quali entrate correnti si regge in modo piu' visibile il profilo finanziario
del Comune di Abbiategrasso, e quanto pesa il rapporto tra entrate proprie e
trasferimenti nel confronto con alcuni comuni vicini?

## Fonte candidata

- fonte pubblica primaria: SIOPE
- base tecnica piu' adatta nel workspace: `siope-comuni/entrate/comuni`

La scelta ha senso perche' SIOPE permette una lettura abbastanza leggera delle
entrate correnti comunali senza entrare subito nel dettaglio contabile piu'
pesante di un bilancio completo.

## Perimetro MVP

- anni: `2021-2025`
- territorio: Abbiategrasso + un gruppo piccolo di comuni gia' usati nei filoni
  locali, oppure un benchmark piu' stretto del Sud Ovest milanese
- focus iniziale su poche voci leggibili:
  - componenti principali delle entrate correnti
  - trasferimenti correnti
  - una distinzione leggibile tra entrate proprie e risorse esterne
  - una misura semplice del peso relativo delle principali componenti

## Perche' sta bene qui

- la domanda e' locale e leggibile
- il formato puo' restare leggero: un notebook, uno o due grafici, una nota
- non serve portare qui la pipeline del Lab: basta un CSV bundled molto piccolo
  derivato da un output gia' pulito

## Caveat iniziale

- SIOPE e' potente ma puo' diventare rapidamente piu' tecnica del tono della
  repo
- il primo passaggio deve restare su una lettura molto semplice delle entrate
  correnti, senza aprire subito il fronte completo di entrate + uscite + cassa
  + residui
- le label finali andranno riallineate al mart reale di `siope-comuni`, senza
  forzare una mappatura finta con le categorie del bilancio armonizzato

## Output minimo plausibile

- un notebook su Abbiategrasso e comuni di confronto
- un grafico della composizione percentuale delle entrate correnti
- una nota breve sul rapporto tra entrate proprie e trasferimenti
