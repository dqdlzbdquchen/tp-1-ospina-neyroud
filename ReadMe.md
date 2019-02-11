**TP 1 - Installation d’Ubuntu Server et prise en main du shell**

	Ce premier TP a pour but de créer et configurer à l’aide de VirtualBox les machines virtuelles qui nous serviront durant tout le module, d’installer de zéro un système Ubuntu Server et de prendre en main les commandes de base de l’interpréteur de commande (shell).

	* __Exercice 1. Installation du serveur__
	
	Création de la VM serveur en suivant les instructions puis clonage de cette VM en client.


	* __Exercice 2. Prise en main de l’interpréteur de commandes__
	
	** Manuel **
	
	Question 1 : A l’aide du manuel, identifiez le rôle de la commande which
		* La commande which renvoie le chemin des fichiers (ou liens) qui seraient éxécutés dans l'environnement courant si ddes arguments avaient été données comme commandes dans un interpréteur de commandes strictement conforme à POSIX. pour ce faire, which cherche dans la variable PATH les fichiers éxécutables correspondant aux noms des arguments. which ne normalise pas les chemins.
		
	Question 2 : Quelle commande permet de rechercher le mot option dans cette page ?
		* Lorsque l'on a tapé "man which" on tape ensuite "/options".
		
	Question 3 : Comment quitte-t-on le manuel ?
		* On quitte le manuel en pressant la touche "q".
	
	Question 4 : Afficher la première page de la section 6 ; de quoi parle cette section ?
		* On tape la commande "man 6 intro".
			
	** Navigation dans l’arborescence des fichiers **
	
	Question 1 : allez dans le dossier /var/log
		* On tape la commande "cd /var/log".
		
	Question 2 : remontez dans le dossier parent (/var) en utilisant un chemin relatif
		* On éxécute la commande "cd ..".
		
	Question 3 : retournez dans le dossier personnel
		* On éxécute la commande "cd ~".
		
	Question 4 : revenez au dossier précédent (/var)
		* On éxécute la commande "cd /var".
		
	Question 5 : essayez d’accéder au dossier /root ; que se passe-t-il ?
		* On obtient une erreur système : "permission denied".

	Question 6 : essayez la commande sudo cd /root ; que se passe-t-il ? Expliquez
		* On nous demande de saisir le mdp admin mais au final on obtient un "command not found". La commande "sudo" n'est disponible qu'en bash.
		
	Question 7 : à partir de votre dossier personnel, créez l’arborescence suivante :
		* mkdir Dossier1 Dossier2 Dossier2/Dossier2.1 Dossier2/Dossier2.2
		* touch Dossier1/Fichier1 Dossier2/Dossier2.2/Fichier2 Dossier2/Dossier2.2/Fichier3 
		
	Question 8 : revenez dans votre dossier personnel ; à l’aide de la commande rm, essayez de supprimer Fichier1, puis Dossier1 ; que se passe-t-il ?
		*
	
	Question 9 : quelle commande permet de supprimer un dossier ?
		*

	Question 10 : que se passe-t-il quand on applique cette commande à Dossier2 ?
		*

	Question 11 : comment supprimer en une seule commande Dossier2 et son contenu ?
		*



	* __Exercice 3. Découverte de l’éditeur de texte nano__
	
	Question 1 : 
		* 

	* __Exercice 4. Personnalisation du shell__
	
	Question 1 : 
		* 

	* __Exercice 5. Pour les plus rapides__
	
	Question 1 : 
		* 

