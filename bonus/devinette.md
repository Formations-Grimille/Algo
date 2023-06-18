ALGO Devinette

VARIABLES
    nbADeviner, tentative, score: entier

DÉBUT

    score <- 0

    ÉCRIRE("Joueur 1, donne un nombre à faire deviner au joueur 2")
    LIRE(nbADeviner)

    RÉPÉTER

        ÉCRIRE("Joueur 2, tente de retrouver le nombre du joueur 1")
        LIRE(tentative)

        SI (tentative > nbADeviner) ALORS
            ÉCRIRE("Le nombre recherché est plus petit")
        FINSI

        SI (tentative < nbADeviner) ALORS
            ÉCRIRE("Le nombre recherché est plus grand")
        FINSI

        // on incrémente la valeur du score
        score <- score + 1

    JUSQU'À (tentative = nbADeviner)

    SI (score > 1) ALORS
        ÉCRIRE("Bravo tu as trouvé le nombre", nbADeviner, "en", score, "tentatives")
    SINON
        ÉCRIRE("Bravo tu as trouvé le nombre", nbADeviner, "en", score, "tentative")
    FINSI

    // Possible avec un Cas où
    /*
    CAS OÙ score VAUT
        1: ÉCRIRE("Bravo tu as trouvé le nombre", nbADeviner, "en", score, "tentative")
        AUTRE: ÉCRIRE("Bravo tu as trouvé le nombre", nbADeviner, "en", score, "tentatives")
    FINCAS
    */
FIN