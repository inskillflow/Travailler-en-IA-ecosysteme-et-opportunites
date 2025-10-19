# Examen final — Métiers Data, IA, Big Data, BI, GenAI & Marketing 

**Durée :** 3 heures 
**Consignes :** Utilisez des mots simples. 



## GLOSSAIRE DES TERMES TECHNIQUES

- **KPI** : chiffre important pour piloter (ex : chiffre d’affaires, taux de conversion).  
- **Entrepôt de données (Data Warehouse)** : grande base **officielle** et **propre** pour analyser.  
- **Data Lake** : grand stockage **brut** (on garde tout, pas encore nettoyé).  
- **ETL** (Extract-Transform-Load) : on **prend**, on **nettoie/transforme**, puis on **charge** propre dans l’entrepôt.  
- **ELT** (Extract-Load-Transform) : on **prend**, on **charge brut** d’abord, **puis** on **nettoie dedans** (dans l’entrepôt).  
- **Orchestration (Airflow)** : calendrier qui **lance les étapes** (ingestion, nettoyage, chargement) et **alerte** si ça rate.  
- **Kafka (streaming)** : reçoit des **données en continu** (capteurs, clics).  
- **Spark (gros volumes)** : calcule **en parallèle** quand les données sont très grosses.  
- **Parquet (format)** : fichiers **colonnaires** comprimés, **rapides** pour analyser.  
- **API** : porte d’entrée d’un service pour demander un **résultat** (ex : une **prédiction**).  
- **Docker** : **boîte** qui contient l’application pour l’emmener partout.  
- **Kubernetes (K8s)** : **organise et fait tourner** plusieurs boîtes (Docker) et **adapte la taille** si besoin.  
- **ML (Machine Learning)** : apprend à **prédire** avec des données (ex : départ client).  
- **DL (Deep Learning)** : ML **avec gros réseaux** (images, son, texte).  
- **LLM (Grand modèle de langue)** : modèle qui **lit/écrit du texte** (chat, résumé).  
- **Prompt** : **consigne** donnée au LLM (ton, format, limites).  
- **Embeddings (vecteurs)** : version **numérique** d’un texte/image pour **chercher par le sens**.  
- **Base vectorielle** : base qui **range/cherche** par **similarité** de vecteurs.  
- **RAG** : on **cherche** d’abord des passages utiles, puis le LLM **répond** avec ces passages.  
- **Drift (dérive)** : les **données changent**, le modèle **vieillit** (il faut surveiller et réentraîner).  
- **A/B test** : tester **A vs B** proprement (ex : objet d’email).  
- **CAC / LTV / ROAS** : coût d’acquisition / valeur vie client / retour sur dépenses pub.



## MÉTIERS (rappels)

- **BI Analyst / BI Dev** : tableaux de bord clairs pour la direction (Power BI, Tableau).  
- **Data Analyst** : analyse et KPI (SQL, Excel/pandas).  
- **Analytics Engineer (AE)** : prépare des **tables propres et testées** pour analyser (dbt).  
- **Data Engineer (Big Data)** : construit les **tuyaux** (ETL/ELT), gros volumes (Spark, Kafka, Airflow).  
- **Data Architect** : organise **où sont les données** et **qui peut voir quoi**.  
- **Data Steward (Gouvernance)** : **qualité**, définitions, **règles d’accès** (PII).  
- **Data Scientist (ML)** : **expérimente** des modèles pour prédire (scikit-learn).  
- **Applied Scientist / Deep Learning** : **images/texte/son** (PyTorch/TensorFlow).  
- **ML Engineer** : met un **modèle en ligne** (API), rapide et fiable (FastAPI, Docker, K8s).  
- **MLOps / Platform** : **automatise** entraînement/déploiement/suivi (MLflow, Kubeflow).  
- **GenAI / LLM Developer** : apps avec LLM (prompts, **RAG**, embeddings).  
- **Prompt Engineer** : écrit/structure des **prompts** et **teste la qualité**.  
- **LLMOps / GenAI Platform** : **mesure et contrôle** les LLM en prod (coût, garde-fous).  
- **NLP Engineer** : traite le **texte** (classer, extraire).  
- **Computer Vision / Generative Image** : **images/vidéos** (détection, génération).  
- **Marketing/Growth Analyst** : **campagnes**, **A/B**, **CAC/LTV/ROAS**.  
- **Marketing Data Scientist** : **attribution** et **modèle de budget** (MMM).  
- **AI Product Manager** : besoin → métriques → feuille de route.

