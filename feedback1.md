# Avis apprennant numéro 1 

Hello ! Je vais avoir le plaisir de te faire un petit retour sur ton projet

On va voir ensemble les points forts et faibles de ton projet et les pistes d'améliorations susceptibles de t'aider dans ta progression de futur développeur :)

## Points forts 

- Tu as compris l'importance de dotenv, en particulier pour les données sensibles de ton application telle que l'adresse de ta base de données Postgres. Cependant, assure-toi d'inclure la variable SESSION_SECRET dans ton env.example, car actuellement elle n'est pas incluse et cela peut causer des problèmes lors de l'installation.
 
- Tu as respecté les consignes et même réussi à obtenir des bonus.

- Tu as compris les avantages des contrôleurs et des middlewares pour organiser efficacement ton code (et faciliter ainsi la maintenance).

- Tu as bien défini tes routes et même pensé à une route 404 pour les entrées incorrectes.

- On peut voir tes efforts pour gérer l'asynchronisme et les erreurs.

- Tu as compris l'importance de l'architecture MVP.

- Ton code est bien commenté.

- Les noms des fonctions et des variables sont simples et clairs.


## Points faibles 

- Il serait très important de travailler sur la validation des entrées utilisateur pour éviter les potentielles failles de sécurité. 

- Ce serait bien d'implémenter une gestion d'erreur plus complète pour tous les endroits sensibles de ton code.

- Pense à protéger tes requêtes SQL pour éviter les failles SQL. (Par exemple, la concaténation est très déconseillé dans une requête SQL)

- Il serait également bien de revoir la recherche par valeur pour implémenter une requête dynamique qui dépend du paramètre "direction".

- Il est important d'encrypter les objets de session pour limiter les failles de sécurité. ([Article](https://blog.jscrambler.com/best-practices-for-secure-session-management-in-node) qui en parle)

- Essaie de comprendre pourquoi certaines fonctions semblent abandonnées ou commentées et pense à les nettoyer pour faciliter la compréhension du code.

## Conseils 

- L'utilisation de position: fixed pour l'en-tête et le pied de page peut causer des problèmes d'affichage sur certaines résolutions d'écran ou navigateurs 

- Pense à vérifier la limite de la taille du deck dans le contrôleur pour rendre le code plus clair et compréhensible.

- N'oublie pas de configurer les sessions pour les définir sur leur durée de vie.

## Ressource 

Quelques ressources ci-dessous peuvent t'aider à mieux comprendre les points que je t'ai donnés :

- [Pour les sessions](https://www.section.io/engineering-education/session-management-in-nodejs-using-expressjs-and-express-session/)

- [Pour les injections SQL](https://www.stackhawk.com/blog/node-js-sql-injection-guide-examples-and-prevention/)

- [La gestion des erreurs](https://developer.mozilla.org/fr/docs/Web/JavaScript/Guide/Control_flow_and_error_handling)


## Bugs 

J'ai repéré certains bugs dans ton projet, voici la liste:

- Sur la page de résultat d'une recherche par élément, un NaN s'affiche en haut
- Sur la page de la carte, certains éléments apparaissent avec une catégorie "empty"
- Sur la partie bonus "recherche par valeur", la sélection est "strictement égale" alors que nous demandons une sélection "strictement égale ou supérieure à".

## Bilan 

Tout d'abord, Félicitation ! 

On voit bien ta progression et ton envie de bien faire en matière de code ! 

Il te reste encore quelques points à améliorer mais dans l'ensemble, je trouve ton projet très encourageant. Continue comme ça !

Avis personnel RAS projet validé 