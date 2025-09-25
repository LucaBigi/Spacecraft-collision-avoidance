# Previsione del rischio di collisione in orbita per eventi ad alto rischio

Il presente lavoro è stato svolto nell’ambito di un tirocinio curriculare presso il Comando delle Operazioni Spaziali (COS), in collaborazione con la Sapienza Università di Roma, e ha previsto lo sviluppo di un sistema predittivo basato su tecniche di machine learning, in grado di stimare, con almeno due giorni di anticipo, il rischio finale associato a ciascun evento di congiunzione in orbita bassa (LEO), utilizzando esclusivamente le informazioni contenute nei Conjunction Data Messages (CDM), messaggi standardizzati che descrivono le condizioni orbitali relative ai due oggetti coinvolti. 

Come riferimento per la valutazione delle prestazioni dei modelli sviluppati, sono stati utilizzati i dataset e i criteri ufficiali della Spacecraft Collision Avoidance Challenge, promossa dall’Agenzia Spaziale Europea (ESA) nel 2019. 

Dopo una panoramica delle criticità del problema e dei principali algoritmi esplorati, la tesi si concentra sulla descrizione dettagliata della pipeline finale di classificazione: un sistema multilivello, basato su un’architettura modulare ed ensemble di modelli. Il cuore del sistema è costituito da 56 Support Vector Machine, coordinate attraverso meccanismi di voto e consenso per identificare eventi classificabili con maggiore affidabilità. Gli eventi più incerti vengono gestiti da fasi successive, che impiegano classificatori specializzati addestrati su sottoinsiemi mirati del dataset. 

A complemento della pipeline di classificazione è stato sviluppato in parallelo un modulo di regressione, in grado di fornire una stima continua del rischio per gli eventi etichettati come ad alto rischio dal modulo di classificazione. l'integrazione dei due modelli è stata testata sul dataset ufficiale della challenge, ed ha ottenuto uno score pari a 0.559, risultato che colloca il modello risultante al secondo posto assoluto tra i 97 team ce hanno partecipato alla Challenge, e al primo posto tra tutti i modelli interamente basati su tecniche di machine learning.

## Contenuto del repository

- **Tesi completa**: file PDF contenente una descrizione dell'intero lavoro, comprensivo di:
  - Descrizione del problema
  - Modelli di Machine Learning testati e utilizzati
  - Analisi dei risultati e metriche (F2, Recall, FPR, MSEHR, score finale)
  - Grafici e tabelle dei risultati
  - Pseudocodici e spiegazioni dettagliate dei modelli

## Nota sul codice

Il codice originale utilizzato per gli esperimenti **non è pubblico** per motivi di privacy e proprietà intellettuale. Tutti i dettagli sul funzionamento dei modelli e sulla pipeline sono comunque inclusi nella tesi in PDF.

## Licenza

Il contenuto di questo repository è a scopo accademico e informativo. Tutti i materiali sono di proprietà dell’autore e non possono essere copiati o redistribuiti senza autorizzazione.

## Citazioni

per maggiori informazioni sulla **Spacecraft Collision Avoidance Challenge** del 2019, fare riferimento a:
Thomas Uriot et al. “Spacecraft collision avoidance challenge: Design and results of a machine learning competition”. In: Astrodynamics 6.2 (2022), pp. 121–140. doi: 10.1007/s42064-021-0101-5.