<br/>
<br/>



# PARTIE 1 — Recherche & définition des termes techniques 

**Objectif.** Vérifier que vous comprenez le vocabulaire Data/IA vu dans l’examen.

**Consigne.** Pour **chaque terme** ci-dessous :
1) Faire une recherche sur internet.
2) Donnez une **définition simple**.  
3) Ajoutez **1 exemple** (comment on l’utilise).  



## Liste des termes à définir

1. **Power BI**  
2. **KPI**  
3. **CSV**  
4. **Entrepôt (Data Warehouse)**  
5. **ETL**  
6. **ELT**  
7. **Modèle (ML)**  
8. **Churn**  
9. **F1**  
10. **AUC**  
11. **API**  
12. **FastAPI**  
13. **Docker**  
14. **Latence**  
15. **Airflow**  
16. **Pipeline (data)**  
17. **Alerte (monitoring)**  
18. **RAG**  
19. **Prompt**  
20. **Expériences modèles (experiment tracking)**  
21. **Drift (dérive)**  
22. **Réentraînement (retraining)**  
23. **Kafka**  
24. **Données en continu (streaming)**  
25. **Parquet**  
26. **A/B test**  
27. **Emailing**  
28. **Taux d’ouverture**

> **Option** (bonus +2 pts) : ajoutez **2 termes supplémentaires** liés à votre futur métier (ex. “dbt”, “Embeddings”, “Vector DB”) avec définitions + exemples + sources.




## Astuces rapides

- Visez des **phrases courtes** : “**ETL** = on transforme **avant** de charger”.  
- L’**exemple** doit montrer **comment** on s’en sert : “Avec **Airflow**, on lance chaque nuit le job d’ingestion, et on reçoit une **alerte** Slack si ça échoue.”  
- **Croisez 2 sources** si vous hésitez.  
- Privilégiez des **définitions d’usage**, pas des discours théoriques.

<br/>

# PARTIE 2 — Identifier le bon métier

**Consigne :** Choisissez **un seul** métier. Justifiez !

1) Tableaux de bord mensuels pour la direction (Power BI), mêmes KPI partout.  
→ [  ] BI Analyst/Dev  [  ] Data Analyst  [  ] Data Engineer  [  ] ML Engineer  [  ] Data Scientist

2) Lire chaque nuit des CSV, **nettoyer** puis **charger** propre dans l’entrepôt (**ETL**).  
→ [  ] BI  [  ] Data Analyst  [  ] **Data Engineer**  [  ] DS  [  ] MLE

3) **Charger brut** d’abord dans l’entrepôt puis **transformer dedans** (**ELT**).  
→ [  ] BI  [  ] DA  [  ] **Analytics Engineer**  [  ] DS  [  ] DE

4) Tester plusieurs **modèles** pour prédire le **churn**, comparer **F1/AUC**.  
→ [  ] DA  [  ] **Data Scientist**  [  ] MLE  [  ] BI  [  ] DE

5) Mettre un modèle en **API** rapide (FastAPI), **Docker**, surveiller **latence**.  
→ [  ] DA  [  ] DS  [  ] **ML Engineer**  [  ] DE  [  ] BI

6) **Airflow** : lancer un pipeline tous les jours, **alerte** si échec.  
→ [  ] BI  [  ] **Data Engineer**  [  ] DS  [  ] AE  [  ] MLE

7) Construire un **chat** qui cherche dans la doc et répond ( **RAG** + **prompts** ).  
→ [  ] DA  [  ] DS  [  ] **GenAI/LLM Dev**  [  ] MLOps  [  ] BI

