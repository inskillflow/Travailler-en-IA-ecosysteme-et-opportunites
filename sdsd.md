
# IA par règles (input = rules, output = decision)

```mermaid
flowchart LR
  RULES["RULES (input)"] --> ENGINE["RULE ENGINE"] --> DEC["DECISION (output)"];

  classDef input fill:#ffe0b2,stroke:#e65100,stroke-width:1px,color:#e65100;
  classDef output fill:#ffe0b2,stroke:#e65100,stroke-width:1px,color:#e65100;

  class RULES input;
  class DEC output;
```

# Machine Learning (input = data, output = learned rules)

```mermaid
flowchart LR
  DATA["DATA (input)"] --> ALGO["LEARNING"] --> RULES["RULES (learned)"];
  
  classDef input fill:#d4f7d4,stroke:#2e7d32,stroke-width:1px,color:#1b5e20;
  classDef output fill:#ffe0b2,stroke:#e65100,stroke-width:1px,color:#e65100;
  class DATA input;
  class RULES output;
```

**Lecture** : on donne des **données en entrée**, l’algorithme apprend, et on obtient des **règles/modèle en sortie**.

---



```mermaid
flowchart LR
  RULES["RULES (input)"] --> ENGINE["RULE ENGINE"] --> DEC["DECISION (output)"];
  DATA["DATA (runtime)"] --> ENGINE;

  classDef input fill:#d4f7d4,stroke:#2e7d32,stroke-width:1px,color:#1b5e20;
  classDef output fill:#ffe0b2,stroke:#e65100,stroke-width:1px,color:#e65100;
  class RULES input;
  class DATA input;
  class DEC output;
```

**Lecture** : on donne des **règles et des données en entrée**, le moteur applique ces règles et donne une **décision/action en sortie**.

---

Ces deux blocs **se rendent correctement sur GitHub** :
– Pas d’accents ni guillemets typographiques
– Parenthèses limitées
– Couleurs définies via `classDef`

Tu peux ainsi montrer clairement la différence :

* **ML** : Data en entrée → Règles (modèle) en sortie
* **IA règles** : Règles en entrée → Décision en sortie




Parfait, voici le diagramme **IA par règles** simplifié au maximum avec **juste RULES en input** (colorié) et **DECISION en output** (colorié). Compatible GitHub :



**Lecture** :
– Tu donnes **des règles en entrée**,
– Le moteur applique ces règles,
– Tu obtiens une **décision/action en sortie**.
