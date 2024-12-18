# Présentation d'une scénarisation d'un projet multimedia: Umbrae Arborum
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
    L[Le visiteur entre dans la piece] --> N[Le visiteur admire la piece]
    N -->A
    A{Visiteur s'approche des lumieres} --> B[Le motif des lumieres change]
    A --Le visiteur ne fait rien -->D
    A -->E[Des effets sonores se fait entendre]
    A --> G{Le visiteur touche la lumiere}
    B --> C{Le visiteur recule}
    C -->D[Les lumiere reviennent a leur motif original]
    C --> F[Les effets sonores s'atténuent]
    F --> D
    E --> C
    G --> H[La lumiere réagit]
    G --> I[Un effet sonore se fait entendre]
    H --> K[Les lumieres autour de celle-ci réagissent à leur tour]
    I --> K
    K --> M{Le visiteur retire sa main de la lumiere}
    M -->D
    D --> N
````
## Ambiance
![Desktop - 1](https://github.com/user-attachments/assets/68f36ccf-5758-4596-8822-a8ec2c1a31ff)



# Technologies

## Support médiatique

Lumières interactives

mettre plus de matériel pour avoir un environnement sensible

detecteurs pour chaque branches de lumières
## Matériel
### TOF ( time of flight ) Distance Ranging Sensor Unit
Calcule la distance entre le point émetteur et l'objet détecté en mesurant le temps de trajet aller-retour du signal laser ( pouvant aller jusqu'à deux mêtres.

Lorsque les spectateurs s'approchent des lumieres, le détecteur mesure la proximité de celui-ci et fera réagir les lumieres.

# Références
[capacitive sensor](https://www.bareconductive.com/blogs/resources/make-a-basic-capacitive-sensor-with-electric-paint-and-arduino)<br>

# synoptique

### matériel:
- TOF
- Paquet de 10 LED Strip WS2811
- Arduino microcontroleur
-  Speakers
- Subwoofer
- 1MΩ resistor
- Atom proto kit
- carte de son

### Branchement

```mermaid
flowchart TB
    subgraph ordinateur
    J[comutateur ethernet] --> A
   
    A[ordinateur]
    end
    subgraph speaker
    A --> C[carte de son]
    C --> D[speaker]
    C --> E[subwoofer]
    end
    subgraph microcontroleur
    A --> B[microcontroleur]
     J --> B
   
    end
    subgraph capacitance

    B --> F[Atom proto kit] 
    F --> G[Zone tactile coducteur]
    end
    subgraph tof
    B --> H[TOF]
    end
    subgraph lumiere
    B --> I[lumiere]
    end



```

# Plantation

![Plan_Umbrae Arborum](https://github.com/user-attachments/assets/7b4dc8a6-f874-471b-8e8a-2c6d2151b31b)

## Fleur

![Fleur](https://github.com/user-attachments/assets/3e64b2d3-8cd5-4214-80a8-6d775d3bba99)
![Fleur2](https://github.com/user-attachments/assets/f141b3e3-6af1-4e54-bd08-531dcf461f06)

# Simulation

![3d_projet](https://github.com/user-attachments/assets/aa5d3564-205a-4899-a782-5c6503e4aeaa)

# Scénarimage

![scénarimage_repos](https://github.com/user-attachments/assets/86278ee0-8a08-4b51-b702-f482bbf2a498)

![scénarimage_approche](https://github.com/user-attachments/assets/291cf9ad-a3e9-4671-ad57-a46b35b392c8)

![scénarimage_touche](https://github.com/user-attachments/assets/3e0ebf53-aede-43e1-8153-4f157ceec023)




# Devis Technique

## Matériel
- TOF(?)
- Paquet de 10 LED Strip WS2811(?)
- Arduino microcontroleur(?)
-  Speakers (4)
- Subwoofer(2)
- 1MΩ resistor(?)
- Atom proto kit (?)
- carte de son (1)
- support a plusieurs bras (8)
- supports pour les speakers (4)
- tape
- cable ethernet
- cable électrique
- commutateur ethernet
- ordinateur
- fausses plantes
- fausses plantes sur les murs

## Logiciels
- Ableton live
- Arduino IDE
- Plugdata
- loopMIDI
  

