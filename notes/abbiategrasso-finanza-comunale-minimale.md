# Abbiategrasso: finanza comunale minimale

Terzo filone locale attivo della repo.

## Domanda guida

Su quali entrate correnti si regge in modo piu' visibile il profilo finanziario
del Comune di Abbiategrasso, e quanto pesa il rapporto tra entrate proprie e
risorse esterne nel confronto con alcuni comuni gia' usati nei filoni locali?

## Fonte

- base bundled nella repo: `data/abbiategrasso_finanza_minimale_2021_2025.csv`
- origine del dato: `siope-comuni/entrate/comuni`
- fonte pubblica primaria: SIOPE

Il CSV bundled deriva dal mart multi-anno del Lab e mantiene solo un perimetro
molto piccolo: `2021` e `2025`, sei comuni, poche macro-categorie leggibili.

## Perimetro minimo

- anni: `2021` e `2025`
- comuni: Abbiategrasso, Magenta, Vigevano, Buccinasco, Rozzano, Corsico
- focus:
  - `Imposte proprie`
  - `Fondi perequativi`
  - `Trasferimenti correnti`
  - `Altro`
- esclusione esplicita del titolo `9`, per restare sulle entrate correnti

## Segnali iniziali

- ad Abbiategrasso le `Imposte proprie` restano la componente principale delle
  entrate correnti sia nel `2021` sia nel `2025`
- nel `2025` il peso combinato di `Fondi perequativi` e `Trasferimenti
  correnti` resta comunque rilevante e vale circa un quarto del totale
- nel benchmark `2025`, Abbiategrasso ha una quota di `Imposte proprie` piu'
  bassa di quasi tutto il gruppo, ma non emerge neppure come il comune piu'
  dipendente da `Fondi perequativi` e `Trasferimenti correnti`, perche' pesa di
  piu' anche la quota `Altro`
- la quota `Altro` resta ampia e segnala che un eventuale follow-up dovra'
  scendere di un livello sulle voci SIOPE

## Caveat minimi

- SIOPE resta una lettura per cassa e per struttura dei flussi, non sostituisce
  un bilancio armonizzato completo
- le macro-categorie usate qui seguono il mart reale di `siope-comuni`, non una
  mappatura diretta delle categorie di bilancio tradizionali
- il benchmark dei sei comuni resta una scelta di leggibilita', non un matching
  rigoroso