8) Suivre **expériences modèles**, alerter en cas de **drift**, **réentraîner** automatiquement.  
→ [  ] DA  [  ] DS  [  ] MLE  [  ] **MLOps/Platform**  [  ] BI

9) **Kafka** : recevoir des données **en continu**, écrire en **Parquet**.  
→ [  ] DA  [  ] **Data Engineer (Big Data)**  [  ] DS  [  ] BI  [  ] AE

10) **A/B test** sur un emailing pour améliorer le taux d’ouverture.  
→ [  ] DA  [  ] **Marketing/Growth Analyst**  [  ] DS  [  ] BI  [  ] AE

<br/>


# PARTIE 3 — Associer Tâche ↔ Livrable ↔ Outil 

**Consigne :** Complétez **Métier**, **Livrable**, **Outil**.

| Tâche (simple) | Métier | Livrable | Outil principal |
|---|---|---|---|
| Tableau de bord ventes hebdo | … | Tableau de bord | Power BI / Tableau |
| Charger brut puis transformer dedans (ELT) | … | Tables prêtes | dbt |
| Planifier ingestion + nettoyage chaque nuit | … | Job planifié fiable | Airflow |
| Tester modèles churn et rapport simple | … | Notebook + résumé | scikit-learn |
| Exposer un modèle via une API rapide | … | Service en ligne | FastAPI + Docker |
| Alerte dérive + réentraînement auto | … | Pipeline MLOps | MLflow / Kubeflow |


<br/>

# PARTIE 4 — Vrai/Faux expliqué 

**Consigne :** Répondez **Vrai** ou **Faux** + **1 phrase** simple.

1) **ETL** = transformer les données **avant** de charger. → V/F + 1 phrase  
2) **ELT** = charger **brut** d’abord, transformer **dans l’entrepôt**. → V/F + 1 phrase  
3) **Kafka** sert à lire des fichiers Excel manuels une fois par mois. → V/F + 1 phrase  
4) **ML Engineer** pense à la **latence** et au **déploiement**. → V/F + 1 phrase  
5) **RAG** = répondre **après** avoir **cherché** des passages utiles. → V/F + 1 phrase

<br/>

# PARTIE 5 — Mini-cas 

Pour **chaque cas** : **Métier**, **Livrable**, **3 outils**, **2 KPI**, **1 risque**.

**Cas A — Doc interne**  
On veut un assistant qui répond aux questions des employés avec la doc interne.  
- Métier : ______  Livrable : ______  Outils (3) : ______  KPI (2) : ______  Risque (1) : ______

**Cas B — Données capteurs (continu)**  
Des machines envoient des données en **continu** ; on veut stocker et analyser plus tard.  
- Métier : ______  Livrable : ______  Outils (3) : ______  KPI (2) : ______  Risque (1) : ______

**Cas C — Direction (hebdomadaire)**  
La direction veut un tableau simple des ventes par pays et produit, **chaque semaine**.  
- Métier : ______  Livrable : ______  Outils (3) : ______  KPI (2) : ______  Risque (1) : ______

<br/>

# PARTIE 6 — Ordre des étapes d’un petit projet ( **/8** )

**Consigne :** Numérotez **1 à 8**.

- [ ] Définir le besoin + les KPI  
- [ ] Récupérer et **nettoyer** les données  
- [ ] **Séparer** entraînement/test (si modèle)  
- [ ] **Créer** les variables utiles (features)  
- [ ] **Entraîner** puis **évaluer** le modèle (si applicable)  
- [ ] **Préparer** les tables pour l’analyse (AE/dbt)  
- [ ] **Mettre en ligne** (API ou tableau de bord)  
- [ ] **Surveiller** et **améliorer** (erreurs, coût, drift)

<br/>





# PARTIE 7 — Se lancer en Data & IA

Cochez **une seule** réponse.

1) Pour un **débutant complet**, la priorité les 3 premiers mois :  
A. Kubernetes  B. Python bases + SQL  C. Fine-tuning LLM  D. Vision par ordinateur

