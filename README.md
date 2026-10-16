# TP-2-Etude-de-cas

# Analyse Big Data des accidents de la route avec PySpark

Reprise commentée de l'article *« Big data Analysis of Road Crash Data using PySpark with PySpark Tutorial »*
(Rakesh Nain, Medium) : accidents de la route en Australie-Méridionale, 2012-2019.

**Rendu : [`etude_de_cas.ipynb`](analyse_accidents_pyspark.ipynb)**

Apports par rapport au code original :
- explications des notions Spark (RDD, partitions, transformations/actions, jointures, UDF, Spark SQL) ;
- lecture commentée de chaque résultat et de chaque figure ;
- correction de 5 erreurs trouvées dans l'article (indices de colonnes, découpage CSV, double comptage
  après jointure, requêtes RDD/DataFrame/SQL incohérentes), avec vérification par `assert` ;
- comparaison RDD / DataFrame / Spark SQL (plan d'exécution et temps).

## Reproduire
1. Télécharger les données depuis le dépôt de l'auteur :
   https://github.com/RakeshNain/Big-data-Analysis-of-Road-Crash-Data-using-PySpark-with-PySpark-Tutorial
   (dossiers `units_data/`, `crash_data/` et `data for given tutorials/`), et les placer à côté du notebook.
2. `pip install "pyspark==3.5.*" pandas matplotlib` ; Spark 3.5 nécessite Java 8, 11 ou 17.
3. Exécuter toutes les cellules du notebook.
