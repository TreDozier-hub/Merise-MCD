## Quiz guidé : Modélisation des données et MERISE

### 1. Quand on parle de données dans le développement, pourquoi faut-il modéliser ?
```
   -La modélisation des données consiste à représenter de manière structurée et abstraite les informations d'un système pour faciliter leur gestion, leur compréhension et leur manipulation. La méthode MERISE est une approche d'analyse et de conception qui utilise des modèles, comme le modèle conceptuel de données (MCD), pour structurer les données et les processus d'un système d'information de manière claire et cohérente.
   ```

### 2. Qu'est-ce qu'une base de données ?
```
   - Une base de données, c'est comme un endroit où on range des informations pour les retrouver
   facilement plus tard. Par exemple, si tu as un cahier où tu écris les noms de tes amis et leurs 
   numéros de téléphone, c'est une petite base de données. C'est juste un moyen organisé pour garder 
   des choses importantes bien rangées et pouvoir les utiliser quand on en a besoin ! 
```
### 3. Que veut dire MERISE ?
```
   --> est une méthode d'analyse, de conception et de gestion de projet informatique.

   --> Cette méthode a eu comme objectif premier de jeter un pont entre les besoins des utilisateurs et les solutions des informaticiens.

   - Le mot MERISE ne correspond pas directement à un acronyme, mais il est souvent interprété comme une contraction de "Méthode d'Étude et de Réalisation Informatique pour les Systèmes d'Entreprise".
   - Cette interprétation reflète bien son objectif : analyser, concevoir et structurer les systèmes d'information dans les entreprises.
```
#### Les 4 niveaux de MERISE :

1. **Le niveau conceptuel** : Que définit le niveau conceptuel dans la méthode MERISE ?
2. **Le niveau organisationnel** : Que définit le niveau organisationnel dans MERISE ?
3. **Le niveau logique** : Que définit le niveau logique dans MERISE ?
4. **Le niveau physique** : Que définit le niveau physique dans MERISE ?
```
1. **Le niveau conceptuel** : Dans la méthode MERISE, le niveau conceptuel définit les données et traitements du système de manière abstraite, sans prendre en compte les contraintes techniques. 

--> Le Modèle Conceptuel de Données (MCD) : Il décrit les données essentielles du système, leurs relations, et les règles de gestion associées, en se basant sur des entités, des associations et des cardinalités.

-->Le Modèle Conceptuel de Traitements (MCT) : Il représente les processus, les flux d'informations et les interactions entre les différents éléments du système.

2. **Le niveau organisationnel** : Le niveau organisationnel dans MERISE décrit les processus et les flux d'informations tels qu'ils se déroulent dans l'organisation, en tenant compte des acteurs et des règles de gestion.  

3. **Le niveau logique** : Le niveau logique dans MERISE détaille la structure et l'organisation des données et traitements en fonction des contraintes du logiciel ou de la technologie choisie.  

4. **Le niveau physique** : Le niveau physique dans MERISE spécifie la mise en œuvre concrète des données et des traitements sur le matériel et les systèmes techniques utilisés.

### 4. MERISE : Modèle Conceptuel des Données

1. Quelles sont les trois notions de base introduites dans le modèle conceptuel des données MERISE ?
   - **Entité** : Qu'est-ce qu'une entité dans le contexte de MERISE ?
   - **Propriété** : Qu'est-ce qu'une propriété dans MERISE ?
   - **Relation** : Qu'est-ce qu'une relation dans MERISE ?

   1. **Entité** : Une entité dans MERISE représente un objet ou une notion identifiable du système (comme un client, un produit, ou une commande) qui possède des caractéristiques à modéliser.  

   2. **Propriété** : Une propriété dans MERISE est une caractéristique ou un attribut qui décrit une entité ou une relation, comme le nom d’un client ou le prix d’un produit.  

   3. **Relation** : Une relation dans MERISE est un lien qui établit une association logique entre deux ou plusieurs entités, comme le lien entre un client et les commandes qu’il passe.
```
#### Les cardinalités

