# Contexte

## Introduction

Cette documentation décrit la méthodologie et les données utilisées pour le calcul des indicateurs de marché immobilier et de stock dans le cadre du recul du trait de côte.

Une première étude nationale réalisée en 2023 avec la DTecREM du Cerema a permis de poser les fondations de la méthodologie actuellement employée, qui est toujours en cours d'évolution afin d'améliorer la précision des résultats et la pertinence des indicateurs obtenus.

En particulier, la méthodologie décrite ici est celle employée à l'occasion de l'étude commandée au Cerema Hauts-de-France par l'Établissement Public Foncier des Hauts-de-France (fin 2025).

## Objectifs

Pour différents périmètres d'étude, l'objectif est de déterminer :  

* des indicateurs des marchés fonciers et immobiliers, pour chaque période d'étude : volumes de transactions, prix de vente, activité du marché, évolution des prix depuis 2010, catégories d'acheteurs et de vendeurs les plus représentées,
* des indicateurs de stock, pour une année donnée (ici 2024) : nombre de logements par type et par période de construction, par type d'occupation et mode d'occupation (résidences principales, secondaires, logements vacants)…
* des indicateurs de contexte, pour une année donnée : les 3ème, 5ème (médiane) et 7ème déciles de revenus déclarés sont ajoutés.

Pour chaque périmètre d'étude, les indicateurs sont déclinés sur des échelles d'agrégation diverses : commune, EPCI, périmètre entier...

Les volets suivants permettront d'affiner et d'ajouter des informations, en précisant notamment les équipements publics situés dans le périmètre d'étude, par exemple.

## Données mobilisées

Le calcul de ces indicateurs mobilise les bases de données suivantes :

* Fichiers fonciers 2024 (Cerema),
* DV3F 2025-1 (Cerema),
* ADMIN EXPRESS COG2024 (IGN) pour la détection des EPCI,
* Table de conversion des € base 100 2015 (INSEE),
* Filosofi 2021 (INSEE),
* Inventaire des zones d'activités économiques (Région Hauts-de-France).

Les bases de données issues de données fiscales sont le socle de ce traitement. Seules les communes cadastrées peuvent donc être correctement traitées par cette routine.

## Scénarios étudiés

Quatre scénarios ont été étudiés pour la production des indicateurs du volet 1.  

### Périodes d'étude

Pour tous les scénarios, l'année de référence utilisée pour le calcul du stock est 2024. Les périodes d'études suivantes ont été choisies pour calculer les indicateurs des marchés fonciers et immobiliers :

* pour les prix et les volumes : 2010-2012, 2014-2016, 2019-2021, 2022-2024,
* pour l'activité du marché : toutes les périodes de trois ans glissants depuis 2018.

Le calcul des indicateurs sur trois ans plutôt qu'un seul permet une significativité accrue en raison du faible nombre d'individus sur les échantillons géographiques de petite taille pour une seule année.

### Scénario 1 : bande des 200 m

Il s'agit d'une bande de 200 m le long du littoral des Hauts-de-France. Cette bande a été calculée par le Cerema Hauts-de-France à partir de la limite Terre-mer, version novembre 2021, en ignorant les polygones de moins de 100 m² (îlots, parties de terres partiellement immergées…).

Les indicateurs ont été agrégés à l'échelle des communes situées dans cette bande et sur l'ensemble du périmètre.

### Scénario 2 : communes littorales sauf bande des 200 m

Il s'agit de 54 communes considérées "littorales" par l'EPF Hauts-de-France, auxquelles ont été soustraites la bande des 200 m.

Les indicateurs ont été agrégés à l'échelle des communes littorales et sur l'ensemble du périmètre.

### Scénario 3 : région Hauts-de-France

Il s'agit de l'ensemble de la région Hauts-de-France.

Les indicateurs ont été agrégés à l'échelle des communes littorales, des EPCI littoraux et sur l'ensemble du périmètre. Il y a 9 EPCI considérés littoraux dans la région : CA du Boulonnais, CA Grand Calais Terres et Mers, CC Ponthieu-Marquenterre, CC des Villes Sœurs, CU de Dunkerque, CA de la Baie de Somme, CA des Deux Baies en Montreuillois, CC de la Région d'Audruicq, CC de la Terre des Deux Caps.