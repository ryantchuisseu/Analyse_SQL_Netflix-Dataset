# Analyse_SQL_Netflix-Dataset
 
Nous voulons travailler avec des données sous forme de DataFrame, mais nous souhaitons également effectuer des opérations SQL sur ces données. Cela nous permet de tirer parti des fonctionnalités de pandas tout en utilisant SQL pour des requêtes complexes.

## Outils utilisés:
pyhon, SQL


## Projet SQL : Analyse du Dataset Netflix Movies and TV Shows



# Description
Ce projet présente une série d'exemples de syntaxe SQL en utilisant le dataset Netflix Movies and TV Shows, composé de 8809 lignes. 
L'objectif est de démontrer l'utilisation de concepts SQL clés, tels que les mots-clés SQL, le filtrage de données, les jointures, les unions, les fonctions d'agrégation, les tables temporaires, et les fonctions de fenêtre.

L'intérêt de ce projet est d'illustrer différentes techniques SQL à travers des requêtes appliquées à un dataset réel, permettant ainsi une compréhension pratique et appliquée de SQL.

# **Documentation des Requêtes SQL sur la Base de Données Netflix**

Ce document fournit une liste de requêtes SQL appliquées sur la base de données _Netflix_, avec les descriptions correspondantes pour chaque requête.

### **Structure des données Netflix**

La base de données _Netflix_ contient les colonnes suivantes :

- **cast** : Liste des acteurs apparaissant dans le contenu.
- **country** : Pays où le contenu a été produit.
- **date_added** : Date d'ajout du contenu sur _Netflix_.
- **description** : Brève description du contenu.
- **director** : Nom du ou des réalisateurs.
- **duration** : Durée du contenu (_en minutes pour les films ou en nombre de saisons pour les séries_).
- **listed_in** : Catégories/Genres auxquels le contenu appartient.
- **release_year** : Année de sortie du contenu.
- **show_id** : Identifiant unique pour chaque contenu.
- **title** : Titre du film ou de la série.
- **type** : Type de contenu (_Movie_ ou _TV Show_).
- **rating** : Classification du contenu (_ex. PG-13, R, etc._).

### **Requêtes et Explications**
1. **Question 1**
   _Afficher les 5 premiers éléments du tableau_
![1ère question](https://github.com/user-attachments/assets/53eba979-17bd-4f0b-b0b9-885c6416903d)
<img src="https://github.com/user-attachments/assets/53eba979-17bd-4f0b-b0b9-885c6416903d" alt="Description de l'image" width="300">

   

1. **Question 2**  
   _Quelles sont les valeurs distinctes de l'identifiant de contenu (`show_id`) dans la base de données Netflix ?_

2. **Question 3**  
   _Quels sont les titres uniques de contenus ajoutés après l'année 2020 sur Netflix ?_

3. **Question 4**  
   _Quel est le titre unique de contenu parmi ceux sortis après 2020 et intitulés "Blood & Water" ou avant 2021 pour "Kota Factory", mais qui n'ont pas été produits en Inde ?_

4. **Question 5**  
   _Quels sont les titres uniques des contenus Netflix, triés par ordre alphabétique ?_

5. **Question 6**  
   _Quels sont les cinq premiers enregistrements dans la base de données Netflix ?_

6. **Question 7**  
   _Quelle est l'année de sortie la plus ancienne et la plus récente des contenus, le nombre d'années de sortie distinctes, et la moyenne des années de sortie de tous les contenus ?_

7. **Question 8**  
   _Quels pays ont un nom qui finit par "ia", commence par "ia", contient "ia" ou commence et se termine par "a" ?_

8. **Question 9**  
   _Quels sont les contenus produits en Inde, aux États-Unis ou en Australie, triés par pays en ordre croissant ?_

9. **Question 10**  
   _Quels contenus sont sortis entre 2020 et 2021 ?_

10. **Question 11**  
    _Quels sont les identifiants (`show_id`) correspondant aux deux tables de contenu avec le type et le titre, si les identifiants (`show_id`) sont partagés dans les deux tables de Netflix ?_

11. **Question 12**  
    _Quels sont les contenus Netflix provenant soit d'Inde, soit des États-Unis ?_

12. **Question 13**  
    _Combien de contenus sont produits en Inde, aux États-Unis et en Afrique du Sud dans la base de données Netflix ?_

13. **Question 14**  
    _Quels sont les titres uniques de contenus dans la table Netflix (en utilisant une sous-requête) ?_

14. **Question 15**  
    _Quelle est la première valeur d'année de sortie non nulle dans la table Netflix, ou 0 si elle n'existe pas ?_

15. **Question 16**  
    _Quelle est la première valeur d'année de sortie convertie en valeur flottante dans la table Netflix ?_

16. **Question 17**  
    _Quels contenus ont des années de sortie consécutives (en "back-to-back") et quels titres sont concernés, triés par ordre croissant des années de sortie ?_

17. **Question 18**  
    _Quels sont les titres, types et réalisateurs de chaque contenu, et quel est leur numéro de rang lorsqu'on trie les titres par ordre croissant ?_

18. **Question 19**  
    _Quel est le premier pays dont le nom finit par "ia", le premier pays dont le nom commence par "a", et le premier pays contenant "a" avec une longueur minimale de 4 caractères ?_

19. **Question 20**  
    _Quel est le pays ayant le plus grand nombre de contenus uniques sur Netflix ?_



# Objectifs et Types de Requêtes
Ce projet explore plusieurs aspects de SQL, avec des exemples de requêtes dans chaque catégorie suivante :

**Mots-clés SQL** :  Utilisation de mots-clés tels que SELECT, WHERE, ORDER BY, et GROUP BY pour manipuler et interroger les données.

**Filtrage de données** : Application de conditions pour filtrer les enregistrements selon des critères spécifiques (par exemple, contenu par pays ou année de sortie).

**Jointures** : Illustrations de jointures entre tables pour relier des données (par exemple, joindre le dataset à d'autres datasets si disponibles).

**Unions** : Exemples d'unions pour combiner plusieurs ensembles de résultats en une seule sortie.

**Fonctions d'agrégation** : Utilisation de fonctions telles que COUNT, SUM, AVG, pour obtenir des insights quantitatifs, comme le nombre de films par année.

**Tables temporaires** : Création et utilisation de tables temporaires pour stocker des résultats intermédiaires et simplifier des requêtes complexes.

**Fonctions de fenêtre** : Utilisation de fonctions de fenêtre (ROW_NUMBER(), LAG, LEAD, etc.) pour effectuer des calculs basés sur des groupes de lignes.


# **Utilisation**

1. **Téléchargez** le dataset ici _Kaggle_.

2. **Utilisez python** pour travailler dans un environnement SQL compatible.

3. **Exécutez** les requêtes SQL fournies dans ce projet pour explorer les différentes fonctionnalités de SQL.

4. **Modifiez** et **expérimentez** les requêtes pour répondre à vos propres questions sur les données.

