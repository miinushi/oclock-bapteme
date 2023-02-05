Salut ! Je vais avoir comme mission de t'apporter un feedback sur ton travail dans la réalisation d'un MCD

En avant toute ! 

# Review

- La table Address:
    - Il faudra que tu renommes le champ "adress" car il est mal orthographié 
    - Il faudra également modifier la cardinalité 0, N avec User en 1, N car dans un modèle classique, lorsque l'User se login, il devrait avoir au moins une adresse

- La table Product:
    - Tu devras également changer la relation Many To Many qui ne se représente pas exactement comme ça dans le langage merise, tu devrais le représenter via l'utilisation de cardinalités 0, N/1, N <=> 0, N/1, N
    - Tu peux aussi renommer le champ "amount" en "price", car avec "amount" on pourrait croire à un nombre et non un prix

- La table Order:
    - Il faudrait renommer le champ "total_amount" en "total_price" pour les mêmes raisons que Product

- Toutes les tables:
    - Dans le langage merise, l'id doit être mis en valeur, il faudrait donc le souligner

# Feedback général:

- Ce MCD est un bon départ, il y a encore un peu de travail à faire notamment :
    - Gestion des stocks, là il n'y en a pas, ce qui ne permet pas de constituer un site e-commerce correctement 

- En plus des choses manquantes, il y a quelques problèmes de conception généralisés, des manquements:
    - Sur le produit, aucune table "Product Image" n'est disponible, comment les images sont stockées ? Je pense que tu pourrais l'inclure
    - Sur le produit, le système pourrait posséder un système de "Product Variant" pour désigner une variante de produit, car actuellement tu le représentes au travers du champ "type" mais c'est très peu scalable dans un site e-commerce qui "évolue".
    - Sur le user, on ne sait pas comment est stocké le mot de passe, mais le nommage du champ "password" laisse croire que celui-ci est stocké en clair, ⚠️ il doit être stocké sous forme de hash via une méthode adaptée (argon2i par exemple).
    - Sur toutes les tables, des champs de temporalité pourraient être un plus, tels que des champs "created_at", "updated_at" afin d'obtenir plus de contexte sur la création de tel Utilisateur, Order, Product ou Adress

# Ressources 

- Logiciel pour les MCD 
    - [GitMind](https://gitmind.com/fr/)
    - [Visual Pardigm](https://www.visual-paradigm.com/)
    - [Draw.io](https://draw.io/)

- Documentation autour du MCD 
    - [Première documentation](https://www.base-de-donnees.com/mcd/)
    - [Deuxième documentation](https://web.maths.unsw.edu.au/~lafaye/CCM/merise/mcd.htm#:~:text=Le%20mod%C3%A8le%20conceptuel%20des%20donn%C3%A9es,l'aide%20d'entit%C3%A9s)
    - [La cardinalité](http://tony3d3.free.fr/files/Les-Cardinalites.pdf)

- Les mots de passe 
    - [Pourquoi hasher les mot de passe](https://security.stackexchange.com/questions/36833/why-should-i-hash-passwords)

# Bilan

Ce MCD est un bon départ mais il te reste encore un peu de travail pour le finir complètement. il manque quelques éléments et il y a encore des modifications à apporter afin d'être complètement finis.
