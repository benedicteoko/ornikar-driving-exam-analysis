## Présentation du projet

Ce projet analyse les données d'entraînement de la plateforme d'examen théorique du permis de conduire d'Ornikar.

L'objectif est de comprendre l'engagement des candidats et d'identifier les facteurs associés à la réussite à l'examen théorique du permis de conduire.

## Tableau de bord interactif

🚀 Découvrez le tableau de bord interactif :

👉 https://lookerstudio.google.com/reporting/(https://lookerstudio.google.com/reporting/6bd8fea1-d1b3-4583-a969-183af3b98189)


## Requêtes SQL

Les requêtes SQL utilisées pour cette analyse sont disponibles dans le fichier suivant :

- `ornikar_analysis.sql`

Le jeu de données utilisé dans ce projet fait partie d'un jeu de données d'entraînement et ne peut être partagé publiquement. Cependant, certaines requêtes SQL utilisées pour l'analyse sont incluses dans ce dépôt.

Exemple

```sql
SELECT
  first_product,
  COUNT(*) AS number_users
FROM `data-analytics-essentials-sc.ornikar.consumption`
GROUP BY first_product
ORDER BY number_users DESC;
```

- La plupart des candidats achètent le produit **Code pur**.
- La réussite à l'examen semble davantage liée à **l'engagement et à la pratique** qu'au type de produit.
- Les candidats qui effectuent davantage de séries d'entraînement ont tendance à obtenir de meilleurs taux de réussite.
- La moyenne des scores obtenus aux **5 dernières séries d'entraînement** semble être un indicateur fiable du niveau de préparation à l'examen.

- ## Outils

- SQL (BigQuery)
- Looker Studio
- GitHub

- Analyse de données
