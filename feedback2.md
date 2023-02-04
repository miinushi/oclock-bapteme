# Avis apprennant numéro 2

Hello ! 

J'ai le plaisir de faire une review de ton code !
 
## Points forts 

- Tu as su tirer parti de l'asynchrone
- Tu as su gérer correctement tes erreurs avec un bloc de code try/catch
- Tu as compris l'intérêt des sessions
- Tu vérifies bien l'existence de la carte avant de l'ajouter à la session
- Tu utilises correctement les objets mis à disposition (req.query par ex)
- Tu filtres tes données de résultats avec filter, ce qui est appréciable
- Tu as bien séparé tes contrôleurs de tes fonctions d'accès à la base de données  (getAllCards(), getElements(), getOneCard())
- Les contrôleurs sont bien séparés et organisés dans différents fichiers
- Définition claire des routes et de leur correspondance avec les contrôleurs
- Tu utilises bien les middleware
- Gestion du port correct en fonction des variables d'environnement ou attribution d'un port par défaut

## Points faibles  

- Pas de commentaire (ce qui peut te limiter si tu reviens sur ton code plus tard par exemple)
- La chaîne secrète de gestion de session devrait être stockée dans un fichier d'environnement externe au lieu d'être stockée en clair dans le code.
- La configuration de session manque de protection HTTPS, ce qui expose les informations transmises à une interception par un tiers.
- Le code manque de validation de l'entrée utilisateur pour les paramètres de requête, ce qui peut entraîner des erreurs dans la requête SQL ou la saisie de données sensibles.
- La gestion des erreurs pour les requêtes à la base de données est absente, ce qui peut causer des problèmes tels que des erreurs non gérées et des temps d'arrêt imprévus.
- Le code ne vérifie pas si la variable d'environnement PG_URL est définie avant de l'utiliser.
- La fonction ne vérifie pas si la variable "cardElement" est vide ou manquante.
- La fonction ne gère pas les erreurs lors de la récupération des cartes depuis la base de données.
- La logique de filtrage des cartes pourrait être améliorée pour gérer les cas d'absence de résultats ou de réponse plus appropriée en cas d'erreur.
- Les réponses en cas d'erreur sont très générales et ne facilitent pas la compréhension de ce qui ne va pas.
- Le code ne gère pas les cas d'entrée incorrecte (comme une entrée non numérique pour req.params.id).


## Conseils  

Je te conseille de prendre connaissance des points ci-dessus et d'essayer de reprendre ton projet pour l'améliorer, je trouve qu'il y a beaucoup de positif dans ton code et qu'on sent que tu veux bien faire ! Une fois que tu auras retravaillé un peu ton projet, prend du recul et tu verras que tu as faits beaucoup de progrès !

## Ressource 

Voici une ressource qui te sera utile : 

[La gestion des erreurs en Javascript](https://developer.mozilla.org/fr/docs/Web/JavaScript/Guide/Control_flow_and_error_handling)

## Bugs 

- Certains détails requis ne sont pas disponibles lorsqu'on clique sur une carte
- Les routes pour la recherche par niveau, valeur et nom sont inexistants
- La fonctionnalité de suppression de carte du deck n'est pas disponible
 
## Bilan

En conclusion, je pense que ton code est plutôt bon, il manque l'application de certaines notions importante (comme la gestion des erreurs, la gestion des null) mais globalement, c'est un bon travail.

N'hésite pas à retravailler le projet pour bien mettre en application mes retours et continuer sereinement ta formation.