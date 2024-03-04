##  Création du projet Spring Initializer

Nous avons créé un nouveau projet Spring en utilisant Spring Initializer du intellij ultimate  et avons ajouté les dépendances suivantes : JPA, H2, Spring Web et Lombok.

![1](https://github.com/osmel1/tpSpring1/assets/110778429/108ff3e6-bf17-44f3-9ebf-4020894f0533)

##  Création de l'entité JPA Patient

Nous avons créé une entité JPA nommée Patient avec les attributs suivants :

id (type Long)
nom (type String)
dateNaissance (type Date)
malade (type boolean)
score (type int)
![patientEntity](https://github.com/osmel1/tpSpring1/assets/110778429/776d24c0-9b2c-4bf5-9c40-40b0fd821c04)

##  Configuration de l'unité de persistance

Nous avons configuré l'unité de persistance dans le fichier application.properties en définissant les paramètres nécessaires pour H2 Database.
![3](https://github.com/osmel1/tpSpring1/assets/110778429/079cbcf3-b926-4d48-b470-896e4a06adf2)
Pour vérifier le bon fonctionnement de notre application, nous pouvons accéder à la console H2 en utilisant l'URL suivante dans un navigateur : `localhost:port-num/h2-console` .
![2](https://github.com/osmel1/tpSpring1/assets/110778429/3f96478d-98bc-485e-8ec7-223956246b4a)
## Création de l'interface JPA Repository

Nous avons créé une interface JPA Repository qui herite de sur Spring Data pour gérer les opérations CRUD sur l'entité Patient.

![patientRepo](https://github.com/osmel1/tpSpring1/assets/110778429/7e3843aa-06f9-4967-b952-0353a1c234ad)

##  Test des opérations de gestion de patients

Nous avons testé les opérations suivantes :
![test2](https://github.com/osmel1/tpSpring1/assets/110778429/f452a9fb-dd42-4fc8-9a94-495a7a8f19a6)
![test1](https://github.com/osmel1/tpSpring1/assets/110778429/59fc3470-1925-4b68-805d-310d82186225)

## Migration de H2 Database vers MySQL

Nous avons migré la base de données H2 vers MySQL en modifiant la configuration de l'unité de persistance dans le fichier application.properties pour utiliser MySQL au lieu de H2. Nous avons également effectué les modifications nécessaires pour que le schéma de la base de données soit compatible avec MySQL.
Enfin, il est nécessaire d'ajouter la dépendance MySQL dans le fichier pom.xml.
![dependencyMysql](https://github.com/osmel1/tpSpring1/assets/110778429/9d5af633-69e6-46a4-b2e4-cecd0b7d3e54)
![maeven](https://github.com/osmel1/tpSpring1/assets/110778429/1aa15007-a0d9-4920-9962-85fa8caa0d09)
![migrateMysql](https://github.com/osmel1/tpSpring1/assets/110778429/355105a6-ec8f-4874-8343-15324ae4fd99)

##  Patient, Médecin, rendez-vous, consultation : 
# les entities : 
![image](https://github.com/osmel1/tpSpring1/assets/110778429/37258a40-ddee-4ed8-a16f-2ac0c70277d9)
![image](https://github.com/osmel1/tpSpring1/assets/110778429/c451e0f6-dd10-4959-afe5-9de602ecb957)
![image](https://github.com/osmel1/tpSpring1/assets/110778429/110e41d9-ab93-4f8b-9c4a-98111ec87701)
![image](https://github.com/osmel1/tpSpring1/assets/110778429/b4bfa123-1d5d-46ec-98a0-d0bbbd2a2216)
# les interfaces repository pour chaque entity  : 
![image](https://github.com/osmel1/tpSpring1/assets/110778429/194f8a0d-e42e-4da9-bc71-2426b04e3c63)
![image](https://github.com/osmel1/tpSpring1/assets/110778429/2e89a858-141f-4f71-8ac3-2a668f4d6487)
![image](https://github.com/osmel1/tpSpring1/assets/110778429/9e2cebf0-4e89-486e-90e8-7a72517cd9d0)
![image](https://github.com/osmel1/tpSpring1/assets/110778429/1c979905-7d7b-4b33-a89a-37a8760635f7)

# la couche metier : 
l'interface métier 
![image](https://github.com/osmel1/tpSpring1/assets/110778429/52b24906-cfbc-4974-9d5c-b6979f2c5063)

une implementation de l'interface :  
![image](https://github.com/osmel1/tpSpring1/assets/110778429/446e249c-f01a-4cd5-beb8-3783600f74f9)
![image](https://github.com/osmel1/tpSpring1/assets/110778429/7de834f4-bad8-44cd-9592-039d19d1c8c3)


