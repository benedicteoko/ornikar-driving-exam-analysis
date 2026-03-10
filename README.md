Ce projet analyse les données d'entraînement de la plateforme d'examen théorique du permis de conduire d'Ornikar à l'aide de SQL (BigQuery) et de Looker Studio.

L'analyse porte sur l'engagement des candidats, leurs performances lors des entraînements et les facteurs comportementaux associés à la réussite à l'examen.

### Training Engagement

![Dashboard](dashboard_consumption_ornikar.png)

### Exam Results

![Dashboard](dashboard_exam_ornikar.png)


292
## Requêtes SQL

Les requêtes SQL utilisées pour cette analyse sont disponibles dans le fichier suivant :

- `ornikar_analysis.sql`

Le jeu de données utilisé dans ce projet fait partie d'un jeu de données d'entraînement et ne peut être partagé publiquement. Cependant, toutes les requêtes SQL utilisées pour l'analyse sont incluses dans ce dépôt.
###Exemple

```sql
SELECT
  first_product,
  COUNT(*) AS number_users
FROM `data-analytics-essentials-sc.ornikar.consumption`
GROUP BY first_product
ORDER BY number_users DESC;

  
