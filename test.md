Top — GitHub n’aime pas certains caractères (accents, guillemets échappés, parenthèses longues) dans les **titres de subgraph** et **labels** Mermaid.
Voici des **versions 100% compatibles GitHub** (ASCII, labels simples), plus **plein d’exemples** à coller et tester.

---

## 1) Machine Learning — learn rules from data (train + inference)

```mermaid
flowchart LR
  %% TRAINING: data -> algorithm -> model
  subgraph TRAINING[Training: learn rules from data]
    D1[(Train data)]
    Y1[(Labels)]
    ALG[Learning algorithm]
    MODEL[(Trained model)]
    D1 --> ALG
    Y1 --> ALG
    ALG --> MODEL
  end

  %% INFERENCE: new data + model -> prediction
  subgraph INFERENCE[Inference: use the learned model]
    X[(New data)]
    MODEL --> P[Prediction]
    X --> P
  end
```

**Lecture rapide**

* Entrée (training) : data + labels → Sortie : **model** (règles apprises)
* Entrée (inference) : new data + model → Sortie : **prediction**

---

## 2) Rules-based AI — programming (if-then)

```mermaid
flowchart LR
  RULES["Hand-written rules if-then"]; RUNTIME["Runtime data"]; ENGINE["Rule engine"]; DECISION["Decision/Action"];
  RULES --> ENGINE; RUNTIME --> ENGINE; ENGINE --> DECISION;
```

**Lecture rapide**

* Entrée : **règles écrites** + données d’exécution → Sortie : **décision**
* Pas d’apprentissage automatique.

---

## 3) Deep Learning — unstructured data, deep nets

```mermaid
flowchart LR
  %% TRAIN
  subgraph DL_TRAIN[Training]
    U[(Unstructured data: images, audio, text)]
    NET[Deep neural network]
    W[(Learned weights = model)]
    U --> NET --> W
  end

  %% INFER
  subgraph DL_INFER[Inference]
    XU[(New unstructured data)]
    W --> Y[Prediction / Generation]
    XU --> Y
  end
```

**Lecture rapide**

* Entrée (train) : données **non structurées** → Sortie : **poids/ modèle**
* Entrée (infer) : nouvelles données + modèle → **prédiction / génération**

---

# Beaucoup d’exemples à tester

### A) ML (supervised) — classifier simple

```mermaid
flowchart LR
  TRAIN_DATA[(Tabular data)]
  LABELS[(Labels)]
  CLASSIFIER[Supervised learner]
  MODEL[(Classifier model)]
  NEW[(New row)]
  PRED[Class prediction]

  TRAIN_DATA --> CLASSIFIER
  LABELS --> CLASSIFIER
  CLASSIFIER --> MODEL
  MODEL --> PRED
  NEW --> PRED
```

### B) ML (regression) — price prediction

```mermaid
flowchart LR
  X[(Features: size, rooms, location)]
  Y[(Price)]
  REG[Regressor]
  M[(Trained regressor)]
  XNEW[(New features)]
  YHAT[Predicted price]

  X --> REG
  Y --> REG
  REG --> M
  M --> YHAT
  XNEW --> YHAT
```

### C) DL (vision) — object detection with CNN

```mermaid
flowchart LR
  IMGS["Images"]; CNN["Deep CNN"]; WEIGHTS["Learned weights"]; TESTIMG["New image"]; DETS["Detections: boxes + classes"];
  IMGS --> CNN --> WEIGHTS;
  WEIGHTS --> DETS;
  TESTIMG --> DETS;
```

### D) DL (speech/avatar) — text & voice

```mermaid
flowchart LR
  AV_DATA["Audio/Video samples"]; MODEL["Deep model (Transformer)"]; VOICE["Learned voice/face model"]; SCRIPT["Text prompt"]; OUTPUT["Talking avatar (audio/video)"];
  AV_DATA --> MODEL --> VOICE;
  VOICE --> OUTPUT;
  SCRIPT --> OUTPUT;
```

### E) Rules-based — vending machine / washer / calculator

```mermaid
flowchart TB
  BTN[B1/B2 button pressed]
  PROG[If-then program]
  ACT[Dispense coffee/tea]

  BTN --> PROG --> ACT

  WBTN[Washer program button] --> PROG2[If-then program] --> RUN[Run cycle]
  KEYS[Calculator keys] --> PROG3[If-then + ops] --> RES[Result]
```

### F) Decision guide — which approach?

```mermaid
flowchart TB
  Q0{Need learning from data?}
  Q0 -- No --> RB[Rules-based: write if-then rules]
  Q0 -- Yes --> Q1{Data type mostly structured?}
  Q1 -- Yes --> ML[Use ML (trees, SVM, regression)]
  Q1 -- No --> Q2{Images/Audio/Text or high complexity?}
  Q2 -- Yes --> DL[Use DL (CNN/RNN/Transformer)]
  Q2 -- No --> ML2[ML + feature engineering]
```

### G) Compact — ML in one glance

```mermaid
flowchart LR
  Data[(Data)] -->|train| Algo[Learning algo] --> Model[(Model)]
  New[(New data)] -->|apply| Pred[Prediction]
  Model -. used by .-> Pred
```

---

## Conseils GitHub Mermaid

* Évite les **accents**, **guillemets**, **parenthèses longues** dans les **titres de subgraph** et **labels**.
* Utilise des labels courts en **ASCII**.
* Garde la structure `flowchart LR|TB`, `subgraph ID[Title] ... end`.
* Si un rendu échoue, **simplifie** d’abord les labels (pas de slash, pas de guillemets).

Tu veux une variante **ultra-minimale** uniquement avec “Input/Output” pour coller en tête de chapitre ?
