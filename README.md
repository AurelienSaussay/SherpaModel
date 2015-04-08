# Modèle Sherpa

Modèle SHERPA, Shale Extraction and Recovery Projection Analysis

Le modèle SHERPA permet la modélisation de gisement de gaz de schiste, pour un ensemble d'hypothèses technico-économiques fournies par l'utilisateur. Il se trouve dans le fichier *SHERPA.xlsx*. Pour en savoir plus, consulter le working paper 	[Can the US shale revolution be duplicated in Europe?](http://www.ofce.sciences-po.fr/pdf-articles/actu/WP2015-10-1-.pdf)

## Scénarios de production

Trois scénarios sont inclus à titre illustratif :

- **Central**
    - Coûts de forage dans la moyenne haute US (10 M$ par puit)
    - Production initiale par puit comparable à la moyenne haute des gisements américains
    - Fréquence de forage significative (30 puits par mois)
- **VAN nulle**
    - Coûts de forage 30% supérieur à la moyenne haute US (13 M$ par puit)
    - Production initiale par puit comparable à la moyenne haute des gisements américains
    - Fréquence de forage significative (30 puits par mois)
- **Extrême**
    - Coûts de forage dans la moyenne haute US (10 M$ par puit)
    - Production initiale par puit comparable au meilleur des gisements américains (Haynesville)
    - Fréquence de forage significative (30 puits par mois)

Deux scénarios complémentaires sont fournis vierges, à la disposition de l'utilisateur.

## Hypothèses et calibration

La calibration du modèle se trouve dans l'onglet *Assumptions*. Les hypothèses paramétrables, qui doivent être entrées dans l'onglet *Scenarios*, sont les suivantes :

- Au niveau du **puits** :
    - **Year 5+ decline rate** : taux de déclin du puits moyen au delà de la 5e année. Les 4 premières années de taux de déclins sont calibrées sur les données de production américaines (voir l'onglet **Assumptions**).
    - **Drilling costs ($)** : coûts de forage et de completion par puits en USD.
    - **Average first day production (Mcf)** : production du puits moyen au premier jour d'exploitation. Combiné aux taux de déclin, cette hypothèse détermine la production totale du puits moyen.
    - **Operating expenses ($/MMBtu)** : coût opérationnel pour la production d'un MMBtu en USD.
    - **Gas prices ($/MMBtu)** : hypothèse de prix moyen retenu pour la période considérée.

- Au niveau du **gisement** :
  - **Maximum drillings per month** : rythme de forage permanent après la période de montée en charge, en puits par mois.
  - **Duration of ramp-up (months)** : durée de la période de montée en puissance du nombre de forage par mois, en nombre de mois.
  - **Duration of production (years)** : durée de la période de forage, en année.
  - **Discount rate** : taux d'actualisation utilisé pour le calcul de la VAN.
  - **Technically Recoverable Resources (Tcf)** : volume total de la ressource gazière techniquement récupérable (en trillion de pieds cubiques).
