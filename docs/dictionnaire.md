# Dictionnaire

Cette page propose un lexique de correspondance entre nom de variable et signification, pour l'ensemble des tables de résultats produits par la routine de calcul.

## Table `locaux_mutes_plusieurs_fois`

| Nom de variable                       | Description                                                                                                 |
| ------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| idmutation                            | Identifiant de mutation                                                                                     |
| nbmut                                 | Nombre de mutations de ce local seul depuis 2010                                                            |
| rang_mutation                         | Numéro de la mutation par ordre chronologique d'événement                                                   |
| datemut                               | Date de la mutation                                                                                         |
| anneemut                              | Année de la mutation                                                                                        |
| annees_depuis_precedent               | Nombre d'années depuis la muation précédente                                                                |
| prix                                  | Prix de vente à l'année de la mutation (€)                                                                  |
| pxm2                                  | Prix de vente au m² à l'année de la mutation (€/m²)                                                         |
| prix_2024                             | Prix de vente converti (€2024)                                                                              |
| pxm2_2024                             | Prix de vente au m² converti (€2024/m²)                                                                     |
| variation_nominale_prix_precedent     | Différence entre le prix de vente et le prix de vente de la mutation précédente (€2024)                     |
| variation_nominale_prix_pct_precedent | Variation du prix de vente par rapport au prix de vente de la mutation précédente (%)                       |
| variation_nominale_prix_initial       | Différence entre le prix de vente et le prix de vente de la première mutation enregistrée dans DV3F (€2024) |
| variation_nominale_prix_pct_initial   | Variation du prix de vente par rapport au prix de vente de la première mutation enregistrée dans DV3F (%)   |
| tcam_reel_pct                         | Taux de croissance annuel moyen réel (%)                                                                    |
| impact_inflation_pct                  | Impact de l'inflation dans la variation du prix (%)                                                         |

## Table `prix_volumes`

| Nom de variable                 | Description                                                       |
| ------------------------------- | ----------------------------------------------------------------- |
| periode                         | Année du milieu de la période d'étude (2011 = 2010 - 2012)        |
| code                            | Code géographique ou identifiant de l'unité d'agrégation          |
| nom                             | Libellé de l'unité d'agrégation                                   |
| nb_mutations                    | Nombre de mutations                                               |
| valeurfonc_totale               | Valeur foncière totale des mutations (€)                          |
| surface_totale                  | Surface totale vendue cumulée (m²)                                |
| nb_foncier_nu                   | Nombre de mutations de foncier nu                                 |
| surface_totale_foncier_nu       | Surface totale de terrains de mutations de fonciers nus (m²)      |
| nbtrans_maisons                 | Nombre de transactions de maisons                                 |
| nbtrans_appts                   | Nombre de transactions d'appartements                             |
| nbtrans_act                     | Nombre de transactions de locaux d'activité                       |
| nbtrans_act_tertiaire           | Nombre de transactions de locaux d'activité tertiaire             |
| nblocmut_maisons                | Nombre de maisons qui ont muté                                    |
| px_med_maison                   | Prix médian d'une maison (€)                                      |
| nblocmut_appts                  | Nombre d'appartements qui ont muté                                |
| px_med_appt                     | Prix médian d'un appartement (€)                                  |
| nblocmut_act                    | Nombre de locaux d'activité qui ont muté                          |
| nblocmut_act_tertiaire          | Nombre de locaux d'activité tertiaire qui ont muté                |
| nb_mutations_foncier_nu_tab     | Nombre de mutations de fonciers nus supposés terrains à bâtir     |
| pxm2_median_foncier_nu_tab      | Prix médian des fonciers nus supposés terrain à bâtir (€/m²)      |
| nb_mutations_foncier_nu_non_tab | Nombre de mutations de fonciers nus supposés non terrains à bâtir |
| pxm2_median_foncier_nu_non_tab  | Prix médian des fonciers nus non supposés terrain à bâtir (€/m²)  |
|                                 |

## Table `ratio_activite`

| Nom de variable | Description                                                           |
| --------------- | --------------------------------------------------------------------- |
| periode         | Année du milieu de la période d'étude (2011 = 2010 - 2012)            |
| code            | Code géographique ou identifiant de l'unité d'agrégation              |
| nom             | Libellé de l'unité d'agrégation                                       |
| nlogts          | Nombre de logements (stock) à la première année de la période d'étude |
| nbtrans         | Nombre de transactions pendant la période d'étude                     |
| nblogtrans      | Nombre de logements ayant mutés pendant la période d'étude            |
| ratio_activite  | Part des logements vendus pendant la période d'étude                  |
|                 |

## Table `stock_evol_volet_1`

