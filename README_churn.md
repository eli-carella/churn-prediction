# 📊 Customer Churn Prediction con Random Forest

Questo progetto utilizza un modello di machine learning basato su Random Forest per prevedere il **churn dei clienti** (abbandono) nel settore delle telecomunicazioni. Il dataset utilizzato è il [Telco Customer Churn Dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) disponibile su Kaggle.

## 🧠 Obiettivo del progetto

* Predire quali clienti sono a rischio di abbandono.
* Individuare i fattori chiave che influenzano la decisione di un cliente di lasciare l’azienda.
* Affrontare lo sbilanciamento della classe target utilizzando **SMOTE (Synthetic Minority Oversampling Technique)**.

## 📁 Struttura del Notebook

1. **Import e caricamento dati**
2. **Pulizia e preprocessing**
3. **Analisi esplorativa dei dati (EDA)**
4. **Codifica delle variabili categoriche**
5. **Suddivisione in training/test set**
6. **Bilanciamento del training set con SMOTE**
7. **Training del modello Random Forest**
8. **Valutazione delle performance**
9. **Analisi della feature importance**
10. **Conclusioni aziendali**

## 🧪 Tecniche utilizzate

* **Label Encoding** per la codifica delle variabili categoriche
* **SMOTE** per bilanciare la variabile target (`Churn`)
* **Random Forest** per la classificazione
* **Confusion Matrix, Accuracy, Precision, Recall, F1-score** per la valutazione
* **Visualizzazioni con Matplotlib/Seaborn**

## ⚙️ Requisiti

* Python ≥ 3.7
* `pandas`, `numpy`, `seaborn`, `matplotlib`
* `scikit-learn`
* `imblearn` (installabile con `pip install imbalanced-learn`)

## 📈 Risultati

* **Accuracy** dopo bilanciamento: \~0.77
* **Recall** per clienti che abbandonano: migliorato da 0.49 a 0.57
* **Feature importanti**: tipo di contratto, metodo di pagamento, durata del contratto, spesa mensile

## 📌 Conclusioni

Il modello fornisce buone performance nel rilevare clienti a rischio churn e può essere usato per supportare strategie aziendali di fidelizzazione (es. campagne retention, sconti mirati, modifiche contrattuali).
