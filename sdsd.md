Parfait, voici tout réécrit d’un seul bloc avec **IA par règles**, **Machine Learning** et **Deep Learning**.
Chaque diagramme est simplifié, colorisé, prêt pour GitHub et montre clairement l’entrée et la sortie.
Deep Learning est présenté comme un cas particulier du ML pour **données non structurées / tâches complexes**.

---

## IA par règles (input = rules, output = decision)

```mermaid
flowchart LR
  %% IA par règles : règles codées par l'humain -> moteur -> décision
  RULES["RULES (input)"] --> ENGINE["RULE ENGINE"] --> DEC["DECISION (output)"];

  classDef input fill:#ffe0b2,stroke:#e65100,stroke-width:1px,color:#e65100; 
  classDef output fill:#ffffb2,stroke:#e65100,stroke-width:1px,color:#e65100; 

  class RULES input;
  class DEC output;
```

**Lecture** :
Règles programmées en entrée → moteur applique les règles → décision en sortie (aucun apprentissage).

---

## Machine Learning (input = data, output = learned rules + decision)

```mermaid
flowchart LR
  %% ML : données structurées -> algo -> règles apprises -> décision
  DATA["DATA (structured input)"] --> ALGO["LEARNING ALGORITHM"] --> RULES["RULES (learned)"];
  RULES --> DEC["DECISION (output)"];

  classDef input fill:#d4f7d4,stroke:#2e7d32,stroke-width:1px,color:#1b5e20; 
  classDef output fill:#ffe0b2,stroke:#e65100,stroke-width:1px,color:#e65100; 

  class DATA input;
  class RULES output;
  class DEC output;
```

**Lecture** :
Données structurées en entrée → algorithme apprend des règles (modèle) → règles appliquées pour produire une décision.

---

## Deep Learning (input = unstructured data, output = learned deep model + decision)

```mermaid
flowchart LR
  %% DL : données non structurées/tâches complexes -> réseau profond -> modèle appris -> décision
  DATAU["DATA (unstructured input)"] --> NET["DEEP NEURAL NETWORK"] --> MODEL["DEEP MODEL (learned)"];
  MODEL --> DEC["DECISION / PREDICTION (output)"];

  classDef input fill:#d4f7d4,stroke:#2e7d32,stroke-width:1px,color:#1b5e20; 
  classDef output fill:#ffe0b2,stroke:#e65100,stroke-width:1px,color:#e65100; 

  class DATAU input;
  class MODEL output;
  class DEC output;
```

**Lecture** :
Données **non structurées** (images, audio, texte) en entrée → réseau de neurones profond apprend un **modèle complexe** → modèle utilisé pour donner une **décision/prédiction**.

---

### Résumé visuel

* **IA par règles** : Règles en entrée → Décision en sortie (pas d’apprentissage).
* **Machine Learning** : Données structurées en entrée → Règles apprises (modèle) → Décision.
* **Deep Learning** : Données non structurées / tâches complexes en entrée → Réseau profond (modèle appris) → Décision.

Ces trois blocs Mermaid sont prêts à coller dans ton README.md et rendent correctement sur GitHub.
