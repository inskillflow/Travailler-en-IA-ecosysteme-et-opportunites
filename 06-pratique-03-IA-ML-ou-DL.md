> **Instructeur :** REHOUMA Haythem
> **Date :** Octobre 2025
> **Durée :** 25 minutes (Partie Quiz)
> **Consignes :**
  
- Lisez attentivement chaque énoncé.
- Pour chaque question (1 à 10), indiquez **une seule** catégorie : **IA**, **ML** ou **DL**.
- IA = systèmes à règles, **sans apprentissage** ; ML = apprentissage **sans réseaux profonds** ; DL = **réseaux de neurones profonds** (CNN/RNN/Transformers, etc.).


# Partie 1 - Quiz – IA / ML / DL 


## Questions 

1. Un calculateur fiscal qui applique des **barèmes** et des **règles “si… alors…”** pour estimer l’impôt dû, sans apprendre des données passées.
   Réponse (IA / ML / DL) : ______

2. Un modèle qui **prédit la demande électrique horaire** d’une ville à partir de 5 ans d’historique en utilisant **régression** et variables météo (pas de réseaux profonds).
   Réponse (IA / ML / DL) : ______

3. Un système de **segmentation d’images médicales** (IRM) basé sur une **architecture U-Net** entraînée sur des milliers d’exemples annotés.
   Réponse (IA / ML / DL) : ______

4. Un **assistant téléphonique** qui suit un **arbre de décision scripté** (menus DTMF/voix) pour router les appels, sans apprentissage.
   Réponse (IA / ML / DL) : ______

5. Un moteur de **notation de risque crédit** utilisant **gradient boosting** sur données tabulaires (revenus, ancienneté, incidents), sans réseaux profonds.
   Réponse (IA / ML / DL) : ______

6. Un système de **reconnaissance de l’écriture manuscrite** utilisant un **Transformeur visuel** entraîné sur des millions d’images de texte.
   Réponse (IA / ML / DL) : ______

7. Le **contrôle d’un four industriel** par **seuils** et temporisations (PID + règles) : si T > 900 °C alors couper, sinon maintenir. Pas d’apprentissage.
   Réponse (IA / ML / DL) : ______

8. Détection d’**anomalies** sur capteurs d’une flotte de pompes (pression/débit) via **Isolation Forest** et séries de temps nettoyées.
   Réponse (IA / ML / DL) : ______

9. **Transcription vocale** en texte en temps réel avec un **modèle end-to-end** (RNN/Transformeur audio) entraîné sur des milliers d’heures.
   Réponse (IA / ML / DL) : ______

10. **Recommandations produits** par **factorisation de matrices** (collaboratif implicite) sans réseaux profonds.
    Réponse (IA / ML / DL) : ______

<br/>

# Questions de développement (30 minutes)

## Consigne générale

Proposez **trois exemples distincts** :

* **(A) IA par règles** (ni ML ni DL)
* **(B) ML (IA mais pas DL)**
* **(C) DL (réseaux profonds)**

Pour **chaque** exemple, fournissez :

1. **Contexte** (2–3 lignes : qui utilise, pour quel objectif).
2. **Entrées → Sorties** (données attendues, format, résultat produit).
3. **Justification de la catégorie** :

   * (A) Décrivez la **logique déterministe** “si… alors…”, absence d’apprentissage.
   * (B) Expliquez la **nature tabulaire/structurée**, la **complexité modérée**, l’**algorithme non profond** (p. ex. régression, SVM, forêts, boosting).
   * (C) Argumentez la **complexité** (images/son/texte libre, grande échelle) et l’**usage explicite d’un réseau profond** (CNN/RNN/Transformeur).

### Modèle de réponse à remplir

**(A) IA par règles (sans ML/DL)**

* Contexte : …
* Entrées → Sorties : …
* Justification : …

**(B) ML (IA mais pas DL)**

* Contexte : …
* Entrées → Sorties : …
* Algorithme pressenti : …
* Justification : …

**(C) DL (réseau profond)**

* Contexte : …
* Entrées → Sorties : …
* Architecture pressentie : …
* Justification : …

<br/>

# Étude de contexte de l’IA (marchés) — 1 h, travail individuel

**Objectif :** Identifier où l’IA est la plus utilisée selon **deux marchés géographiques** au choix (ex. **États unis**, **Québec**, **Allemagne** et **Ontario** ; ou **Maroc** et **France**).

## 1) Analyse par marché (40 %)

Pour **chaque marché**, répondez :

* **Secteurs les plus actifs** (p. ex. industrie, santé, finance, retail, énergie…).
* **Cas d’usage dominants** (chatbots, vision, prédiction demande, maintenance prédictive, NLP clinique, détection fraude, copilotes code…).
* **Facteurs explicatifs** (économie, démographie, politique publique, maturité cloud, réglementation, pénurie/abondance de talents).

## 2) Comparaison (30 %)

* **Similarités / différences clés** (adoption, régulation, financement, écosystèmes).
* **Niveau de maturité** (cadres juridiques, aides publiques, hubs/clusters, emploi).
* **Tableau de synthèse** obligatoire (2 marchés × 3 volets min. : Réglementation, Financement, Emploi/Compétences).

> **Gabarit minimal de tableau**
>
> | Volet              | Marché A | Marché B |
> | ------------------ | -------- | -------- |
> | Réglementation     | …        | …        |
> | Financement        | …        | …        |
> | Emploi/Compétences | …        | …        |

## 3) Proposition d’application (30 %)

Choisissez **l’un des deux marchés** et proposez une application IA réaliste :

* **Problème** ciblé et utilisateurs finaux.
* **Type d’IA** (IA par règles, ML traditionnel, DL) & briève **architecture**.
* **Données** (sources, volume, qualité, gouvernance).
* **Impact attendu** (coûts, gains, risques).
* **Limites** (biais, vie privée, conformité, coûts d’inférence, dépendances cloud).

### Barème (section marchés) – /60

* Analyse pertinente : /20
* Comparaison claire (avec tableau) : /15
* Proposition réaliste (technique & métier) : /15
* Présentation et clarté : /10
  **Total : /60**

<br/>

## Annexe 1 — Rappels synthétiques

* **IA (large)** : systèmes **à règles** (logique, planification, recherche d’états), **pas d’apprentissage** requis.
* **ML** : apprentissage **à partir de données** (souvent **structurées/tabulaires**), **sans réseaux profonds**.
* **DL** : **réseaux de neurones profonds** (CNN/RNN/Transformers), adaptés aux **tâches complexes** et/ou **données massives** (images, audio, texte libre).

## Annexe 2 — Ressources (au choix des étudiants)

* Offres d’emploi/observatoires : LinkedIn Jobs, Indeed, StatCan, Investissement Québec, OECD AI Observatory, AI.gov, rapports sectoriels.
* Bonnes pratiques : vérifier fiabilité des sources ; citer chiffres avec référence.

