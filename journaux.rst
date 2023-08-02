Journaux des activations et désactivations des PGT
=================================================  
Archivage des données
---------------------
L'application SIRIUS conserve la trace des activations et désactivations des PGT. 
Marc Koenig crée chaque mois un fichier .XLSX pour faire des statistiques sur les activations de PGT.
Depuis janvier 2022, Marc partage ce fichier sur OSMOSE : 

.. _a link:   https://osmose.numerique.gouv.fr/jcms/p_3395684/fr/mte-tunnels-idf-fond-documentaire?documentKinds=&explorerCurrentCategory=p_3586253&mids=&portlet=p_3395683&types=ALL




Exploitation des données
---------------------------
Les champs des fichiers sont les suivants : 

``['ID_ENREG_JNAL_EXPL', 'ID_FONCTION', 'SECTEUR', 'DATEE', 'mois', 'jour',   'HORODATE_ACCES_FONCTION', 'ACTEUR_ENREG_JNAL_EXPL', 'NOM_COMPTE','DESCRIPTION', 'type', 'nom', 'delest']``::
  A quoi correspond le champs 'ID_ENREG_JNAL_EXPL' ? permet-il de faire un lien avec un autre objet de SIRIUS ?

Les champs utiles pour exploiter les données sont les suivants :

* 'SECTEUR' 
* 'HORODATE_ACCES_FONCTION' (date à la seconde)
* 'NOM_COMPTE'
* 'DESCRIPTION'  (Désignation du PGT)


