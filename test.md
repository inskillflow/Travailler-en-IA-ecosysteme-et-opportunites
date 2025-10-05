
* **ML** : l’**entrée** est la **donnée** (et labels si supervisé) → la **sortie** est un **modèle/règles apprises**.
* **IA (programmation par règles)** : l’**entrée** est des **règles écrites par le développeur** (+ données d’exécution) → la **sortie** est la **décision/action**.



### 1) Machine Learning — apprendre des règles à partir des données (train + inference)

```mermaid
flowchart LR
    %% --- TRAINING ---
    subgraph TRAINING[Entraînement (apprentissage des règles)]
        D1[(Données d'entraînement)]
        L1[(Labels/Targets)]
        A1[Algorithme d'apprentissage]
        M1[(Modèle / Règles apprises)]

        D1 --> A1
        L1 --> A1
        A1 --> M1
    end

    %% --- INFERENCE ---
    subgraph INFERENCE[Utilisation (prédiction)]
        ND[(Nouvelles données)]
        M1 --> P[Prédiction / Décision]
        ND --> P
    end
```

**Lecture rapide**

* **Entrée (training)** : données (et labels) → **Sortie** : modèle (règles apprises).
* **Entrée (inference)** : nouvelles données + modèle → **Sortie** : prédiction/décision.

---

### 2) IA par programmation (système à règles) — règles en entrée, décision en sortie

```mermaid
flowchart LR
    DEV[Développeur] --> R[(Règles \"si...alors...\")]
    subgraph SYSTEME[Système à règles]
        R --> E[Moteur d'inférence]
        X[(Données d'exécution)] --> E
        E --> Y[Décision / Action]
    end
```

**Lecture rapide**

* **Entrée** : règles écrites par le développeur (programme) + données d’exécution.
* **Sortie** : décision/action déterminée par les règles (pas d’apprentissage).

---

### (Optionnel) Deep Learning — cas complexes / données non structurées

```mermaid
flowchart LR
    subgraph TRAINING_DL[Entraînement]
        Dimg[(Images / Audio / Texte libre)]
        NN[Reseau de neurones profond (multi-couches)]
        Mdl[(Poids appris = Modèle)]
        Dimg --> NN --> Mdl
    end

    subgraph INFERENCE_DL[Utilisation]
        Xnew[(Données non structurées)]
        Mdl --> Yhat[Prédiction / Génération]
        Xnew --> Yhat
    end
```

**Lecture rapide**

* **Entrée (training)** : données souvent **non structurées** (images, audio, texte) → **Sortie** : modèle neuronal (poids).
* **Entrée (inference)** : nouvelles données + modèle → **Sortie** : prédiction/génération.

--