2. Que définissent les cardinalités dans un modèle conceptuel des données ?
```
--> Les cardinalités dans un modèle conceptuel de données définissent combien d'éléments d'une entité peuvent être associés à combien d'éléments d'une autre entité. Par exemple, elles indiquent si un client peut passer une ou plusieurs commandes (1,N) ou si une commande appartient à un seul client (1,1).

Exemple :
IBien sûr ! La notion de cardinalité en SQL est comme une règle pour expliquer combien de fois une chose peut être liée à une autre dans une relation.

Imagine que tu as deux boîtes :

    Une boîte "Personnes".
    Une boîte "Voitures".

La cardinalité te dit combien de voitures une personne peut avoir, et combien de personnes peuvent partager une voiture.
Les types de cardinalité :

    (1,1) :
        Chaque personne a exactement une voiture.
        Exemple : "Chacun a une voiture attribuée."

    (0,1) :
        Une personne peut avoir 0 ou 1 voiture.
        Exemple : "Pas tout le monde a une voiture."

    (0,n) :
        Une personne peut avoir 0, 1 ou plusieurs voitures.
        Exemple : "Certaines personnes adorent collectionner les voitures !"

    (1,n) :
        Chaque personne a au moins 1 voiture, mais peut en avoir beaucoup.
        Exemple : "Les membres d’un club de voitures anciennes, par exemple."

    (n,m) :
        Plusieurs personnes peuvent partager plusieurs voitures.
        Exemple : "Un service de covoiturage où les voitures sont partagées par tout le monde."

Tu peux voir cela comme une étiquette qui décrit combien de connexions peuvent exister entre deux boîtes. 
```
#### Quelles sont les limites de la méthode MERISE ?
```
   -->  Elle est moins adaptée aux projets transverses aux organisations, qui gèrent le plus souvent des informations à caractère sociétal (environnemental et social) avec des parties prenantes.
```
### 5. Propriété des Associations / Relation Réflexive

1. Qu'est-ce qu'une relation réflexive dans un modèle conceptuel des données ?
```
   -->Une relation réflexive dans un modèle conceptuel de données est une relation où une entité est liée à elle-même. Cela représente une situation où les instances d'une même entité interagissent entre elles.
```
### 6. Notion : Entité Forte / Entité Faible

1. Qu'est-ce qu'une entité forte ?
2. Qu'est-ce qu'une entité faible ?
```
Entité forte : Une entité forte est une entité qui existe indépendamment et possède une clé primaire propre, c'est-à-dire un identifiant unique qui la distingue de toutes les autres entités. Par exemple, un Client est une entité forte, car chaque client peut être identifié de manière unique par son numéro de client.

Entité faible : Une entité faible dépend d'une autre entité (généralement une entité forte) pour exister et n'a pas de clé primaire propre. Elle est identifiée grâce à la clé primaire de l'entité forte à laquelle elle est liée. Par exemple, une Commande est une entité faible car elle dépend du client qui a passé la commande pour être identifiée (par exemple, numéro de commande + numéro de client).
```
### 7. MLD : Modèle Logique des Données

1. Quel est le rôle du **Modèle Logique des Données (MLD)** dans la transition entre le modèle conceptuel et la mise en œuvre réelle d'une base de données ?
2. Dans le MLD, comment une entité, un identifiant et une propriété sont-ils représentés ?
```
--> En partant d'un MCD, un MLD introduit les éléments, les relations et les détails contextuels nécessaires à la structure des données afin de se rapprocher de la mise en œuvre.

--> Dans le Modèle Logique de Données (MLD), les éléments sont représentés de manière plus structurée et proche de la base de données réelle. Voici comment chaque élément est représenté :

    Entité : L'entité est représentée par une table dans le MLD. Par exemple, une entité "Client" devient une table nommée Client.

    Identifiant : L'identifiant, ou clé primaire, est représenté par une colonne spécifique dans la table, qui permet d'identifier de manière unique chaque ligne de la table. Par exemple, dans la table Client, la clé primaire pourrait être le NuméroClient.

    Propriété : Les propriétés sont représentées par des colonnes dans la table. Elles correspondent aux attributs de l'entité, comme Nom, Adresse ou Email dans la table Client.

Ainsi, dans le MLD, une entité devient une table, son identifiant devient une colonne clé primaire, et ses propriétés deviennent des colonnes normales.

#### UML : Unified Modeling Language

1. Qu'est-ce que **UML** (Unified Modeling Language) et quel est son rôle dans la modélisation des systèmes logiciels ?
```
--> **UML** (Unified Modeling Language) est un langage de modélisation graphique utilisé pour représenter et concevoir des systèmes logiciels. Il permet de décrire visuellement les différentes parties d'un système, comme les données, les comportements et les interactions, à l'aide de diagrammes standardisés.

