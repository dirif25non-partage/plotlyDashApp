Temps de parcours pendant la fermeture de l'A13.
###################################################

Compte : trafic.diridf

MyDrive : /tempsGoogle/A13 (NoteBook ...)

Projet : TempsParcours 	// id:tempsparcours

function : evol-enr-temps-big-query

bigquery : `tempsparcours.temps_google.A13-2024`

storage bucket : 'itineraires-fermetures'

application : https://github.com/dirif25non-partage/tempsA13

Création le 3/6/24

Modification le 19/6


Traitements
*************
Une fonction (evol-enr-temps-big-query) interroge tous les quarts d'heure les temps Google sur 8 OD. 

La réponse complète à la requête est enregistrée dans Google Storage ('itineraires-fermetures').

Pour limiter le volume stocké sur Storage, on fait une extraction avec le notebook et on enregistre les données sur le DRIVE dans un fichier au format JSON (environ 5 Mo par jour !).

Depuis le 19/6, les temps reçus sont enregistrés dans la table :code:`tempsparcours.temps_google.A13-2024`.

Attention
************
Le gros fichier Json qui enregistre les itinéraires ne comporte pas l'horodatage !

L'heure est contenue dans le nom du fichier.

Il faut faire correspondre les fichiers (DEF qui est la liste des nom de fichiers)

J'ai récupéré 2 fichiers DF mais la mise en correspondance demande des précautions.










