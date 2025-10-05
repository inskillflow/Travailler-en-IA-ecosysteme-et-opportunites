Voici des **diagrammes Mermaid ultra-simples** qui montrent exactement ce que tu veux, avec **couleurs** sur l’**entrée data** (vert) et la **sortie rules** (orange). Compatibles GitHub (ASCII, labels courts, pas d’accents).

---

## Machine Learning — input = data, output = rules (learned)

```mermaid
flowchart LR
  DATA["DATA (input)"]; ALGO["LEARNING"]; RULES["RULES (learned)"];
  DATA --> ALGO --> RULES;

  %% Coloring
  classDef input fill:#d4f7d4,stroke:#2e7d32,stroke-width:1px,color:#1b5e20;
  classDef output fill:#ffe0b2,stroke:#e65100,stroke-width:1px,color:#e65100;
  class DATA input;
  class RULES output;
```

### Variante compacte (de secours)

```mermaid
flowchart LR
  D["DATA (input)"] --> A["LEARNING"] --> R["RULES (learned)"];
  classDef input fill:#d4f7d4,stroke:#2e7d32,color:#1b5e20;
  classDef output fill:#ffe0b2,stroke:#e65100,color:#e65100;
  class D input; class R output;
```

---

## IA par règles — input = rules, output = decision (pour contraste)

```mermaid
flowchart LR
  RULES["RULES (input)"]; ENGINE["RULE ENGINE"]; DEC["DECISION (output)"];
  DATA["RUNTIME DATA"] --> ENGINE;
  RULES --> ENGINE --> DEC;

  %% Coloring (rules as input)
  classDef input fill:#d4f7d4,stroke:#2e7d32,stroke-width:1px,color:#1b5e20;
  class RULES input;
```

Tu peux copier-coller tel quel dans ton README.md. Si GitHub chipote, utilise la **variante compacte**.
