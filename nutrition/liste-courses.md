# Rotation nutrition — 4 semaines

Pour **varier les repas**, 4 semaines types tournent en boucle :

| Semaine | Thème | Fichier |
|---|---|---|
| S1 | Base océan (thon/poisson blanc, riz + patate douce) | [semaine-1.md](semaine-1.md) |
| S2 | Volaille & taro (poulet/dinde, taro + uru + pomme de terre) | [semaine-2.md](semaine-2.md) |
| S3 | Mix & légumineuses (poisson/poulet/bœuf maigre, riz + lentilles) | [semaine-3.md](semaine-3.md) |
| S4 | Poisson gras & varié (saumon/crevettes, quinoa + fei) | [semaine-4.md](semaine-4.md) |

Puis on repart sur S1.

Chaque fichier contient **3 blocs cohérents entre eux** :
1. **Liste de courses** de la semaine (2 personnes)
2. **Plats à préparer** cette semaine (batch cooking + plats)
3. **Menus jour par jour**, portions **Evan / Compagne**, avec horaires et
   consignes pré / post-séance

## Cibles (identiques d'une semaine à l'autre)

| | Evan | Compagne |
|---|---|---|
| Jour muscu / judo | ~2450 kcal · ~200 g prot | ~2050 kcal · ~170 g prot |
| Samedi (repos) | ~2250 kcal | ~1900 kcal |
| Dimanche (vélo long) | ~2550 kcal | ~2150 kcal |

## Calcul de la semaine en cours

`index = (nombre de semaines entières écoulées depuis le lundi 14 septembre 2026) mod 4`
→ 0 = S1, 1 = S2, 2 = S3, 3 = S4.

- Semaine du lun. 14 sept → **S1**
- Semaine du lun. 21 sept → **S2**
- Semaine du lun. 28 sept → **S3**
- Semaine du lun. 5 oct → **S4**
- Semaine du lun. 12 oct → **S1** … et ainsi de suite jusqu'au 14 novembre.

## Envoi automatique

Chaque **samedi 8h04 (Tahiti)**, la routine cloud
`trig_015QM4a1cDFmWZn5KVTsaPtj` envoie par mail à cadetjolif@hotmail.fr la
semaine type correspondante (liste de courses + plats + menus jour par jour de la
semaine à venir).

## À recaler tous les ~15 jours

Quand les poids baissent, les portions doivent baisser (~−5 %). Demande la
régénération des 4 semaines types et la mise à jour de la routine avec les
nouveaux poids. Voir [context/nutrition.md](../context/nutrition.md) §4-5.

## Méthode et compléments

Listes d'aliments, méthode des portions à la main, protocole créatine + whey,
apport avant-séance, hydratation : [README.md](README.md).
