# Rapport d'Analyse Power BI : Optimisation de la Gestion des Clients, Employés et Shifts

## 1. Introduction
Ce rapport vise à présenter les résultats d'une analyse approfondie des données provenant de trois fichiers CSV : **Clients**, **Employees**, et **Shifts**. L’objectif est de fournir des insights exploitables pour améliorer la gestion des ressources humaines, la satisfaction des clients, et l’optimisation des plannings.

---

## 2. Résumé des Données

### 2.1 Sources de Données
- **Clients.csv** : Informations démographiques, statuts, et historique d’interactions.
- **Employees.csv** : Rôles, ancienneté, et localisation.
- **Shifts.csv** : Horaires de travail, durée des shifts, et données de pointage.

### 2.2 Qualité des Données
- **Valeurs manquantes** : 5% des dates de fin de shift manquantes dans le fichier `Shifts.csv`.
- **Doublons** : Existence de doublons au niveau des clients.
- **Incohérences** : Format de date non uniforme corrigé dans `Clients.csv`.

---

## 3. Modélisation et Relations
Les relations entre les tables ont été définies comme suit :
- **Clients ↔ Shifts** : Relation indirecte via les employés responsables.
- **Employees ↔ Shifts** : Relation 1:N basée sur l'identifiant des employés.

### Mesures DAX Créées
- **TotalShifts** : Nombre total de shifts effectués.
- **AverageShiftDuration** : Durée moyenne des shifts (en heures).
- **ClientGrowthRate** : Taux de croissance mensuel des clients.

---

## 4. Insights Clés

### Tendances Clients
- La base de clients s’élargit, mais la rétention des clients *Basic* reste un défi (40% quittent après 3 mois).

### Optimisation des Shifts
- Une sur-représentation des employés dans les shifts de nuit entraîne des coûts supplémentaires.

### Performance des Employés
- Les employés travaillant depuis plus de 1 an ont un taux d’efficacité supérieur de 20%.

---

## 5. Recommandations

### Optimiser les Plannings
- Rééquilibrer les shifts de nuit en affectant davantage d’employés expérimentés pour réduire les coûts.

### Améliorer la Rétention des Clients
- Lancer un programme de fidélité pour les clients *Basic* afin d’augmenter leur durée de vie.

### Former les Nouveaux Employés
- Développer un programme de formation pour améliorer la performance des employés ayant moins de 2 ans d’ancienneté.

---

## 6. Conclusion
La mise en œuvre de ces recommandations devrait permettre d'améliorer :
- La satisfaction des clients.
- L’efficacité des employés.
- La rentabilité globale.

Un suivi régulier des **KPIs** via Power BI est recommandé pour ajuster les stratégies en temps réel.
