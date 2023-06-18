ALGO TantQue1A3

VARIABLES
  nb : entier

DÉBUT

    ÉCRIRE("Saisir un nombre entre 1 et 3")
    LIRE(nb)

    TANT QUE (nb < 1) OU (nb > 3) FAIRE

        

        ÉCRIRE("Saisie incorrecte veuillez recommencer")
        LIRE(nb)

    FIN TANT QUE

    ÉCRIRE("Bravo ! La saisie est correcte !")

FIN

--------

### Exemple d'éxécution

// nb vaut 4
// 4 < 1 ET 4 > 3
// FAUX ET VRAI
// FAUX --> donc on sort de la boucle alors que la saisie est incorrecte

// 4 < 1 OU 4 > 3
// FAUX OU VRAI
// VRAI --> on reste dans la boucle c'est donc le OU qu'il nous faut

