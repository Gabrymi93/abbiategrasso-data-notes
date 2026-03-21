# Abbiategrasso: spese comunali per macro-categoria

Estensione del filone finanza comunale, lato uscite.

## Domanda guida

Come si distribuiscono le spese di Abbiategrasso per grandi categorie,
e quali voci pesano di piu' nel profilo recente del Comune?

## Fonte

- base bundled nella repo: `data/abbiategrasso_finanza_uscite_2021_2025.csv`
- origine del dato: mart `siope_uscite_comuni` di [DataCivicLab](https://github.com/dataciviclab/siope-comuni)
- fonte pubblica primaria: SIOPE (Banca d'Italia)

Il CSV bundled mantiene solo il perimetro minimo utile: sei comuni, due anni,
sei macro-categorie aggregate dal codice voce SIOPE.

## Perimetro

- anni: `2021` e `2025`
- comuni: Abbiategrasso, Magenta, Vigevano, Buccinasco, Rozzano, Corsico
- titoli inclusi: 1 (uscite correnti) e 2 (conto capitale / investimenti)
- escluso: titolo 3 (rimborso prestiti) e titoli successivi (partite di giro)
- macro-categorie:
  - `Acquisto beni e servizi` (1.03): contratti di servizio, utenze, canoni
  - `Personale` (1.01): stipendi, contributi, indennita'
  - `Investimenti` (2): fabbricati, strade, beni culturali
  - `Trasferimenti correnti` (1.04): trasferimenti a famiglie e enti
  - `Tributi e imposte` (1.02): IRAP e altri tributi
  - `Altro`: voci residuali titolo 1

## Segnali principali

**Composizione 2025:**
La voce piu' pesante e' `Acquisto beni e servizi` al 49%, che raccoglie i
contratti esternalizzati: rifiuti, mense scolastiche, asilo nido, assistenza
sociale, verde urbano, illuminazione pubblica. Il `Personale` e' al 22.9%,
gli `Investimenti` al 12.7%.

**Confronto 2021-2025:**
Il totale uscite passa da 25.1 a 28.9 milioni di euro (+15%). La quota
`Acquisto beni e servizi` si riduce leggermente (51.6% -> 49.0%), mentre
la quota `Investimenti` cresce (10.6% -> 12.7%): un segnale di maggiore
spesa in conto capitale nel periodo recente.

**Nel benchmark 2025:**
Abbiategrasso ha la quota `Personale` piu' alta tra i sei comuni (22.9%),
contro una media del gruppo intorno al 17-18%. La quota `Acquisto beni e servizi`
e' invece tra le piu' basse (49%), mentre Rozzano arriva al 65.8% e Magenta
al 58.8%. Corsico e' l'eccezione con una quota `Investimenti` molto alta (27%)
rispetto al resto del gruppo.

**Lettura integrata con il filone rifiuti:**
Abbiategrasso ha la quota `Personale` piu' alta del benchmark e la quota
`Acquisto beni e servizi` tra le piu' basse, ma registra comunque il costo
rifiuti per abitante piu' alto del gruppo (filone rifiuti, dato ISPRA 2023).
I due segnali coesistono: spiegarne la relazione richiederebbe dati di dettaglio
sul singolo servizio, non disponibili da SIOPE aggregato.

## Caveat

- SIOPE misura i flussi di cassa, non la competenza di bilancio: i pagamenti
  di un anno possono riferirsi a obbligazioni di anni precedenti
- la mappatura in macro-categorie segue il primo livello del codice voce SIOPE,
  non le missioni/programmi del bilancio armonizzato
- il benchmark dei sei comuni e' lo stesso degli altri filoni locali: scelta
  di leggibilita', non matching statistico
- Corsico nel 2025 mostra un totale uscite molto piu' alto (+68% rispetto al 2021),
  probabilmente per una concentrazione di pagamenti in conto capitale: da leggere
  con cautela nel confronto diretto

## Collegamento con altri filoni

- filone entrate: `abbiategrasso-finanza-comunale-minimale.md`
- filone rifiuti: `abbiategrasso-rifiuti-raccolta-differenziata.md`
  (la voce `Acquisto beni e servizi` include i contratti di raccolta rifiuti)
- mart uscite del Lab: `siope-comuni/out/data/mart/siope_uscite_comuni/`
