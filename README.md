# Pipeline Big Data avec Apache Airflow

Un pipeline Big Data simple orchestré avec Apache Airflow, de l'ingestion des données à l'analyse.

## Architecture du Pipeline

```
Sources → Ingestion → Data Lake (BRUT) → Traitement → Lakehouse (CURATED) → Analyse
```

- **Data Lake (BRUT)**: Stockage des données brutes
- **Traitement**: Nettoyage et structuration des données
- **Data Lakehouse (CURATED)**: Données prêtes pour l'analyse
- **Airflow**: Orchestration et surveillance

## Interface Web Airflow

**URL**: `http://localhost:8080`
**Connexion**: airflow / airflow

![Connexion Airflow](screens/image-1.png)

## Exécution via l'Interface Airflow

### 1. Activation du DAG

![Activation du DAG](screens/image-2.png)

### 2. Déclenchement Manuel

![Déclenchement du DAG](screens/image-3.png)

### 3. Vue Graphique

Visualisez les dépendances des tâches et le flux d'exécution.

![Vue Graphique](screens/image-4.png)

### 4. Surveillance de l'Exécution

- Vert : Succès
- Rouge : Échec
- Bleu : En cours

![État de l'Exécution](screens/image7.png)

### 5. Inspection des Logs

Consultez les logs détaillés pour chaque tâche.

![Logs des Tâches](screens/image-5.png)

## Conclusion

Cet atelier démontre comment construire un pipeline Big Data simple, orchestrer les étapes avec Apache Airflow, surveiller l'exécution via une interface web, et vérifier les résultats dans le Data Lake et le Data Lakehouse. Il fournit une fondation idéale avant de passer à des pipelines Big Data avancés avec Spark, Hadoop et des outils BI.
