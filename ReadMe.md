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
		* Ca ne le supprime pas car le dossier n'est pas vide.
	
	Question 9 : quelle commande permet de supprimer un dossier ?
		* Il suffit de saisir "rmdir" pour supprimer le dossier vide.

	Question 10 : que se passe-t-il quand on applique cette commande à Dossier2 ?
		* Le dossier n'est pas supprimé car il n'est pas vide.

	Question 11 : comment supprimer en une seule commande Dossier2 et son contenu ?
		* Il suffit de saisir "rm -rf" pour supprimer le dossier (et son contenu).


	* __Exercice 3. Découverte de l’éditeur de texte nano__
	
	Question1 : Quelle commande permet d’afficher l’heure ? A quoi sert la commande time ?
		* Il suffit de saisir "date +%T". time renvoie l'heure actuelle sous forme du nombre de secondes écoulées depuis le 1er janvier 1970 à 00h 00m 00s GMT, le début de l'Ère Unix.
		
	Question2 : Dans votre dossier personnel, tapez successivement les commandes ls puis la ; que peut-on en déduire
	sur les fichiers commençant par un point ?
		* Les fichiers commençant par un point sont des fichiers cachés.
		
	Question3 : Où se situe le programme ls ?
		* Grace à la commande "whereis ls" on voit qu'il est situé dans le dossier /bin/ls /usr/share/man/man1/ls.1.gz
		
	Question 4 : Que fait la commande ll ? (indice : la commande alias peut vous aider)
		* Elle permet de lister tout le contenu présent dans le répertoire actuel (avec des données supplémentaires tel que les droits).
		
	Question 5 : Quelle commande permet d’afficher les fichiers contenus dans le dossier /bin ?
		* Grace à la commande "ls /bin".
		
	Question 6 : Que fait la commande ls .. ?
		* Elle affiche le contenu du dossier parent.
		
	Question 7 : Quelle commande donne le chemin complet du dossier courant ?
		* Grace à la commande "pwd".
		
	Question 8 : Que fait la commande echo 'yo' > plop exécutée 2 fois ?
		* La première éxécution de commande permet d'écrire "yo" dans le fichier plop (il est créé s'il n'existe pas) et la seconde commande va écraser le contenu du fichier.
		
	Question 9 : Que fait la commande echo 'yo' >> plop exécutée 2 fois ?
		* La première éxécution de commande permet d'écrire "yo" dans le fichier plop (il est créé s'il n'existe pas) et la seconde commande va rajouter le texte "yo" à la fin du fichier.
		
	Question 10 : A quoi sert la commande file ? Essayez la sur des fichiers de types différents.
		*
		
	Question 11 : Créez un fichier toto qui contient la chaîne Hello Toto ! ; créer ensuite un lien titi vers ce fichier
	avec la commande ln toto titi. Modifiez à présent le contenu de toto et affichez le contenu de titi :
	qu’observe-t-on ? Supprimez le fichier toto ; quelle conséquence cela a-t-il sur titi ?
		*
		
	Question 12 : Créez à présent un lien symbolique tutu sur titi avec la commande ln -s titi tutu. Modifiez le
	contenu de titi ; quelle conséquence pour tutu ? Et inversement ? Supprimez le fichier titi ; quelle
	conséquence cela a-t-il sur tutu ?
		*
		
	Question 13 : Affichez à l’écran le fichier /var/log/syslog. Quels raccourcis clavier permettent d’interrompre et
	reprendre le défilement à l’écran ?
		*
	
	Question 14 : Affichez les 5 premières lignes du fichier /var/log/syslog, puis les 15 dernières, puis seulement les
	lignes 10 à 20.
		*
		
	Question 15 : Que fait la commande dmesg | less ?
		*
		
	Question 16 : Affichez à l’écran le fichier /etc/passwd ; que contient-il ? Quelle commande permet d’afficher la page de manuel de ce fichier ?
		*
		
	Question 17 : Affichez seulement la première colonne triée par ordre alphabétique inverse
		*
		
	Question 18 : Quelle commande nous donne le nombre d’utilisateurs ?
		*
		
	Question 19 : Combien de pages de manuel comportent le mot-clé conversion dans leur description ?
		*
		
	Question 20 : A l’aide de la commande find, recherchez tous les fichiers se nommant passwd présents sur la machine
		*
		
	Question 21 : Modifiez la commande précédente pour que la liste des fichiers trouvés soit enregistrée dans le fichier ~/list_passwd_files.txt et que les erreurs soient redirigées vers le fichier spécial /dev/null
		*
	
	Question 22 : Dans votre dossier personnel, utilisez la commande grep pour chercher où est défini l’alias ll vu
	précédemment
		*
	
	Question 23 : Utilisez la commande locate pour trouver le fichier history.log.
		*
		
	Question 24 : Créer un fichier dans votre dossier personnel puis utilisez locate pour le trouver. Apparaît-il ? Pourquoi ? 
		* 

	* __Exercice 4. Personnalisation du shell__
	
	Question 1 : 
		* 

	* __Exercice 5. Pour les plus rapides__
	
	Question 1 : 
		* 

