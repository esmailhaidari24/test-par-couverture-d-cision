
+ fonction calculateDiscount(nombreArticles : entier, clientExistant : booléen, typeClient : chaîne, jourFerie : booléen) : décimal
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



![](https://github.com/esmailhaidari24/test-par-couverture-d-cision/blob/main/Capture%20d%E2%80%99e%CC%81cran%201403-06-06%20a%CC%80%2021.26.37.png)

![](https://github.com/esmailhaidari24/test-par-couverture-d-cision/blob/main/Untitled%20Diagram-Page-1.drawio%20(1).pdf)
