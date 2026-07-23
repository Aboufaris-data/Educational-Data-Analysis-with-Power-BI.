# Tableau de Bord Scolaire — Power BI

Tableau de bord interactif développé sous **Power BI** pour le suivi et l'analyse de la performance académique d'un établissement scolaire : élèves, enseignants, cours et résultats.

---

## Objectif du Projet

Ce tableau de bord centralise les données scolaires (élèves, enseignants, matières, résultats) afin de fournir à la direction pédagogique une vision claire et actionnable sur :

- La réussite et les risques académiques des élèves
- La performance et la charge de travail du corps enseignant
- L'évolution des résultats par filière, section et année
- Des recommandations stratégiques basées sur les données

---

## Structure du Rapport

Le rapport Power BI est organisé en **4 pages** :

### Vue d'Ensemble — Élèves
- **KPIs clés** : Total Élèves, Taux de Réussite, Moyenne Générale, Élèves à Risque
- **Corrélation** entre la Moyenne Générale et le Nombre d'Absences (nuage de points)
- **Répartition des Élèves par Statut Académique** (Actif, Diplômé, Redoublant, Transféré) — graphique en anneau
- **Évolution des Inscriptions par Année** (courbe 2020–2026)
- **Répartition des Élèves par Niveau Scolaire et Filière** (histogramme groupé : A, B, Économie, Littérature, Sciences)
- **Filtres (slicers)** : Matière, Filière/Section, Année d'Inscription, Niveau Scolaire, Type de Contrat

### Enseignants
- **Distribution des Enseignants par Note d'Évaluation** (histogramme, échelle 1.5 à 5.0)
- **Effectif des Enseignants par Matière et Type de Contrat** (Contractuel, Titulaire, Vacataire)
- **Liste Détaillée des Évaluations par Enseignant** (table : Nom, Matière, Type de Contrat, Note d'Évaluation)
- **Filtres** : Année d'Inscription, Matière, Niveau Scolaire, Filière/Section

### Cours & Résultats
- **KPIs** : Total Matières, Note d'Évaluation Moyenne, Taux de Réussite
- **Évolution de la Moyenne Générale par Année et Filière** (courbes multi-séries 2019–2023)
- **Répartition des Élèves par Matière et Statut** (histogramme empilé)
- **Table récapitulative** : Moyenne Générale par matière
- **Filtres** : Niveau Scolaire, Matière, Filière/Section, Année d'Inscription

### Insights et Recommandations Stratégiques
Synthèse analytique et recommandations pour la direction :

| Axe | Constat | Recommandation |
|---|---|---|
| **Résultats par Filière** | Taux d'échec prononcé dans certaines filières scientifiques et techniques | Sessions de soutien ciblées et révision des méthodes pédagogiques |
| **Charge Horaire des Enseignants** | Déséquilibre structurel entre enseignants vacataires et titulaires | Redistribution équitable des volumes horaires |
| **Profil des Élèves à Risque** | Corrélation entre +15 absences et moyenne < 10 | Système d'alerte précoce et entretiens de cadrage |
| **Plan d'Action Institutionnel** | Besoin de visibilité en temps réel | Automatisation du tableau de bord pour la direction |

---

## Indicateurs Clés (KPIs)

| Indicateur | Valeur |
|---|---|
| Total Élèves | 115 |
| Taux de Réussite | 63.00% |
| Moyenne Générale | 12 |
| Élèves à Risque | 43 |
| Total Matières | 10 |
| Note d'Évaluation Moyenne | 3.16 |

---

## Modèle de Données

Le modèle s'articule autour des entités suivantes :

- **Élèves** : nom, filière/section, niveau scolaire, année d'inscription, statut académique, moyenne générale, nombre d'absences
- **Enseignants** : nom complet, matière, type de contrat, note d'évaluation
- **Matières / Cours** : matière, filière, statut des élèves, résultats

---

## Technologies Utilisées

- **Power BI Desktop** — conception du rapport et des visuels
- **DAX** — mesures et KPIs calculés
- **Power Query** — préparation et nettoyage des données

---

## Installation & Utilisation

### Prérequis
- [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (version récente recommandée)
- Fichier source de données (Excel/CSV/base de données) référencé par le rapport

### Étapes
1. Cloner le dépôt :
   ```bash
   git clone https://github.com/<votre-utilisateur>/<nom-du-repo>.git
   cd <nom-du-repo>
   ```
2. Ouvrir le fichier `.pbix` avec **Power BI Desktop**.
3. Mettre à jour la source de données si nécessaire (`Accueil > Transformer les données > Paramètres source de données`).
4. Actualiser les données (`Accueil > Actualiser`).
5. Explorer les pages via les onglets en bas du rapport.

### Utilisation dans VS Code
Ce dépôt peut être versionné et documenté via VS Code :
- Utilisez l'extension **Power BI** ou consultez le fichier `.pbix` en tant que binaire versionné (Git LFS recommandé pour les fichiers volumineux).
- Le fichier `README.md` et toute documentation complémentaire (notes DAX, dictionnaire de données) peuvent être édités directement dans VS Code.

---

## Arborescence Suggérée

```
├── README.md
├── data/
│   └── donnees_scolaires.xlsx
├── report/
│   └── tableau_de_bord_scolaire.pbix
└── docs/
    └── dictionnaire_donnees.md
```

---

## Confidentialité

Les données utilisées dans ce projet sont anonymisées / fictives et destinées uniquement à des fins de démonstration et d'apprentissage.

---

## Licence

Ce projet est distribué sous licence MIT. Voir le fichier `LICENSE` pour plus de détails.

---

## ✍️ Auteur

Développé par **[ABoufaris Khalid]** — dans le cadre d'un projet d'analyse de données scolaires avec Power BI.
