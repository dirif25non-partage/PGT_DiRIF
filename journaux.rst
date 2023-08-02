Journaux des activations et désactivations des PGT
=================================================  
Archivage des données
---------------------
L'application SIRIUS conserve la trace des activations et désactivations des PGT. 
Marc Koenig crée chaque mois un fichier .XLSX pour faire des statistiques sur les activations de PGT.
Depuis janvier 2022, Marc partage ce fichier sur OSMOSE : 

.. _a link:   https://osmose.numerique.gouv.fr/jcms/p_3395684/fr/mte-tunnels-idf-fond-documentaire?documentKinds=&explorerCurrentCategory=p_3586253&mids=&portlet=p_3395683&types=ALL

Les fichiers jusqu'en avril 2023 n'indiquent pas s'il s'agit d'une activation ou d'une désactivation du PGT. Quand un PGT de travaux apparait à 22h, on peut supposer qu'il s'agit d'une activation. Quand il apparait à 4h, c'est probablement une désactivation. 

Mais quand le PGT apparait plusieurs fois à quelques minutes d'interval, il n'est pas possible de savoir dans quels état on est arrivé.

Depuis mai 2023, le champ DESCRIPTION commence systématiquement par l'un des mots : Activation ou Désactivation.
On ne trouve pas toujours la désactivation après une activation ce qui appelle une explication, on y reviendra ci-dessous.

Exploitation des données
---------------------------
Les champs des fichiers sont les suivants : 

``['ID_ENREG_JNAL_EXPL', 'ID_FONCTION', 'SECTEUR', 'DATEE', 'mois', 'jour',   'HORODATE_ACCES_FONCTION', 'ACTEUR_ENREG_JNAL_EXPL', 'NOM_COMPTE','DESCRIPTION', 'type', 'nom', 'delest']``  

         ``A quoi correspond le champs 'ID_ENREG_JNAL_EXPL' ? permet-il de faire un lien avec un autre objet de SIRIUS ?``

Les champs utiles pour exploiter les données sont les suivants :

* 'SECTEUR' 
* 'HORODATE_ACCES_FONCTION' (date à la seconde)
* 'NOM_COMPTE' (Nom de l'OST connecté à SIRIUS ou PASSERELLE SAGTU, il faut savoir que les OST ne s'identifient pas toujours et qu'un même compte reste parfois ouvert perdant plusieurs vacations.)
* 'DESCRIPTION'  (Désignation du PGT)

Interprétation des données 
--------------------------
Pour interpréter les journaux des PGT, il faut bien comprendre ce qui s'y trouve enregistré.

On identifie ci dessous quelques curiosité qui appellent des explications.

Sequence d'activation et désactivation
.........................................
Sur les mois de mai et juin 2023, on observe 1381 désactivations et 1139 activations. Soit 20 % de plus de désactivations.

L'importance du désequilibre entre les activations et les désactivations est variable selon le type de PGT.



Si l'on examine les suites d'enregistrements d'un même PGT, on trouve très fréquement plusieurs activations ou plusieurs désactivations successives, à quelques secondes ou minutes d'intervale.







