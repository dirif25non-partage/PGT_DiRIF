Base de données des PGT
==========================
La liste des PGT est consultable sur le poste opérateur SIRIUS qui permet de les activer ou de les désactiver et de les modifier.

UCTIR met chaque mois sur OSMOSE la liste des PGT activés ou désactivés le mois précédent.

UIRC fait également chaque jour une extraction de tables qui contiennent un index des niveau de PGT et le lien entre les niveaux et les équipements qui sont activés.

UCTIR utilise ces tables pour représenter sur une carte avec QGIS les effets produits par les PGT.

L'index des PGT **ID_NIVEAU_PGT** qui est utilisé dans la table n'est pas stable dans le temps. Il ne peut donc pas être utilisé pour suivre l'utilisation d'un PGT dans le temps.

Quand on a besoin d'un identifiant fixe, UCTIR utilise le champ **REF_PGT_PARTENAIRE**. C'est en particulier la manière dont le lien est fait avec le SAGTU. Certains utilisateurs (PCTT Est notent la valeur de ce champ à la fin du champ **LIBELLE_NIVEAU_PGT**). 