Le rôle de **UML** dans la modélisation des systèmes logiciels est de fournir une méthode claire et uniforme pour **comprendre**, **documenter** et **communiquer** les structures et le fonctionnement d'un logiciel. Il permet aux développeurs, analystes et autres parties prenantes de mieux comprendre le système, d'éviter les erreurs de conception, et de faciliter la communication tout au long du développement.

![alt text](image-2.png)
![alt text](image-1.png)


-->Classe : définition structurelle et comportementale d’un ensemble d’objets ayant les mêmes
propriétés.
```
#### Notes :

```
Mise en oeuvre de la méthode Merise

    Le Cahier Des Charges (CDC)

    Le Modèle Conceptuel de Communication (MCC)

![alt text](image.png)
```
```
    Le Dictionnaire des Données (DD)
    -->Le dictionnaire des données est un document qui regroupe toutes les données que vous aurez à conserver dans votre base (et qui figureront donc dans le MCD).
    
  ![alt text](image-4.png)


       Le code mnémonique : il s'agit d'un libellé désignant une donnée (par exemple «titre_l» pour le titre d'un livre)

    La désignation : il s'agit d'une mention décrivant ce à quoi la donnée correspond (par exemple «titre du livre»)

    Le type de donnée :

        A ou Alphabétique : lorsque la donnée est uniquement composée de caractères alphabétiques (de 'A' à 'Z' et de 'a' à 'z')

        N ou Numérique : lorsque la donnée est composée uniquement de nombres (entiers ou réels)

        AN ou Alphanumérique : lorsque la donnée peut être composée à la fois de caractères alphabétiques et numériques

        Date : lorsque la donnée est une date (au format AAAA-MM-JJ)

        Booléen : Vrai ou Faux

    La taille : elle s'exprime en nombre de caractères ou de chiffres. Dans le cas d'une date au format AAAA-JJ-MM, on compte également le nombre de caractères, soit 10 caractères. Pour ce qui est du type booléen, nul besoin de préciser la taille (ceci dépend de l'implémentation du SGBDR).

    Et parfois des remarques ou observations complémentaires (par exemple si une donnée est strictement supérieure à 0, etc).
```
    Le Graphe des Dépendances Fonctionnelles (GDF)
    Le Modèle Conceptuel des Données (MCD)
    Le Modèle Organisationnel des Données (MOD)
    Le Modèle Logique des Données (MLD)


<merise>
<cdc><objectifs>Gérer la consommation
</objectifs>
<enjeux>historiser toutes les transactions d’un café pour identifier les atouts et faiblesses commerciales (serveur le plus performant, boissons non vendues…)
</enjeux>
<strategies>construire un outil de saisie pour les serveurs générant des informations pour le patron – l’application devra recenser les serveurs, les commandes et les boissons.
</strategies>
<domaine>on se limite aux ventes de l'établissement (éventuellement étendre aux fournisseurs plus tard)
</domaine>
<contraintes>Contrainte de délais : date de livraison du produit et les éventuelles échéances intermédiaires

Autres contraintes : normes techniques (W3C), clauses juridiques (CNIL dès qu’il s’agit d’informations nominative)…

Critère d’acceptabilité : prévoir le stockage de plus de 10 000 transactions, la montée en charge sur certains horaires…
</contraintes>
</cdc>
<mcc><domaines>rappel des objectifs</domaines>
<acteurs>
<acteur id="Client">
<sortant><libelle>Livraison</libelle><annotations>date et heure
montant par produit</annotations></sortant>
<entrant><libelle>Commande</libelle><annotations>nom du produit
quantité commandée
prix unitaire</annotations></entrant>
</acteur>
</acteurs>
</mcc>
<dd>
<champ><nom>Q1</nom><libelle>Consommation</libelle><type>T</type><obtenu>S</obtenu><exemple>(commande)</exemple></champ>
</dd>
<gdf></gdf>
</merise>
