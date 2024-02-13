Journaux des activations et désactivations des PGT
=================================================  
Archivage des données
---------------------
L'application SIRIUS conserve la trace des activations et des désactivations des PGT. 
Marc Koenig (UCTIR) crée chaque mois un fichier .XLSX pour faire des statistiques sur les activations de PGT.
Depuis janvier 2022, Marc partage ces fichiers sur OSMOSE. 

`Lien OSMOSE`_
    
.. _Lien OSMOSE: https://osmose.numerique.gouv.fr/jcms/p_3395684/fr/mte-tunnels-idf-fond-documentaire?documentKinds=&explorerCurrentCategory=p_3588697&mids=&portlet=p_3395683&types=ALL

`Lien OSMOSE2<https://osmose.numerique.gouv.fr/jcms/p_3395684/fr/mte-tunnels-idf-fond-documentaire?documentKinds=&explorerCurrentCategory=p_3586253&mids=&portlet=p_3395683&types=ALL>`_



Les fichiers, jusqu'en avril 2023, ne contiennent que les activations de PGT. Depuis le mois de mai, figurent aussi les désactivations. 
Le champ DESCRIPTION commence systématiquement par l'un des mots : **Activation** ou **Désactivation**.

On ne trouve pas toujours la désactivation après une activation ce qui appelle une explication, on y reviendra ci-dessous.

Exploitation des données
---------------------------
Les champs des fichiers sont les suivants : 

``['ID_ENREG_JNAL_EXPL', 'ID_FONCTION', 'SECTEUR', 'DATEE', 'mois', 'jour',   'HORODATE_ACCES_FONCTION', 'ACTEUR_ENREG_JNAL_EXPL', 'NOM_COMPTE','DESCRIPTION', 'type', 'nom', 'delest']``  

         ``A quoi correspond le champs 'ID_ENREG_JNAL_EXPL' ? permet-il de faire un lien avec un autre objet de SIRIUS ?``

Les champs utiles pour exploiter les données sont les suivants :

* 'SECTEUR' 
* 'HORODATE_ACCES_FONCTION' (date à la seconde)
* 'NOM_COMPTE' (Nom de l'OST connecté à SIRIUS ou PASSERELLE SAGTU, il faut savoir que les OST ne se déconnectent pas systématiquement et qu'un même compte reste parfois ouvert perdant plusieurs vacations.)
* 'DESCRIPTION'  (Désignation du PGT, les 3 étages séparés par des points ".".)

Interprétation des données 
--------------------------
Pour interpréter les journaux des PGT, il faut bien comprendre ce qui s'y trouve enregistré.

On identifie ci dessous quelques curiosités qui appellent des explications.

Sequence d'activation et désactivation
.........................................
Sur les mois de mai et juin 2023, on observe 1381 désactivations et 1139 activations. Soit 20 % de plus de désactivations.

L'importance du désequilibre entre les activations et les désactivations est variable selon le type de PGT.

Si l'on examine les suites d'enregistrements d'un même PGT, on trouve très fréquement plusieurs activations ou plusieurs désactivations successives, à quelques secondes ou minutes d'intervale.

Il semble que l'OST peut lancer plusieurs fois de suite la commande d'activation ou de désactivation. En particulier, les OST activent certains PGT par groupes. Certains PGT peuvent être dans plusieurs groupes différents qui sont activés successivement.





