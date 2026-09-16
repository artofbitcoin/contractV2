# 2. PMM et formation du prix

Le PMM de DODO adapte la profondeur autour d’un prix externe. La formule dépend du ratio entre les réserves, du prix cible et d’un coefficient de kline qui règle l’agressivité de la courbe.

Cette approche permet une liquidité plus concentrée qu’un invariant constant classique lorsque le prix de référence reste fiable. En contrepartie, une erreur ou une latence de l’oracle peut déplacer la courbe dans une mauvaise zone.

Les fonctions de swap calculent le montant reçu, appliquent les frais et mettent à jour les réserves. Les arrondis et l’ordre des opérations sont essentiels pour éviter une sortie supérieure à la réserve disponible.

Le code distingue les cas où le pool est équilibré, déficitaire ou excédentaire. Ces branches doivent être lues avec les bornes de prix et les protections de slippage.

Suite : [liquidité et contrôles](03-liquidite-controles.md).
