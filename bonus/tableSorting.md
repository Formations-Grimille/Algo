ALGO TriTableau

VARIABLES
    tab: tableau[5] d'entiers
    i, j, tmp: entier

DÉBUT

    // Remplissage du tableau
    tab[0] <- 9
    tab[1] <- 5
    tab[2] <- 4
    tab[3] <- 1
    tab[4] <- 6

    // compteur(tab) <-- avec cette instruction on obtient la taille du tableau : 5
    POUR i ALLANT DE 0 À compteur(tab) - 2 FAIRE

        POUR j ALLANT de i+1 À COMPTEUR(tab) - 1 FAIRE

            SI (tab[i] > tab[j]) ALORS

                tmp <- tab[i]
                tab[i] <- tab[j]
                tab[j] <- tmp

            FINSI

        FINPOUR

    FINPOUR

FIN