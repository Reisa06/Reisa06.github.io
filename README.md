Readme

------------------------ Modification des images

img: getImg("Spearmen", "c0392b") }
Remplacer : img: "liendelimage" }

------------------------ Personnage commun et unique :

isCommander: true
isUnique: true

Ou "false" évidemment :)

------------------------ Type d'unité :

unitType: "Infantry"

Ou "Cavalry" ; "Monster" ; "War Machine" ; "None"

------------------------ Type d'Attachment :

Base de données mise à jour :

Tous les attachements ont maintenant un attType (1 par défaut).

Type 3 (Bastard's Boys) : Configuré pour Sour Alyn, Grunt, Damon, Ben Bones, Skinner.

Type 4 (Compagnons) :

- Bitter : Ne s'active que si Rorge est présent dans l'unité.

- Theon Greyjoy : Ne s'active que si Ramsay Snow (Commander ou Attachement) est présent.

Moteur de Restrictions (Invisible) :

    Quand tu ouvres la fenêtre d'attachement, le système analyse ce qu'il y a déjà dans l'unité.

    Règle Type 1 (Classique) : Impossible d'ajouter si l'unité a déjà un attachement de Type 1 (ex: Capitaine).

    Règle Type 2 (Pas de règle) : Peut être ajouter avant ou après n'importe quel Attachment.

    Règle Type 3 (Additionnel) : Impossible d'ajouter si l'unité a déjà un autre Type 3 (on ne peut pas avoir Skinner ET Ben Bones). Mais on peut avoir un Capitaine (Type 1) ET Skinner (Type 3).

    Règle Type 4 (Conditionnel) : Le bouton est grisé si l'attachement requis n'est pas trouvé dans l'unité.

    Ordre de recrutement : Selon ta règle pour le Type 1 ("ne peut pas être attaché à une unité qui a déjà un attachment"), il faut toujours ajouter le Type 1 en premier (le Capitaine), puis le Type 3 (le Bloody Mummer). Si tu mets le Type 3 en premier, le Type 1 sera bloqué car l'unité n'est plus vide.
