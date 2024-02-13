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
