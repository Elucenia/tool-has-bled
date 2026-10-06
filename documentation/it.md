<!-- ELUCENIA technical documentation · has-bled · it · no clinical/professional/rights approval -->

# HAS-BLED

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/has-bled)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Ipertensione non controllata (pressione arteriosa sistolica \> 160 mmHg)

`h`

### Funzione renale alterata (dialisi, trapianto o creatinina ≥ 2,26 mg/dL)

`rim`

### Funzione epatica alterata (cirrosi o bilirubina \> 2× e AST/ALT \> 3× la norma)

`fig`

### Ictus pregresso

`avc`

### Pregresso sanguinamento o predisposizione (anemia, trombocitopenia)

`sang`

### INR labile (tempo nell’intervallo terapeutico \< 60%)

`inr`

### Età \> 65 anni

`idoso`

### Antiaggregante o antinfiammatorio

`drogas`

### Alcol (≥ 8 consumazioni alla settimana)

`alcool`

## Edizione del metodo

HAS-BLED/Pisters 2010: 9 punti; rene/fegato/farmaci/alcol separati; contesto ESC 2024

## Formula documentata

Un punto per item: H ipertensione, A anomalia renale/epatica (1 ciascuna), S ictus, B sanguinamento, L INR labile, E età (\> 65), D farmaci/alcol (1 ciascuno). Massimo: 9.

## Limiti e popolazione

L’HAS-BLED originale stima il sanguinamento maggiore in un anno nella fibrillazione atriale. Il totale non rappresenta una controindicazione automatica all’anticoagulazione; le definizioni dei fattori e le indicazioni contemporanee devono corrispondere alla versione. La calibrazione e il trattamento antitrombotico della popolazione ne influenzano l’interpretazione.

## Riferimenti

- [Pisters R et al. A novel user-friendly score (HAS-BLED) to assess 1-year risk of major bleeding in patients with atrial fibrillation. Chest, 2010.](https://doi.org/10.1378/chest.10-0134)

- [Van Gelder IC et al. 2024 ESC Guidelines for the management of atrial fibrillation. Eur Heart J, 2024.](https://doi.org/10.1093/eurheartj/ehae176)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Risultati documentati

Le informazioni seguenti conservano gli output del metodo per esempi sintetici. Non costituiscono una validazione clinica indipendente.

### 1

Alto rischio di sanguinamento

| Dettagli del risultato | |
| --- | --- |
| Sanguinamento maggiore | 12,50 o più per 100 pazienti-anno |

Fattori modificabili: controllare la pressione, stabilizzare l’INR o passare a DOAC, rivedere antiaggreganti/FANS, ridurre l’alcol.


### 2

Alto rischio di sanguinamento

| Dettagli del risultato | |
| --- | --- |
| Sanguinamento maggiore | 3,74 per 100 pazienti-anno |

Fattori modificabili: controllare la pressione.


### 3

Rischio di sanguinamento basso

| Dettagli del risultato | |
| --- | --- |
| Sanguinamento maggiore | 1,13 per 100 pazienti-anno |

