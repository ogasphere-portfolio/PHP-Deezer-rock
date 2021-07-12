# Challenge Deezer Rock

Exercice de révision sur PHP et les tableaux associatifs et multidimensionnels

## Instructions

### Groupes

- Consigner les informations fournies dans un tableau associatif ci-dessous dont les clés sont _"name", "fans", "active", "members"_ : identifier le type de variable correspondant à chaque donnée.
- Afficher un tableau HTML _par groupe_ sous la forme :

| ~~The Beatles~~ |
| ----------- |
| 3 412 906 fans |
| *Members* |
| John Lennon, Paul McCartney, George Harrison, Ringo Starr |

- Si le groupe n'est plus actif son nom sera barré via la balise HTML `<del></del>`.
- Afficher le nombre de fans avec un séparateur ' ' tous les 3 chiffres, voir la [fonction PHP number_format](http://php.net/manual/en/function.number-format.php).
- Afficher 2 liens au-dessus des tableaux pour filtrer par groupe _actif, inactif_ ou _tous_ : traiter la demande via un paramètre d'URL et la variable $\_GET (lien direct via `<a href` ou via formulaire selon votre préférence) : n'afficher que les groupes concernés par le filtre !

<details>
    <summary>Liste des groupes</summary>

    - Nom du groupe
    - Nombre de fans du groupe
    - Groupe toujours actif ou non
    - Membres du groupe

    ```
    Louise Attaque
    336014
    true
    Gaëtan Roussel, Arnaud Samuel, Robin Feix, Alexandre Margraff

    Coldplay
    11343676
    true
    Chris Martin, Guy Berryman, Jon Buckland, Will Champion

    U2
    3776210
    true
    Bono, The Edge, Adam Clayton, Larry Mullen Junior, Ivan McCormick, Peter Martin, Dik Evans

    Queen
    5531303
    false
    Freddie Mercury, Brian May, Roger Taylor, John Deacon, Mike Grose, Spike Edney, Doug Bogie, Barry Mitchell

    The Beatles
    3412906
    false
    John Lennon, Paul McCartney, George Harrison, Ringo Starr

    The Rolling Stones
    3977329
    true
    Mick Jagger, Keith Richards, Ron Wood, Charlie Watts

    Nirvana
    6226653
    false
    Kurt Cobain, Dave Grohl, Krist Novoselic, Pat Smear

    Pink Floyd
    3507791
    false
    David Gilmour, Roger Waters, Syd Barrett, Richard Wright, Nick Mason
    ```
</details>

### Commentaires

- Consigner les informations fournies dans un tableau associatif dont les clés sont _"pseudo", "seconds", "comment", "category"_ : identifier le type de variable correspondant à chaque donnée.
- Sous les groupes, afficher sous forme de liste HTML les commentaires de la catégorie : on affichera le nombre d'heures, minutes et secondes depuis que le commentaire a été posté et seulement si le commentaire a été posté il y a moins d'un jour et s'il appartient à la catégorie _"rock"_, soit si on décompose :
    - Boucler sur les commentaires.
    - Afficher l'auteur, afficher le temps écoulé (convertir le nombre de secondes en `h:m:s` via une fonction utilisateur que vous créerez) puis afficher le commentaire.
    - Et seulement si le commentaire a été posté il y a moins d'un jour et s'il appartient à la catégorie _"rock"_.

**Exemple :**

- **Clément** _Il y a 2h 3min 5s_ : Du rock ? Mon oeil !
- **java57** _Il y a 1h 38min 12s_ : Le meilleur groupe de rock de tous les temps !


<details>
    
<summary>Liste des commentaires</summary>

- Pseudo
- Nombre de secondes depuis quand a été posté le commentaire
- Commentaire posté
- Catégorie du commentaire

    ```
    Clément
    89037
    Du rock ? Mon oeil !
    rock

    java57
    9837
    Le meilleur groupe de rock de tous les temps !
    rock

    Yacham
    9737
    Faites un ptit tour sur ma playlist
    rock

    Suzanne
    8737
    j'adore ça je kiffe Freddy mercury
    jazz

    rv41
    8012
    Jamais, jamais il y aura un autre freddy....25ans snif
    rock

    gerty50
    7500
    nostalgie !.... mais que cela fait du bien d'écouter cette voix superbe !...
    rock

    Myriam Claude Chardon
    7620
    grosse pensée pour toi mon Fab!!!! tu me manques .....
    rock

    Bastien Dja Daouadji
    92047
    Sérieux honteux de mettre en couverture un groupe qui a rien à voir avec le groupe de rock QUEEN Deezer: YOU HAD ONE JOB for god sake....
    jazz

    Matthias
    100037
    Groooossse erreur ils ont mélangé les morceaux du vrai Queen avec un homonyme vraiment pourri
    jazz

    Rockeur
    5432
    playlist de métal svp metter des commentaires http://www.deezer.com/playlist/1368668055
    rock

    BRU NOI
    356
    http://www.deezer.com/playlist/1215050481
    rock

    gregmax46
    215
    Un des plus grand groupes de rock Freddie Mercury un phénomène sur scéne
    jazz

    ```

</details>

### Consignes de code

- Pensez à indenter votre code (espaces pour délimiter les blocs if et les fonctions notamment).
- Commentez votre code afin d'expliquer ce que vous faites à quelqu'un qui lirait votre code pour la première fois (ou vous-même par la suite ;)).

---
