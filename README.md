# Boston Housing: analisi dei prezzi mediani

Analisi esplorativa del dataset Boston Housing per studiare l’associazione tra alcune caratteristiche dei quartieri e il prezzo mediano delle abitazioni (`medv`). Il progetto confronta una regressione lineare semplice con un modello a due variabili esplicative.

## Domande di analisi

- Come varia `medv` al variare del numero medio di stanze (`rm`)?
- L’aggiunta di `lstat`, indicatore legato alla quota di popolazione in condizioni socioeconomiche svantaggiate, migliora la capacità esplicativa del modello?
- Quali sono gli intervalli di confidenza e di previsione per un’abitazione con valori selezionati di `rm` e `lstat`?

## Dati

Il file `Boston.csv` contiene 506 osservazioni e 14 variabili. L’analisi si concentra su `medv` (prezzo mediano, espresso in migliaia di dollari), `rm` (numero medio di stanze) e `lstat`.

## Metodi e strumenti

- Statistiche descrittive e matrice di correlazione
- Grafici a dispersione e boxplot
- Regressione lineare semplice: `medv ~ rm`
- Regressione lineare multipla: `medv ~ rm + lstat`
- Intervalli di confidenza e di previsione; analisi grafica dei residui
- R e R Markdown

## Risultati principali

Nel report, il modello con `rm` spiega circa il 48% della variabilità osservata di `medv`. Aggiungendo `lstat`, l’R² sale a circa 0,64. I risultati descrivono associazioni nel dataset e non dimostrano rapporti causali.

## File del progetto

- `Es_Boston.Rmd`: analisi e codice sorgente del report
- `Es_Boston.pdf`: report renderizzato
- `Boston.csv`: dati utilizzati

## Come riprodurre l’analisi

1. Clona o scarica il repository.
2. Apri `Es_Boston.Rmd` in RStudio, mantenendo `Boston.csv` nella stessa cartella.
3. Esegui il documento per generare il report. Il file R Markdown carica i pacchetti R necessari e contiene le istruzioni di installazione.

Il dataset è storico: le relazioni stimate non sono una valutazione dei prezzi immobiliari attuali. Prima di riutilizzarlo, consulta e cita la fonte originale dei dati.
