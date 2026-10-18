
# Analyse SQL de la Santé Mentale des Étudiants Internationaux

## 📌 Contexte du Projet
Ce projet consiste en une exploration et une analyse de données (réalisée via DataCamp) visant à évaluer l'impact de la durée de séjour sur la santé mentale des étudiants internationaux. L'objectif est d'utiliser des requêtes SQL pour extraire, transformer et analyser des indicateurs psychologiques clés à partir d'une base de données d'étudiants.

## 🎯 Objectifs de l'Analyse
L'enjeu principal est de déterminer comment la durée de séjour (`stay`) influence les scores moyens liés aux diagnostics de santé mentale, spécifiquement pour les profils internationaux. Les trois métriques évaluées sont :
1. Le niveau de dépression.
2. Le sentiment de connexion sociale.
3. Le stress d'acculturation.

## 🛠️ Outils et Compétences Techniques
* **Langage :** SQL (PostgreSQL)
* **Techniques appliquées :** 
  * Filtrage conditionnel (`WHERE`)
  * Fonctions d'agrégation (`COUNT`, `AVG`)
  * Formatage numérique (`ROUND`)
  * Groupement des données (`GROUP BY`)
  * Tri descendant (`ORDER BY`)

## 📊 Structure des Données
L'analyse s'appuie sur les colonnes suivantes de la table `students` :
* `inter_dom` : Type d'étudiant (filtre appliqué sur `'Inter'`).
* `stay` : Durée du séjour en années.
* `todep` : Score total de dépression (test PHQ-9).
* `tosc` : Score total de connexion sociale (test SCS).
* `toas` : Score total de stress d'acculturation (test ASISS).

## 🚀 Synthèse des Résultats
Le script `query.sql` génère un tableau de bord synthétique (9 lignes) qui regroupe la population par durée de séjour. Pour chaque groupe, il calcule la taille de la cohorte ainsi que les moyennes précises (à deux décimales) des trois scores de santé mentale. Les données sont triées de la plus longue à la plus courte durée de séjour pour mettre en évidence les tendances d'évolution au fil des années.

---
*Projet de portfolio réalisé par Abdoul Kader Junior KEBE — Élève Ingénieur en Big Data et Intelligence Artificielle.*
