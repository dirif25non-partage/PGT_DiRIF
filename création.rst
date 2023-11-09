Création de PGT
===============

.. toctree::
   :hidden:

  denomination

Les pratiques varient d'un PCTT à l'autre. On décrira ici ce qui est le plus courant dans la mesure où l'un des objectifs est de guider les acteurs vers une pratique commune homogène.

Qui
------
Les PGT sont principalement créés dans les PCTT par les adjoints d'exploitation ou sous leur contrôle.  
Les traficiens du CCT créent aussi des PGT pour mettre en place des actions transversales ou de dimension régionale.

Comment
---------
Le poste opérateur SIRIUS permet de créer, de paramétrer ou de modifier un PGT, c'est même le seul moyen disponible.  
Il n'est pas possible d'importer des PGT qui auraient été décrits en dehors de SIRIUS.
Lorsqu'un PGT est activé, il n'est pas possible de modifier les autres niveaux du même sous-ensemble.  

Dénomination des PGT
---------------------
Les PGT sont organisés en arborescence à 3 étages : **Nom, Sous-ensemble & Niveau**.  

Il n'y a pas de règle sur la manière dont l'arborescence doit être conçue et les pratiques des PCTT diffèrent.

Le premier étage, **Nom**, désigne un ensemble de PGT d'un même secteur, par exemple : 

* 00S_FERMURG_Présignal
* 02E_FERM
* 02O_FERMPROG, 
* 03E_TRAV_Fermeture, 
* 05_DELEST_SN, ,
* 07S_PPA_PNVIF, 
* 10_PPA_ministere    
* 13S_VOIE_DEDIEE,
* 14E_PrésignalisationVitesse.   
Les deux premiers caractères sont en principe utilisés pour désigner le type de PGT, selon les correspondances suivantes :

* Fermeture urgence     00     
* Test équipement de présignalisation     01
* Fermeture programmée     02
* PGT Travaux ou fermeture     03
* Mesure de trafic régionale, délestage     05
* PGT partenaire - Pollution     06
* PNVIF (plan neige et verglas en île-de-france)    07
* Condition Météo Idf     08
* PPA  (plan particulier d'affichage)  10
* PPI   (plan particulier d'intervention)  12 


Le troisième caractère désigne le secteur pour les PGT séctorisés qui sont majoritaires. Pour les PGT non sectorisés, ce caractère est souvent blanc. *Peut-être devrait-on être plus explicite et utiliser 'R' par exemple.*

Le deuxième étage, **Sous-ensemble**, désigne le secteur concerné, par exemple :  

* A14 Y Tunnel La Défense 
* VOIE_BUS_TAXI_A6A
* A86 I Pr75=>80 (La Jonchère => Echangeur A14)      
* 02- A86E_FRESNES                                   
* A86I_A15 > A3                            
* A1Y              

Le troisième étage, **Niveau** désigne un PGT particulier qui peut être une variante ou une composante d'un ensemble d'actions liées entre elles. 
Pour les fermetures programmées, il s'agit souvent des étapes successives de la fermeture effectuée par une équipe d'exploitation.

Dans le journal des PGT les trois étages sont concaténés dans un champ avec un point “.” comme séparateur. Pour faciliter l’exploitation du journal, il faudrait donc éviter d’utiliser le point dans les noms des PGT. Dans l’ensemble cette règle est déjà respectée, mais on a observé par exemple des points pour écrire 02E_FERM.PROG. ou A. PARE …

Créations de PGT en 2023
-------------------------
En 2023, on identifie les nouveaux PGT activés, au sens où ils n'avaient pas été activés en 2022.
Le tableau suivant représente pour le CTT et les 4 PCTT, le nombre de nouveaux PGT par mois.
Les PGT sont attribués à un PCTT en fonction de la 3ème lettre de leur nom (O,E,N,S, C pour le CCT).

+-+---------+---------+---------+---------+---------+-------+
| |     J   |    F    |    M    |    A    |    M    |   J   |      
+-+---------+---------+---------+---------+---------+-------+
|C|     1   |    13   |     5   |     5   |    14   |    10 |  
+-+---------+---------+---------+---------+---------+-------+
|E|     2   |     2   |    15   |     5   |     2   |    24 | 
+-+---------+---------+---------+---------+---------+-------+
|N|     3   |     5   |     6   |    14   |    15   |    16 |
+-+---------+---------+---------+---------+---------+-------+
|O|     6   |     2   |     5   |     7   |    10   |     9 |
+-+---------+---------+---------+---------+---------+-------+
|S|     3   |     0   |     7   |     2   |     1   |     0 |
+-+---------+---------+---------+---------+---------+-------+

