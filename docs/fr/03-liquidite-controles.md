# 3. Liquidité, dépôts et retraits

Les pools DODO peuvent accueillir des fournisseurs qui déposent un ou deux actifs selon le type de marché. Le pool émet des parts et suit les réserves réellement disponibles.

Le retrait recalcule la quote-part du fournisseur à partir de l’état courant. Une liquidité mal valorisée, une réserve insuffisante ou une modification de paramètre peut rendre l’opération moins favorable que prévu.

Les contrats vérifient les montants minimums, les autorisations de transfert et les limites de frais. Les routeurs simplifient l’expérience mais ajoutent une surface d’appel externe qui doit rester cohérente avec le pool.

La création d’un pool et son enregistrement dans les usines sont des étapes distinctes. L’adresse de l’usine, le registre des mainteneurs et les droits d’administration font partie du modèle de confiance.

Suite : [gouvernance et limites](04-gouvernance-limites.md).
