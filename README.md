
1-  fonction calculateDiscount(nombreArticles : entier, clientExistant : booléen, typeClient : chaîne, jourFerie : booléen) : décimal
    remise : décimal = 0.0
    si nombreArticles > 10
        remise = 0.15

    si clientExistant
        remise = remise + 0.05

    si typeClient est "VIP"
        remise = remise + 0.10  # Remise supplémentaire pour les clients VIP

    si jourFerie
        remise = remise + 0.05  # Remise supplémentaire pour les achats pendant les jours fériés

    retourner remise
fin fonction


2- fonction calculerTotalAvecReduction(prixUnitaire : décimal, nombreArticles : entier, estMembre : booléen) : décimal
    reductionTotale : décimal = 0.0
    total : décimal = 0.0
    i : entier = 1

    tant que i <= nombreArticles
        total = total + prixUnitaire

        si estMembre
            reductionTotale = reductionTotale + (prixUnitaire * 0.05)

        i = i + 1

    prixFinal : décimal = total - reductionTotale
    retourner prixFinal
fin fonction





![](https://github.com/esmailhaidari24/test-par-couverture-d-cision/blob/main/Capture%20d%E2%80%99e%CC%81cran%201403-06-06%20a%CC%80%2021.26.37.png)



