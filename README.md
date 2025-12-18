# Dashboard Power BI – Contrôle Budgétaire & Performance Projet (EVM)

## Objectif du projet
Ce projet a pour objectif de réaliser un tableau de bord Power BI permettant
le suivi budgétaire et la performance d’un projet à l’aide de la méthode
**Earned Value Management (EVM)**.

Il permet de visualiser rapidement :
- l’avancement réel du projet
- les écarts de coûts et de délais
- les indicateurs de performance clés

## Données utilisées
Les données proviennent d’un fichier CSV simulant le suivi d’un projet et contiennent :
- Date
- Semaine
- Lot WBS
- Type de coût (PV, EV, AC)
- Valeur

Fichier utilisé : `project_evm_data.csv`

## Indicateurs calculés (DAX)
Les mesures suivantes ont été créées dans Power BI :
- **Total PV** (Planned Value)
- **Total EV** (Earned Value)
- **Total AC** (Actual Cost)
- **CPI** (Cost Performance Index)
- **SPI** (Schedule Performance Index)
- **CV** (Cost Variance)
- **SV** (Schedule Variance)
- **EAC** (Estimate At Completion)

Une alerte visuelle est déclenchée lorsque **CPI < 0.95**.

## Visualisations réalisées
Le dashboard comprend :
- Cartes KPI (PV, EV, AC, CPI)
- Courbes en S (PV, EV, AC)
- Graphique par lot WBS
- Jauges CPI et SPI
- Tableau des écarts
- Filtres interactifs (Date, Semaine, Lot WBS)
- Info-bulles dynamiques (Tooltips)

## Outils utilisés
- **Power BI Desktop**
- **DAX**
- **Fichier CSV**

## Réalisé par
**Cindy K. Njanpouop**  
