Création de PGT
===============
Les pratiques varient d'un PCTT à l'autre. On décrira ici ce qui est le plus courant dans la mesure où l'un des objectifs est de guider les acteurs vers une pratique commune homogène.

Qui
------
Les PGT sont principalement créés dans les PCTT par les adjoints d'exploitation ou sous leur contrôle.  
Les traficiens du CCT créent aussi des PGT pour mettre en place des actions transversales ou de dimension régionale.

Comment
---------
Le poste opérateur SIRIUS permet de créer et de paramétrer un PGT, c'est le moyen utilisé par les PCTT.

Le CCT possède un outil pour créer des PGT en dehors de SIRIUS et de les importer par la suite. Cet outil est utile pour les actions qui consistent à créer systématiquement  des PGT pour un ensemble de sites. On l'utilise par exemple pour créer les PGT de présignalisation de vitesse pour les incidents en tunnel ou pour la mise en place des fermetures d'urgence progressives, en car de panne technique constituant un danger imminent.

Dénomination des PGT
---------------------
Les PGT sont organisés en arborescence à 3 étages : **Nom, Sous-ensemble & Niveau**.  

Le premier étage, **Nom**, désigne une catégorie de PGT, par exemple : 

* 00S_FERMURG_Présignal
* 02E_FERM
* 02O_FERMPROG, 
* 03E_TRAV_Fermeture, 
* 05_DELEST_SN, ,
* 07S_PPA_PNVIF, 
* 10_PPA_ministere    
* 13S_VOIE_DEDIEE,
* 14E_PrésignalisationVitesse.   
Les deux premiers caractères sont en principe utilisés pour désigner la catégorie de PGT.  '00' pour les fermeture d'urgence de tunnels,
'02' pour les fermetures programmées pour travaux ...

Le troisième caractère désigne le secteur pour les PGT séctorisés qui sont majoritaires. Pour les PGT non sectorisés, ce caractère est souvent blanc. Peut-être devrait on être plus explicite et utiliser 'R' par exemple.

Le deuxième étage, **Sous-ensemble**, désigne le secteur concerné, par exemple :  

* A14 Y Tunnel La Défense 
* VOIE_BUS_TAXI_A6A
* A86 I Pr75=>80 (La Jonchère => Echangeur A14)      
* 02- A86E_FRESNES                                   
* A86I_A15 > A3                            
* A1Y              

Le troisième étage, **Niveau** désigne un PGT particulier qui peut être une variante ou une composante d'un ensemble d'actions liées entre elles.

Dans le journal des PGT les trois étages sont concaténés dans un champ avec un point “.” comme séparateur. Pour faciliter l’exploitation du journal, ill faudrait donc éviter d’utiliser le point dans les noms des PGT. Dans l’ensemble cette règle est déjà bien respectée, mais on a observé par exemple des points pour écrire 02E_FERM.PROG. ou A. PARE …

+------------------------+------------+----------+----------+
| Header row, column 1   | Header 2   | Header 3   | Header 4  |
| (header rows optional) |            |          |          |
+========================+============+==========+==========+
| body row 1, column 1   | column 2   | column 3 | column 4|
+------------------------+------------+----------+----------+
| body row 2             | Cells may span columns.          |
+------------------------+------------+---------------------+
| body row 3             | Cells may  | - Table cells       |
+------------------------+ span rows. | - contain           |
| body row 4             |            | - body elements.    |
+------------------------+------------+---------------------+
S
