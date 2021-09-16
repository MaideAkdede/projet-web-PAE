# Projet Web - PAE

> Il s'agit du troisième projet à réaliser pour le cours de projets Web

> "Une application de gestion des PAE. Vous avez vécu la constitution des PAE à la rentrée, vous avez eu en main le formulaire, l’idée est d’en faire une version Web, ce qui permet de l’enrichir de fonctionnalités, et de proposer à monsieur Claisse l’outil de gestion qui va avec pour par exemple, ajouter les cours, les crédits, les ranger dans les blocs, valider les PAE, envoyer des mails de rappel pour les absents, etc. On peut imaginer pas mal de choses en termes de fonctionnalités, et on élaborera le cahier des charges ensemble. Une de vos première tâches est d’y réfléchir déjà."

***


### 1. Fonctionnalités de l’administrateur (Monsieur Claisse) :
-	Avoir la possibilité d’encoder
     - Cours du tronc commun
     - Cours d'une certaine option (2D, 3D, Web)
     - Encoder le nombre de crédit de chaque cours
     - Préciser si le cours est un prérequis ou à un corequis
     - Pouvoir ajouter les heures de chaque cours
     - Ajouter un prof pour chaque cours
-	Accès à la liste des élèves et avoir du contrôle dessus
     - Faire des recherches filtrées dans cette liste d’élève
     - Trier par ordre de PAE
        - Trop peu de crédit
        - Beaucoup trop de crédit
     - Filtrer l’affichage
        - Les élèves qui ont réussis et donc pas besoin de vérifier leur PAE
     - Avoir une pagination
-	Gestion des PAE
     - Avoir la possibilité d’envoyer mail à un élève (bouton)
     - Sélectionner des cours qui nécessitent des prérequis
-	Recevoir des notifications et donc avoir une liste
     - Des élèves demandes à avoir un cours auquel il n’a pas accès (prérequis non validé)
     - Quand le prof du cours concerné accepte qu’un élève puisse avoir un cours même si le prérequis n’est pas validé
- Élèves et Profs
     - peut inscrire des élèves/Profs
     - peut modifier nom/prénom/email en cas d'erreur lors de l'inscription
     - pas besoin de vérification dans ce cas-ci

### 2. Fonctionnalités des profs :
-	Accès à la liste des élèves comme l’admin
-	Reçois les demandes des élèves auxquelles ils aimeraient avoir accès
- Inscription
     - nom prénom et adresse mail
     - confirmer via mail de confirmation (?)

### 3. Fonctionnalités de l’élève :
- Inscription
     - entrer nom prénom et adresse email student
     - vérifier par confirmation email (?)
-	Accès au formulaire pour encoder son nvx PAE
     - Verrouiller le choix de l’encodage
     - Possibilité de cocher `j’ai réussi les 60 crédits du bloc`
     - Lorsqu’on coche une case afficher :  x/60 pour le calcul
     - Automatiser et cocher les cases des cours auxquelles l’étudiant a droit
     - Impossible de cocher des cours avec des prérequis non validés
     - Possibilité d’introduire une demande pour avoir des cours auxquelles il n’aurait pas accès (ce qui enverra une notif a l’admin et un mail au prof concerner)
     - Conserver les données de l’étudiants et l’encodage des PAE précédents tout au long de son parcours scolaire
     - Avant la soumission du formulaire montrer le dernier aperçu afin de donner la possibilité à l’élève de ne pas soumettre son formulaire accidentellement
