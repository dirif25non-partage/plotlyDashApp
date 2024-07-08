Temps de parcours pendant la fermeture de l'A13.
###################################################

Compte : trafic.diridf

MyDrive : /tempsGoogle/A13 (NoteBook ...)

Projet : TempsParcours 	// id:tempsparcours

function : evol-enr-temps-big-query

bigquery : `tempsparcours.temps_google.A13-2024`

application : https://github.com/dirif25non-partage/tempsA13

Création le 3/6/24

Modification le 19/6


Traitements
*************
Une fonction (evol-enr-temps-big-query) interroge tous les quarts d'heure les temps Google sur 8 OD. Les temps reçus sont enregistrés dans la table :code:`tempsparcours.temps_google.A13-2024`.



