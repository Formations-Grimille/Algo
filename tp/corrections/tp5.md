ALGO CalculFacture

VARIABLES
    txTVA, prixHT, prixTTC : flottant
    nbArticles : entier

DÉBUT
    ÉCRIRE("Saisir le nombre d'articles")
    LIRE(nbArticles)

    ÉCRIRE("Saisir le prix HT unitaire d'un article")
    LIRE(prixHT)

    ÉCRIRE("Saisir le taux de TVA (20, 10, 5.5 par exemple)")
    LIRE(txTVA)

    prixTTC <- prixHT * (1 + txTVA/100) * nbArticles
    
    /*
    2 * (1 + 20/100)
    2 * (1 + 0.2)
    2 * 1.2
    2.4 le prix TTC d'un article
    */

    ÉCRIRE("Le prix TTC total est de :", prixTTC, "€")
FIN