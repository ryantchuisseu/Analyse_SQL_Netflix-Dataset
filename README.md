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



2. **Question 2**  
   _Quelles sont les valeurs distinctes de l'identifiant de contenu (`show_id`) dans la base de données Netflix ?_
   
![2ème question](https://github.com/user-attachments/assets/1fce5968-97ce-4357-b76c-797a939a69d7)


4. **Question 3**  
   _Quels sont les titres uniques de contenus ajoutés après l'année 2020 sur Netflix ?_
   
![3ème question](https://github.com/user-attachments/assets/a53fc61a-45f9-4b23-98b7-d8ffed14df2f)


6. **Question 4**  
   _Quel est le titre unique de contenu parmi ceux sortis après 2020 et intitulés "Blood & Water" ou avant 2021 pour "Kota Factory", mais qui n'ont pas été produits en Inde ?_
   
![4ème question](https://github.com/user-attachments/assets/e57d921d-97a4-4fc0-8339-a93655f6fc50)


8. **Question 5**  
   _Quels sont les titres uniques des contenus Netflix, triés par ordre alphabétique ?_
   
![5ème question](https://github.com/user-attachments/assets/1aaab035-0c14-40eb-b5fb-988851f866b4)

 

10. **Question 6**  
   _Quels sont les cinq premiers enregistrements dans la base de données Netflix ?_

![6eme question](https://github.com/user-attachments/assets/1b2d41f2-9b6a-47a3-a6c3-05213d4b3087)



12. **Question 7**  
   _Quelle est l'année de sortie la plus ancienne et la plus récente des contenus, le nombre d'années de sortie distinctes, et la moyenne des années de sortie de tous les contenus ?_

![7eme question](https://github.com/user-attachments/assets/e48d8419-4e7a-4b0a-8e6f-1c2c651cba8c)

   

14. **Question 8**  
   _Quels pays ont un nom qui finit par "ia", commence par "ia", contient "ia" ou commence et se termine par "a" ?_

![8ème question](https://github.com/user-attachments/assets/4a77ca9f-d254-4c85-be1e-027ac1a0ffde)


16. **Question 9**  
   _Quels sont les contenus produits en Inde, aux États-Unis ou en Australie, triés par pays en ordre croissant ?_

![9ème question](https://github.com/user-attachments/assets/36d94ae3-6492-4f45-b524-544b33527f01)



18. **Question 10**  
   _Quels contenus sont sortis entre 2020 et 2021 ?_

![10ème question](https://github.com/user-attachments/assets/c9b9953f-f1f9-4965-8b47-a731c6aa945a)



20. **Question 11**  
    _Quels sont les identifiants (`show_id`) correspondant aux deux tables de contenu avec le type et le titre, si les identifiants (`show_id`) sont partagés dans les deux tables de Netflix ?_
    
![11ème question](https://github.com/user-attachments/assets/66b36ba4-3887-4ffe-8c0b-572c1c5ad7ab)



22. **Question 12**  
    _Quels sont les contenus Netflix provenant soit d'Inde, soit des États-Unis ?_
    
![12ème question](https://github.com/user-attachments/assets/b878f9dd-4e9c-467d-b59b-da8456c8295e)



24. **Question 13**  
    _Combien de contenus sont produits en Inde, aux États-Unis et en Afrique du Sud dans la base de données Netflix ?_
    
![13ème question](https://github.com/user-attachments/assets/f0f7157c-9d4c-4b9c-931f-feb4a5213ef9)



26. **Question 14**  
    _Quels sont les titres uniques de contenus dans la table Netflix (en utilisant une sous-requête) ?_
    
![14 ème question](https://github.com/user-attachments/assets/ad4178aa-1766-4095-b4cb-14eb865b2ed1)



28. **Question 15**  
    _Quelle est la première valeur d'année de sortie non nulle dans la table Netflix, ou 0 si elle n'existe pas ?_
    
![15ème question](https://github.com/user-attachments/assets/a0b85877-c0ae-42c5-ac1e-5689c18d8a32)



30. **Question 16**  
    _Quelle est la première valeur d'année de sortie convertie en valeur flottante dans la table Netflix ?_
    
![16 ème question](https://github.com/user-attachments/assets/594ade8f-5bd0-41a4-a076-1f3715a0eead)



32. **Question 17**  
    _Quels contenus ont des années de sortie consécutives (en "back-to-back") et quels titres sont concernés, triés par ordre croissant des années de sortie ?_
    
![17ème question](https://github.com/user-attachments/assets/61a5f89d-4d78-46a1-a635-7ed7bf261807)



34. **Question 18**  
    _Quels sont les titres, types et réalisateurs de chaque contenu, et quel est leur numéro de rang lorsqu'on trie les titres par ordre croissant ?_
    
![18ème question](https://github.com/user-attachments/assets/a709b53a-502c-404a-b353-bf75a58a3c1f)



19 **Question 19**  
    _Quel est le premier pays dont le nom finit par "ia", le premier pays dont le nom commence par "a", et le premier pays contenant "a" avec une longueur minimale de 4 caractères ?_
    
![19ème question](https://github.com/user-attachments/assets/a147f0ad-f65c-4d7b-9f4c-ab7a81559d6b)



20. **Question 20**  
    _Quel est le pays ayant le plus grand nombre de contenus uniques sur Netflix ?_
    
![20ème question](https://github.com/user-attachments/assets/d6f8cb38-8df6-4736-a639-d40deb0c0176)



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

