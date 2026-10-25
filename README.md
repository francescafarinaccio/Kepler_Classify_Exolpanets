# Kepler_Classify_Exolpanets
Machine Learning per l'Astronomia Computazionale: Classificazione di Esopianeti (NASA Kepler)

Questo repository contiene il progetto finale per l'esame di **Intelligenza Artificiale per la Ricerca Scientifica**. Il lavoro sviluppa una pipeline di Machine Learning rigorosa basata sul dataset **NASA Kepler Cumulative Object of Interest (KOI)** per distinguere gli esopianeti confermati dai falsi positivi fotometrici

## Sintesi del Progetto

* **Dataset**: NASA Kepler Cumulative KOI Table (7.587 osservazioni, 13 variabili fisiche)
* **Target**: Classificazione binaria tra `CONFIRMED` (1) e `FALSE POSITIVE` (0)
* **Metodologia**: 
  * Segregazione preventiva del Test Set Hold-Out (20\%)
  * Preprocessing e imputazione incapsulati in **Scikit-Learn Pipeline** (Protocollo Anti-Leakage)
  * Tuning degli iperparametri tramite **5-Fold Stratified Cross-Validation**
  * Quantificazione dell'incertezza prestazionale tramite **1.000 iterazioni Bootstrap**
  * Validazione dell'interpretabilità fisica tramite **SHAP Values**

