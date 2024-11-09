# Pre-processing per il Dataset di Rilevazione del Tumore al Seno

Questo progetto si concentra sul pre-processing di un dataset relativo alla rilevazione del tumore al seno, con l'obiettivo di preparare i dati per essere utilizzati in modelli di machine learning. La pipeline di pre-processing è suddivisa in tre approcci distinti che trattano i dati in base al target e alle caratteristiche delle variabili.

## Obiettivo

- **Pre-processing per i record con Target = 1**: Si applicano operazioni di pulizia, simmetrizzazione delle variabili asimmetriche e one-hot encoding per le variabili categoriche, seguite da standardizzazione.
- **Pre-processing per tutti i record del dataset**: Si gestiscono i valori mancanti, si applica la discretizzazione delle variabili numeriche e si esegue l'encoding ordinale delle variabili categoriche. Inoltre, viene effettuata la selezione delle 5 variabili più informative.
- **Pre-processing delle variabili numeriche**: Si concentra sul trattamento dei valori mancanti e sull'applicazione di Principal Component Analysis (PCA) per ridurre la dimensionalità, seguita dalla normalizzazione delle variabili numeriche.

## Caratteristiche principali

- **Data Cleaning**: Gestione dei valori mancanti in modo differenziato per variabili simmetriche e asimmetriche.
- **Simmetrizzazione delle variabili asimmetriche**: Utilizzo di tecniche per migliorare la distribuzione dei dati.
- **One-Hot Encoding**: Conversione delle variabili categoriche in formato numerico.
- **Discretizzazione delle variabili numeriche**: Riduzione della complessità delle variabili numeriche.
- **Selezione delle variabili informative**: Riduzione delle dimensioni del dataset, selezionando le variabili più rilevanti per il modello.
- **Principal Component Analysis (PCA)**: Riduzione della dimensionalità del dataset per migliorare le performance dei modelli.

## Utilizzo

1. Carica il dataset.
2. Separa le variabili numeriche e categoriche.
3. Applica il pre-processing personalizzato per ciascuna pipeline.
4. Unisci le pipeline e salva il risultato finale in un file `joblib` per essere utilizzato in produzione.

## Requisiti

- `pandas`
- `scikit-learn`
- `joblib`

## Esecuzione

Per eseguire il pre-processing, carica il notebook e lancia il codice per applicare le pipeline sul dataset. L'oggetto finale (contenente tutte le pipeline) sarà esportato in un file `pipeline.joblib` per un facile riutilizzo.

## Licenza

Questo progetto è distribuito sotto la licenza MIT. Vedi il file LICENSE per ulteriori dettagli.
