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


Explication des graphiques du dashboard
 1. Cartes KPI – Indicateurs clés

Ces cartes affichent une vue synthétique de l’état global du projet.
Total PV (Planned Value) :
Représente le budget prévu du projet à une date donnée.
Total EV (Earned Value) :
Représente la valeur réelle du travail effectivement réalisé.
Total AC (Actual Cost) :
Correspond au coût réel dépensé pour le projet.
CPI (Cost Performance Index) :
Indicateur de performance des coûts.
CPI < 1 : dépassement budgétaire
CPI = 1 : budget respecté
CPI > 1 : économies réalisées

Ces cartes permettent de comprendre immédiatement la situation financière du projet.
2. Courbes en S – Évolution PV, EV et AC par date

Ce graphique montre l’évolution dans le temps des trois indicateurs principaux :
PV : planification initiale
EV : avancement réel
AC : coûts réellement engagés

L’analyse visuelle permet de :
détecter un retard lorsque EV est en dessous de PV
détecter un dépassement de budget lorsque AC est au-dessus de EV
C’est le graphique central de la méthode EVM.

3. Graphique Total EV et Total AC par Lot WBS
Ce graphique compare la valeur acquise (EV) et le coût réel (AC) pour chaque lot de travail (WBS).
Il permet :

d’identifier les lots les plus coûteux
de repérer précisément où se situent les dérives
d’aider à la prise de décision corrective ciblée
Très utile pour les chefs de projet.

4. Jauge CPI – Performance des coûts
La jauge CPI permet une lecture immédiate de la performance budgétaire :

Zone verte : bonne performance
Zone orange : vigilance
Zone rouge : performance critique
Une cible à 1 est utilisée comme référence.

5. Jauge SPI – Performance des délais
La jauge SPI mesure la performance du planning :
SPI < 1 : retard
SPI = 1 : planning respecté
SPI > 1 : avance

Elle permet d’évaluer si le projet avance comme prévu dans le temps.

6. Tableau récapitulatif des indicateurs
Ce tableau présente les valeurs numériques détaillées :
PV total
Véhicules électriques à part entière
Climatisation totale
CV (Variance des coûts)
IPC

Il sert à :
valider les chiffres affichés dans les graphiques
fournir une analyse chiffrée précise
être utilisé comme base pour des rapports détaillés

7. Infobulles (Bulles d'information)
Des info-bulles interactives ont été ajoutées sur certains graphiques.
Elles permettent :
d’afficher des détails supplémentaires au survol
d’enrichir l’analyse sans surcharger le dashboard principal
d’améliorer l’expérience utilisateur

8. Alerte automatique de performance

Une alerte visuelle apparaît lorsque :
IPC < 0,95
Cette alerte permet d’attirer immédiatement l’attention sur une situation critique, facilitant une réaction rapide.

Conclusion
Ce tableau de bord Power BI permet :
un suivi budgétaire clair
une analyse visuelle rapide
une aide à la décision efficace
Il s’agit d’un projet de démonstration, mais la logique est directement applicable à un contexte réel de gestion de projet.

## Réalisé par
**Cindy K. Njanpouop**  