| Nom de variable                     | Description                                                                                                                       |
| ----------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| periode                             | Année du milieu de la période d'étude (2011 = 2010 - 2012)                                                                        |
| code                                | Code géographique ou identifiant de l'unité d'agrégation                                                                          |
| nom                                 | Libellé de l'unité d'agrégation                                                                                                   |
| nb_maisons                          | Nombre de maisons                                                                                                                 |
| nb_appts                            | Nombre d'appartements                                                                                                             |
| nb_logts_av45                       | Nombre de logements construits avant 1945                                                                                         |
| nb_logts_45_59                      | Nombre de logements construits entre 1945 et 1959                                                                                 |
| nb_logts_60_74                      | Nombre de logements construits entre 1960 et 1974                                                                                 |
| nb_logts_75_97                      | Nombre de logements construits entre 1975 et 1997                                                                                 |
| nb_logts_98_12                      | Nombre de logements construits entre 1998 et 2012                                                                                 |
| nb_logts_ap13                       | Nombre de logements construits après 2013                                                                                         |
| nb_logts_petits                     | Nombre de logements de petite taille                                                                                              |
| nb_logts_moyens                     | Nombre de logements de taille moyenne                                                                                             |
| nb_logts_grands                     | Nombre de logements de grande taille                                                                                              |
| nb_logts_rppo                       | Nombre de résidences principales occupées par leur propriétaire                                                                   |
| nb_logts_rppb                       | Nombre de résidences principales en location privée                                                                               |
| nb_logts_rs                         | Nombre de résidences secondaires                                                                                                  |
| nb_logts_autre                      | Nombre de logements qui ne sont ni vacants ni dans les deux situations précédentes (inclut les logements sociaux)                 |
| nb_logts_vac2a                      | Nombre de logements vacants depuis au moins 2 ans                                                                                 |
| nb_bureaux                          | Nombre de bureaux                                                                                                                 |
| nb_commerces                        | Nombre de commerces                                                                                                               |
| nb_campings                         | Nombre de campings                                                                                                                |
| nb_hotels                           | Nombre d'hôtels                                                                                                                   |
| nb_act_autres                       | Nombre de locaux d'activité non compris dans les cas précédents                                                                   |
| stot_act_tertiaire                  | Surface de locaux d'activité tertiaire (m²)                                                                                       |
| surfaces_urba                       | Surfaces urbanisées (ha)                                                                                                          |
| surfaces_naf                        | Surfaces NAF (ha)                                                                                                                 |
| surface_zae_ha                      | Surface de zones d'activités économiques (ha)                                                                                     |
| nb_tup                              | Nombre de TUP dans le périmètre d'étude                                                                                           |
| nb_tup_multiple_in_perimetre        | nombre de TUP dans le périmètre d'étude dont le ou un des propriétaires possède également une autre TUP dans le périmètre d'étude |
| surface_multiple_in_perimetre       | Somme des surfaces des TUP dont le ou un des propriétaires possède également une autre TUP dans le périmètre d'étude (ha)         |
| nb_tup_multiple_any                 | Nombre de TUP dans le périmètre d'étude dont le ou un des propriétaires possède également une autre TUP dans le même département  |
| surface_multiple_in_perimetre       | Somme des surfaces des TUP dont le ou un des propriétaires possède également une autre TUP dans le même département (ha)          |
| revenus_d3                          | Troisième décile de revenus déclarés pour cette unité d'agrégation                                                                |
| revenus_med                         | Médiane des revenus déclarés pour cette unité d'agrégation                                                                        |
| revenus_d7                          | Septième décile de revenus déclarés pour cette unité d'agrégation                                                                 |
| evol_vf_med_maison                  | Évolution du prix médian d'une maison entre la première période et la dernière période d'étude (%)                                |
| evol_vf_med_appt                    | Évolution du prix médian d'un appartement entre la première période et la dernière période d'étude (%)                            |
| evol_pxm2_median_foncier_nu_tab     | Évolution du prix médian au m² d'un foncier nu supposé TAB entre la première période et la dernière période d'étude (%)           |
| evol_pxm2_median_foncier_nu_non_tab | Évolution du prix médian au m² d'un foncier nu supposé non TAB entre la première période et la dernière période d'étude (%)       |
| ecart_activite                      | Différence entre le taux d'activité de la période la plus récente et la première période (points)                                 |

## Tables `top_acheteurs` et `top_vendeurs`

| Nom de variable                | Description                                                                                                              |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------------------ |
| periode                        | Année du milieu de la période d'étude (2011 = 2010 - 2012)                                                               |
| code                           | Code géographique ou identifiant de l'unité d'agrégation                                                                 |
| nom                            | Libellé de l'unité d'agrégation                                                                                          |
| categorie                      | Catégorie de propriétaire                                                                                                |
| occurrences                    | Nombre de mutations où cette catégorie de propriétaire apparaît seule                                                    |
| classement_occurences          | Classement de la catégorie de propriétaire en fonction de nombre d'occurrences                                           |
| sum_vf                         | Somme des montants des ventes pour cette catégorie de propriétaire                                                       |
| classement_sum_vf              | Classement de la catégorie de propriétaire en fonction de la somme des montants des ventes                               |
| occurrences_bati               | Nombre de mutations où cette catégorie de propriétaire apparaît seule pour des mutations bâties                          |
| classement_occurences_bati     | Classement de la catégorie de propriétaire en fonction de nombre d'occurrences pour des mutations bâties                 |
| sum_vf_bati                    | Somme des montants des ventes pour cette catégorie de propriétaire  pour des mutations bâties                            |
| classement_sum_vf_bati         | Classement de la catégorie de propriétaire en fonction de la somme des montants des ventes pour des mutations bâties     |
| occurrences_non_bati           | Nombre de mutations où cette catégorie de propriétaire apparaît seule pour des mutations non bâties                      |
| classement_occurences_non_bati | Classement de la catégorie de propriétaire en fonction de nombre d'occurrences pour des mutations non bâties             |
| sum_vf_non_bati                | Somme des montants des ventes pour cette catégorie de propriétaire  pour des mutations non bâties                        |
| classement_sum_vf_non_bati     | Classement de la catégorie de propriétaire en fonction de la somme des montants des ventes pour des mutations non bâties |
|                                |
