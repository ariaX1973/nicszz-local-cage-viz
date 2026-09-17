# NICSzz local — surfaces 3D et chemins de selle

Visualisation interactive des surfaces continues de **NICSzz local à 1,7 Å**, projetées sur la topologie moléculaire, pour quatre structures : `sat0`, `sat1 trans`, `sat1 cis` et `sat2`.

La visualisation permet de :

- faire pivoter, déplacer et zoomer chaque structure en 3D ;
- afficher ou masquer la molécule, la surface NICSzz et le chemin critique ;
- repérer les minima NICSzz associés aux deux cycles ;
- suivre le chemin minimax reliant ces minima sur la surface ;
- identifier le point selle et les barrières NICSzz correspondantes.

## Visualisation en ligne

[Ouvrir la visualisation interactive](https://ariax1973.github.io/nicszz-local-cage-viz/)

Le fichier [`index.html`](index.html) est autonome et peut aussi être téléchargé puis ouvert directement dans un navigateur moderne.

## Méthode

Le tenseur de blindage est projeté sur l'axe normal local de chaque point afin d'obtenir NICSzz dans le repère moléculaire local. Les deux minima sont déterminés à partir des valeurs NICSzz dans les bassins des cycles. Leur connexion suit un chemin minimax de type PES : le point le plus élevé rencontré le long du meilleur chemin constitue le point selle discret.

