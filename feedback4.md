# Avis apprennant numéro 4
 
## Points forts 

- Tu utilises correctement l'asynchrone dans ton code  
- Tu as essayer de gérer les erreurs avec notamment des blocs try/catch (cependant, attention à bien le faire partout, connection bdd etc)
- La fonction getCard permet de récupérer une seule carte en fonction de son ID.  (Tu as bien compris l'objectif du data mapper)
- Les routes sont clairement définies avec des URL et des méthodes HTTP dédiées pour chaque route (GET pour la page d'accueil, la page de recherche et la page de la carte) et sont dans un fichier séparer pour une 
meilleures maintenabilités.
- Tu serts correctement ton dossier public
- Le code définit le port de l'application en utilisant la variable d'environnement PORT ou en utilisant la valeur 1234 par défaut

## Points faibles 

- Il n'y a pas de gestion des erreurs pour les entrées utilisateur et [cela pourrait être une source de vulnérabilité](https://cheatsheetseries.owasp.org/cheatsheets/Input_Validation_Cheat_Sheet.html#:~:text=Input%20validation%20is%20performed%20to,malfunction%20of%20various%20downstream%20components.)
- Les informations sur les erreurs sont simplement consignées dans la console , ce qui peut rendre difficile le débogage ultérieur.  
- Le rendu de la vue n'est pas complètement défini pour la méthode cardPage. (Tu as mis un objet vide)
- La méthode searchPage ne fait rien d'autre que le rendu d'une vue, il faudrait y ajouter la logique métier (on récupére la donnée en BDD et on l'envoie via la vue par exemple)
- L'emplacement de la photo de la carte n'est pas clairement défini (attention au erreur)
- Le code n'implémente aucune fonction pour se déconnecter de la base de données (Il faudrait faire une fonction pour te déconnecter de la base avant de sortir de ton programme)
- Le code n'utilise pas de validation pour s'assurer que l'ID passé à la fonction getCard est valide (Imagine si j'envoie par exemple "banane" au lieu d'un vrai id)
- Dans dataMapper.js tu importes request mais tu ne l'utilises pas 
- Le code s'arrête à l'étape numéro 1 

## Conseils 

Je te conseille vivement de ne pas rester bloqué si tu ne comprends pas une consigne, n'hésite pas à me contacter pour que je puisse t'aider et bien t'expliquer certaines notions qui pourraient te bloquer dans ta 
progression.

## Ressource

- [Comment construire une application avec express et postgreSQL](https://dev.to/glaucia86/developing-a-crud-node-js-application-with-postgresql-4c9o)
- [POO en Javascript](https://developer.mozilla.org/fr/docs/Learn/JavaScript/Objects/Basics)
- [Comment utiliser EJS](https://www.digitalocean.com/community/tutorials/how-to-use-ejs-to-template-your-node-application-fr)
 
## Bugs 

Les fonctions principale du site ne fonctionne plus : 

- Afficher les cartes
- Afficher son deck
- Ajouter des cartes au deck & supprimer 
- Les recherches
 
## Bilan 

Malgré quelques difficultés, je pense que tu as compris quelques notions notamment l'objectif dû data Mapper et des vues. Si tu es bloqué dans ta progression par ce que tu ne comprends pas une consigne ou 
Parce que tu as des lacunes, n'hésite pas à me le faire savoir pour que je puisse t'apporter de l'aide et le soutien pédagogique dont tu as besoin. N'hésite pas non plus à poser des questions durant les cours si tu ne comprends pas un concept.

Accroches-toi, je suis sûr que tu vas y arriver ! :)