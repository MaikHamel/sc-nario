# Présentation d'une scénarisation d'un projet multimedia


## Idee simplifié
Les spectateurs se trouvent dans un forêt magique/fantastique/d'un monde parallèle où ceux-ci interagissent avec des créatures prenant forme de végétaux.


## Mise en contexte
Les spectateurs se  situent dans une pièce représentant une foret dans un monde parallèle. La pièce est rempli de lumières de différentes types et formes, représentant des créatures lumineuses en forme de végétation. Ces lumières suivront continuellement des motifs lumineux. Lorsque les spectateurs sont dans le champ de détection, proche des lumières, ces lumières, changeront changeront de vitesse, de luminosité et de motif, comme si ceux ci veulent communiquer avec les spectateurs.  De plus, lorsque les spectateur toucheront les lumières ceux-ci changeront de couleur ou de motif. Lorsqu'une lumière est touché et change de couleur, tous les lumières autour de celle-ci changeront de couleur, pour avoir le même que le lumière touché, comme si tout les lumières représente un biome, un tout."

## Interaction avec les sectateurs
#### Proximité et Réactions des Lumières
Lorsque les spectateurs s’approchent des lumières, celles-ci réagissent de manière dynamique. Elles modifient leur vitesse, leur luminosité et leur motif lumineux en fonction de la proximité des spectateurs. Cette interaction donne l'impression que les lumières tentent de communiquer ou de répondre aux visiteurs.

#### Au toucher
Lorsque les spectateurs touchent une lumière, celle-ci change de couleur et de motif. Cet acte provoque une réponse synchronisée : toutes les lumières environnantes adoptent la même couleur et motif que la lumière touchée. Cette interaction crée l’illusion que les lumières représentent un biome cohérent, où chaque lumière est interconnectée et influencée par ses voisines, renforçant ainsi l’idée d’un tout harmonieux.

## Animation au repos
Lorsque les créatures (lumières) ne reçoivent pas d'interactions de la part des visiteurs, ceux-ci suivent des motifs de manière continuelles. À certain moments, une lumière change de motif, de manière a communiquer avec une autre lumière, qui répondra  à son tour.

## Effet sonore et musique d'ambiance

Chaque motif lumineux, lorsqu'il y a pas d'interaction avec le visiteur, a sa propre ambiance musicale. Lorsque le spectateur interagit avec une lumière, celle-ci émet un son aléatoirement venant d'une banque de son (effet sonores). Lorsque les lumières autour de celle-ci réagissent, un son similaire et reproduit par ceux-ci. 


## Scénario interactif

```mermaid
graph TD;
    L[Le visiteur entre, admire la piece et se promene dans la foret] --> A
    A{Visiteur s'approche des lumieres} --> B[Le motif des lumieres change]
    A --Le visiteur ne fait rien -->D
    A -->E[Des effets sonores se fait entendre]
    A --> G{Le visiteur touche la lumiere}
    B --> C{Le visiteur recule}
    C -->D[Les lumiere reviennent a leur motif original]
    C --> F[Les effets sonores s'atténuent]
    E --> C
    G --> H[La lumiere réagit]
    G --> I[Un effet sonore se fait entendre]
    H --> K[Les lumieres autour de celle-ci réagissent à leur tour]
    I --> K

    
