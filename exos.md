1-Lire le livre blanc: https://bitcoin.org/bitcoin.pdf, cherchez une version française si vous avez du mal avec l'anglais. (Mais dans ce cas vous risquez d'avoir du mal avec la Blockchain tout court).

2-Un arbre de merkle nécessite une paire de hashes pour produire un nouveau hash parent. Il faut donc a absolument que le nombre de transactions qui produiront le Merkle root soit pair.
Comment est géré le cas ou le nombre de transactions dans le Block à valider est impair pour générer un Merlke root ?

      - L'arbre de merkle est un arbre binaire, donc besoin d'avoir un nombre pair de noeuds, si le nombre de transactions est impair, le dernier hachage sera dupliqué une fois pour créer un nombre pair de noeuds;;

3-Dans le réseau bitcoin, Comment un nouveau noeud arrive t'il à retrouver ses pairs et ainsi rejoindre le réseau ? Expliquer le processus avec vos propres mots.

      - Un nouveau noeud arrive à retrouver ses pairs grace au noeuds d'amorçage qui sont utilisés pour localiser les noeuds actifs.
      Autrement dit, les oeuds d'amorçage ne sont utilisés que pour localiser ou trouver des noeuds complets exécutant le client Bitcoin. Quelque chose comme un carnet d'adresses qui indique aux autres noeuds à qui ils doivent s'adresser pour faire partie du réseau. 

4-Pouvez vous nommer au moins une personne qui a ou aurait pu influencer directement ou indirectement la création de Bitcoin par ses travaux (une personne qui n'a pas été nommée dans le cours)?

      - La première étude sur les chaînes de blocs cryptographiquement sécurisées a été décrite en 1991 par Stuart Haber et W. Scott Stornetta

5-Avec vos propres recherches et grâce aux compétences acquises en cours pouvez vous expliquer comment une Blockchain crée un lien entre ses différents Blocks?

      - Les transactions effectuées entre les utilisateurs du réseau sont regroupées par blocs. Chaque bloc est validé par les noeuds du réseau appelés les “mineurs”, selon des techniques qui dépendent du type de blockchain. Dans la blockchain du bitcoin cette technique est appelée le “Proof-of-Work”, preuve de travail, et consiste en la résolution de problèmes algorithmique.



6-Quelle structure de données informatique peut représenter le mieux cette chaine de Block: https://en.wikipedia.org/wiki/List_of_data_structures ?

7-Si je souhaite modifier une transaction de 10 bitcoin que j'ai effectué il y a 6 mois en une        transaction de 1 Bitcoin, que dois je modifier dans la Blockchain et que dois je mettre en oeuvre pour que cette modification persiste ?

      - il faudrait modifier le Merkle path qi lui meme modifierai le Merkle root pour ensuite modifier le Block header mais cela est impossible..


Est ce possible selon vous ? 

      - je ne pense que cela soit possible, il faudrait pouvoir modifier toutes les verifications faite depuis 6 mois par tous les mneurs de la planete..