# ISN_TP_GIT_Initiation
TP d'initiation à la pratique de GIT

* Vous vous êtes mis par groupe de deux et vous avez chacun créé un compte sur GitHub (nous désignerons par noordo4xx et noordo4yy vos identifiants respectifs dans ce qui suit).
* Dupliquez (*fork*) le projet ISN_TP_GIT_Initiation dans votre espace public.
* Récupérez sur votre disque dur les sources du projet.

        git clone https://github.com/noordo4xx/ISN_TP_GIT_Initiation.git

* Définissez une étiquette (depot-officiel) pour désigner le dépôt officiel :

        cd ISN_TP_GIT_Initiation
        git remote add depot-officiel https://github.com/noordo/ISN_TP_GIT_Initiation.git

* Vérifiez la liste des dépôts distants référencés :

        git remote -v

* Sur votre disque dur, ajoutez à la fin de ce fichier les initiales et l'identifiant GitHub de **l'un** des 2 membres du groupe (par exemple noordo4xx). La ligne doit commencer par une étoile. Corrigez la liste pour que la dernière ligne se termine par un point et les autres par des virgules.
* Faites une révision (ajout à une nouvelle branche de développement : devNoordo4xx) :

        git checkout -b devNoordo4xx
        git add README.md
        git commit

* Publiez-la dans votre espace public:

        git push origin devNoordo4xx

* Ajoutez les initiales et l'identifiant GitHub du membre du binôme (noordo4yy) selon les mêmes règles que tout à l'heure.
* Faites une révision (ajout à une nouvelle branche de développement : devNoordo4yy) :

        git checkout master
        git checkout -b devNoordo4yy
        git add README.md
        git commit

* Intégrez la première branche à nouvelle branche (devGroupe) d'intégration des développements des 2 membres du groupe.

        git checkout master
        git checkout -b devGroupe
        git merge devNoordo4xx
        
* Essayez d'intégrer la seconde branche à devGroupe :

        git merge devNoordo4yy

* Réglez le conflit. Modifiez la mise en page de la liste pour qu'elle soit correcte. Puis déclarez que le conflit est réglé :

        git add README.md
        git commit

* Une fois que le conflit est réglé par une révision, publiez l'ensemble des révisions dans votre espace public :

        git push origin devGroupe

* Dans GitHub faites une demande d'intégration (*pull request*).

* Supposons maintenant que la maintenance de la branche officielle ne soit plus assurée et que vous décidiez de prendre la relève. Récupérez la dernière version officielle :
 
        git pull depot-officiel master

* Récupérez la demande d'intégration d'un de vos collègues (noordo4zz) :

        git pull https://github.com/noordo4zz/ISN_TP_GIT_Initiation.git nomdesabranche

* Réglez le conflit. Mettez à jour votre branche maître. Publiez.

Liste des élèves de TS ayant réussi ce TP
-----------------------------------------

* GM alias noordo400.
