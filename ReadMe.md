**TP 1 - Installation d’Ubuntu Server et prise en main du shell**

	L'objectif de cet exercice est de comprendre les fonctions et la manipulation de fichiers.

	* __Exercice 1. Installation du serveur__
	
	L'objectif de cette question est d'écrire un programme déclarant, initialisant et affichant les détails des informations de 5 étudiants, en utilisant seulement des tableaux.
		* Fichiers: etudiant.c
		* Bibliothèques: 
			* stdio.h
			* stdlib.h
		* Reférences:
			* Cours2.pdf
		* Difficulté: 
			* RAS -> Déclaration classique et affichage des tableaux 
		* Commentaires: 
			* /

	* __Exercice 2. Prise en main de l’interpréteur de commandes__
	L'objectif de cette question est d'écrire un programme en utilisant struct capable d'assurer la gestion de données étudiantes.
		* Fichiers: etudiant2.c
		* Bibliothèques: 
			* stdio.h
			* stdlib.h
		* Reférences:
			* Cours2.pdf
		* Difficulté: 
			* Adapter l'ancien code en utilisant la structure
		* Commentaires: 
			* /

	* __Exercice 3. Découverte de l’éditeur de texte nano__
	L'objectif de cette question est d'écrire un programme utilisant struct capable de sortir des couleurs en format RGBA.
		* Fichiers: couleurs.c
		* Bibliothèques: 
			* stdio.h
			* stdlib.h
		* Reférences:
			* Cours2.pdf
		* Difficulté: 
			* / (même méthode que celle effectuée à la question précédente)
		* Commentaires: 
			* On utilise des unsigned char afin d'éviter la sortie de valeurs négatives

	* __Exercice 4. Personnalisation du shell__
	L'objectif de cette question est d'écrire un programme affectant et affichant les valeurs des variables de différents types de base en utilisant leurs adresses.
		* Fichiers: ptrvariables.c
		* Bibliothèques: 
			* stdio.h
			* stdlib.h
		* Reférences:
			* Cours2.pdf
		* Difficulté: 
			* Bien manipuler les pointeurs (adresse, contenu...)
		* Commentaires: 
			* /

	* __Exercice 5. Pour les plus rapides__
	L'objectif de cette question est d'écrire un programme manipulant deux tableaux (int et float) et réalisant des opérations logiques en fonction du nombre rencontré (si l'indice est divisé par 2, la valeur à cette position sera multipliée par 3).
		* Fichiers: tableauptr.c
		* Bibliothèques: 
			* stdio.h
			* stdlib.h
		* Reférences:
			* Cours2.pdf
		* Difficulté: 
			* Bien manipuler les pointeurs
		* Commentaires:
			* Ne pas oublier le sizeof(int) et le sizeof(float)