2) La **phase 1 (Fondations)** inclut surtout :  
A. Python/pandas, statistiques, SQL  B. Docker  C. MMM marketing  D. Négociation salaire

3) La **phase 4 (Portfolio)** demande :  
A. 1 projet sans README  B. 3–5 projets complets documentés  C. Aucun projet  D. Uniquement des certificats

4) **Networking & visibilité** veut dire :  
A. Éviter LinkedIn  B. Optimiser LinkedIn, participer à des events, publier  C. Effacer GitHub  D. Poster des mèmes



> Répondez **VRAI** ou **FAUX** et ajoutez **1 phrase**.


5) Le portfolio doit rester **privé** pour éviter la copie.  
Réponse : _______ — Phrase : _______________________________________



6) Pour postuler, il faut maîtriser **100%** des compétences de l’offre.  
Réponse : _______ — Phrase : _______________________________________

7) “Pratiquer un peu **tous les jours**” est mieux que 5h **une fois** par semaine.  
Réponse : _______ — Phrase : _______________________________________


8) Donnez **2 idées de projets** portfolio *simples mais utiles* dans **un secteur** (ex. marketing/finance/RH).  
Réponse : ____________________________________________________________________  
______________________________________________________________________________







<br/>


## PARTIE 8 — Recherche LinkedIn & analyse d’offres (terrain) 

**Objectif.** Savoir cibler un métier, analyser des offres réelles et en déduire un plan d’action (compétences + portfolio).

**Consignes.**
1) Choisissez **UN** métier Data/IA (exemples : *Développeur Cloud*, *Ingénieur·e Databricks*, *Data Analyst BI*, *ML Engineer*, *GenAI Developer*, etc....).  
2) Trouvez **3 offres réelles** sur **LinkedIn** pour **le même métier** :
   - **1** à **Montréal (QC)**  
   - **1** à **Toronto (ON)**  
   - **1** **au Japon** (Tokyo, Osaka, etc.)
3) Pour chaque offre, remplissez le tableau ci-dessous puis faites la synthèse demandée.

> Rappel : **reformulez** les informations avec vos mots. **Citez le lien** de l’annonce et la **date de consultation**.  


### G1 — Fiche offre (à dupliquer ×3 : Montréal / Toronto / Japon)

- **Métier ciblé :** ____________________  
- **Ville / Pays :** ____________________  
- **Entreprise (secteur / taille si indiqué) :** ____________________  
- **Type de contrat :** ☐ Temps plein ☐ Contrat ☐ Stage/Alternance  
- **Mode de travail :** ☐ Sur site ☐ Hybride ☐ Remote  
- **Niveau :** ☐ Junior ☐ Intermédiaire ☐ Senior ☐ Non précisé  
- **Langues requises :** ____________________  
- **Visa / Sponsorship mentionné :** ☐ Oui ☐ Non ☐ Non précisé  
- **Salaire (si indiqué) :** ____________________  
- **Lien LinkedIn (URL courte) :** ____________________  
- **Date annonce / Date de consultation :** ____ / ____

**Compétences clés demandées (max 10, cochez si “must have”)**
- ☐ SQL  ☐ Python  ☐ Spark  ☐ Databricks  ☐ Delta Lake  ☐ Unity Catalog  
- ☐ Airflow  ☐ dbt  ☐ MLflow  ☐ Streaming (Structured Streaming/Kafka)  
- ☐ AWS ☐ Azure ☐ GCP  ☐ Power BI/Tableau  ☐ Autre : _______________

**Mots-clés spécifiques (recopiez tels quels s’ils apparaissent)**
- Lakehouse / Delta Lake / Unity Catalog / Quality Gates / CDC / SCD / ETL / ELT / Governance / Cost Optimization / SLA / SLO / Monitoring / Observability / Lineage / Security / PII / etc.  
→ _______________________________________________________________________

**Résumé de l’annonce (3–5 lignes, vos mots)**
- _______________________________________________________________________
- _______________________________________________________________________
- _______________________________________________________________________



