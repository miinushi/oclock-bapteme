# Explication fetch

La méthode fetch en JS est utilisée pour récupérer des données à partir d'une URL.

Par exemple, imagine que sur ton site, on veuille récupérer le rendu HTML du détail de la carte qui a l'id numéro 1

On pourrait avoir par exemple :

```js
const card = await fetch('http://localhost:1234/card/1');  
``` 

Ainsi grâce à la méthode fetch, on peut récupérer facilement les détails d'une carte en spécifiant simplement l'URL dans la méthode fetch.

Attention ⚠️, si tu essaies d'exécuter ce code de ton côté, tu obtiendras une erreur liée aux "CORS POLICY".

**Cors Kesako ?**

CORS signifie "Cross-Origin Resource Sharing". Il s'agit d'une sécurité mise en place par les navigateurs pour limiter les requêtes effectuées depuis un site web à d'autres ressources sur d'autres domaines. Si un site web tente d'accéder à une ressource sur un autre domaine sans autorisation, le navigateur bloque cette requête en raison de la politique CORS. Cela empêche les attaques de type "cross-site scripting".

Tu peux utiliser le middleware [cors](https://expressjs.com/en/resources/middleware/cors.html) de express pour autoriser certaines origines à accéder à ton application. 

Tu pourras ensuite même t'amuser à récupérer depuis le HTML de la page des informations précisent que tu voudrais grâce à l'ID par exemple avec un [paquet](https://github.com/jsdom/jsdom) très utilisé dans le [web scraping](https://fr.wikipedia.org/wiki/Web_scraping).

Mais ce n'est pas tout ! Il existe plein de paramètres que tu peux donner à la méthode fetch notamment des fichiers, des paramètres, etc. 

Je te laisse la page de la [documentation](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API) pour que tu puisses voir tout ce qu'il est possible de faire avec la méthode fetch