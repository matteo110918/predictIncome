# Adult Income Prediction POC

Dieses Repository enthält einen Proof-of-Concept (POC) für die Vorhersage des Einkommens (≤50K vs. >50K) anhand des „Adult Income Dataset“. Das Ziel dieses Projekts ist es, einen vollständigen ML-Workflow zu demonstrieren – von Datenanalyse über Preprocessing, Modelltraining und Evaluation bis hin zur Interpretation mittels Partial Dependence Plots.

---

## Inhalte

- [`Adult Income Dataset.csv`](Adult Income Dataset.csv)
  Ursprungsdatensatz (Census-Daten), enthält Personenmerkmale und Einkommensklasse.

- [`income_prediction.py`](income_prediction.py)
  Hauptskript mit allen Schritten:
  1. Datenanalyse (Exploratory Data Analysis)
  2. Preprocessing (Numeric & Kategorial)
  3. Modellbau (Random Forest)
  4. Evaluation (ROC-AUC, ROC-Kurve)
  5. Interpretation (Partial Dependence Plots)
  6. Speichern und Laden des Modells (`model.pkl`)

- [`model.pkl`](model.pkl)
  Persistiertes Random-Forest-Modell.

- [`README.md`](README.md)
  Diese Datei.

---

## Projektbeschreibung

1. **Datenanalyse**
   - Übersicht der Datensätze
   - Verteilung der Zielvariable `income`

2. **Preprocessing**
   - Split in Trainings- und Validierungsset (75 % / 25 %)
   - Identifikation numerischer (`age`, `hours_per_week`) und kategorialer Features
   - `OrdinalEncoder` für kategoriale Daten
   - Passthrough für numerische Daten

3. **Modelltraining**
   - Pipeline aus Preprocessor + `RandomForestClassifier`
   - 100 Bäume, maximale Tiefe = 5, `random_state=0`

4. **Evaluation**
   - Berechnung der AUC (`roc_auc_score`)
   - Darstellung der ROC-Kurve

5. **Modellinterpretation**
   - Laden des gespeicherten Modells
   - Partial Dependence Plots für `age` und `hours_per_week`

---

## Voraussetzungen

- Python ≥ 3.7
- Bibliotheken:
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `scikit-learn`
  - `pickle` (Standardbibliothek)

Installieren via:

```bash
pip install numpy pandas matplotlib scikit-learn