### G2 — Tableau comparatif (synthèse des 3 offres)

| Critère | Montréal | Toronto | Japon |
|---|---|---|---|
| Entreprise (secteur, taille) | | | |
| Seniorité visée | | | |
| Mode de travail (site/hybride/remote) | | | |
| Cloud/Stack (AWS/Azure/GCP) | | | |
| Data stack (Databricks/Spark/dbt/Delta) | | | |
| Orchestration (Airflow/Jobs) | | | |
| BI/Analytics (Power BI, Tableau…) | | | |
| Exigences langue | | | |
| Visa/Sponsorship | | | |
| Salaire (si visible) | | | |





## AIDE MÉMOIRE (mots → métier)

- **Tableau de bord/KPI** → BI / Data Analyst  
- **Tuyaux + gros volumes** → Data Engineer  
- **Tables propres/testées dans l’entrepôt** → Analytics Engineer  
- **Prédire/expérimenter** → Data Scientist  
- **API rapide et fiable** → ML Engineer  
- **Automatiser/monitorer les modèles** → MLOps  
- **LLM + recherche de documents** → GenAI/LLM Dev  
- **Texte** → NLP Engineer  
- **Images/Vidéos** → Computer Vision / Génération d’images  
- **Campagnes/attribution/budget** → Marketing Analyst / Marketing DS



# Annexe utiles:


* **A/B (test A/B)**
  Expérimentation où l’on compare **deux variantes** (A vs B) d’une même campagne/page/annonce pour voir laquelle performe mieux sur un **indicateur unique** (ex. conversion).
  Règle d’or : 1 changement à la fois, échantillon suffisant, arrêt basé sur la **significativité** (pas “au feeling”).

* **CAC (Customer Acquisition Cost / Coût d’acquisition client)**
  **Combien coûte** en moyenne l’acquisition d’1 client.
  **Formule** : ( \text{CAC} = \dfrac{\text{Dépenses marketing+vente sur une période}}{\text{Nombre de nouveaux clients}} )

* **LTV (Lifetime Value / Valeur vie client)**
  **Valeur totale** qu’un client génère sur toute sa relation.
  **Formule simple** : ( \text{LTV} = \text{Panier moyen} \times \text{Marge} \times \text{Nombre d’achats sur la durée} )
  (En SaaS, on utilise souvent ( \text{LTV} = \dfrac{\text{ARPA} \times \text{Marge}}{\text{Taux de churn}} ).)

* **ROAS (Return On Ad Spend / Retour sur dépenses publicitaires)**
  **Recettes générées** pour **1 unité** de budget publicitaire.
  **Formule** : ( \text{ROAS} = \dfrac{\text{Revenus attribués aux pubs}}{\text{Dépenses pubs}} )
  Lecture : ROAS = 4 signifie 1 $ dépensé → 4 $ de revenus.

### Mini-exemple relié

* Dépenses publicitaires mensuelles : 10 000 $
* Nouveaux clients : 200 → **CAC = 10 000 / 200 = 50 $**
* Par client : panier moyen 60 $, marge 40 %, 5 achats sur la durée → **LTV = 60 × 0,4 × 5 = 120 $**
* Revenus attribués aux pubs : 40 000 $ → **ROAS = 40 000 / 10 000 = 4**
* Lecture “Growth” : **LTV/CAC = 120 / 50 = 2,4** (souvent on vise > 3 pour un modèle très sain; 2–3 peut être acceptable selon le cash-flow et le churn).

### À retenir pour un/une Marketing/Growth Analyst

* Prioriser des **tests A/B** propres (un KPI, un changement, échantillons suffisants).
* Suivre **CAC**, **LTV**, **LTV/CAC** et **ROAS** ensemble (pas isolément).
* Agir : baisser le **CAC** (meilleur ciblage, créas), **augmenter le LTV** (upsell, rétention), et optimiser le **ROAS** (allocation budgétaire vers les canaux/annonces gagnants).

