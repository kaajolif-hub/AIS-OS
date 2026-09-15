# Nutrition — descente de poids à deux (14 novembre 2026)

Evan **et sa compagne** préparent la **même poule de sélection le 14 novembre
2026** (Jeux du Pacifique 2027), avec la **même charge d'entraînement**
(3 muscu + 2 judo + 1 sortie vélo longue / semaine). Cette page couvre les deux
profils ; les fiches repas `nutrition/` donnent les portions en **2 colonnes**.

> ⚠️ Plan de travail, pas une prescription médicale. À **valider avec le coach
> et/ou un diététicien du sport**, surtout la partie "fin de parcours". Des
> descentes rapides : l'objectif est de les faire **sans perdre de force ni de
> vitesse**.

## Données de départ

| | Evan | Compagne |
|---|---|---|
| Taille | 176 cm | 166 cm |
| Poids de départ | 98 kg (2026-09-09) | 83 kg (2026-09-09) |
| Poids cible | 90 kg le 14/11/2026 | 78 kg le 14/11/2026 |
| À perdre | ~8 kg (~9 sem) | ~5 kg (~9 sem) |
| Âge | 28 ans | 25 ans |
| Compléments | Créatine + whey | Créatine + whey (mêmes doses) |
| Entraînement | identique | identique |

## 1. Dépense énergétique (méthode)

**Métabolisme de base — Mifflin-St Jeor :**
- Homme : `MB = 10 × poids + 6,25 × taille − 5 × âge + 5`
- Femme : `MB = 10 × poids + 6,25 × taille − 5 × âge − 161`

| | Evan (98 / 176 / 28) | Compagne (83 / 166 / 25) |
|---|---|---|
| Métabolisme de base | ~1945 kcal | ~1580 kcal |
| Facteur d'activité | ×1,6 | ×1,6 |
| **Dépense totale (TDEE)** | **~3110 kcal/j** | **~2530 kcal/j** |

## 2. Déficit visé

| | Evan | Compagne |
|---|---|---|
| Déficit/jour | −600 à −700 | −450 à −550 |
| **Apport de départ** | **~2450 kcal/j** | **~2050 kcal/j** |
| Perte visée | 0,6–0,7 kg/sem | 0,45–0,55 kg/sem |
| Par l'alimentation sur 9 sem | ~5,5–6,5 kg | ~4–4,5 kg |

Le reste (jusqu'au poids exact) se joue sur les **derniers jours**, en affinage
contrôlé (eau, glycogène, résidus digestifs) **avec le coach** — jamais une coupe
d'eau sauvage, surtout si la pesée est le jour du combat.

## 3. Macros au départ

| Macro | Evan (~2450 kcal) | Compagne (~2050 kcal) |
|---|---|---|
| Protéines | **~200 g** (2,2 g/kg cible) | **~170 g** (2,2 g/kg cible) |
| Lipides | **~75 g** (fourchette 65–85) | **~62 g** (fourchette 55–72) |
| Glucides | **~230 g** | **~195 g** |

**Périodisation des glucides** (identique pour les deux, en proportion) :
- Jours muscu (lun/mer/ven) et judo (mar/jeu) : glucides en haut de fourchette, surtout autour de la séance.
- Dimanche (vélo long) : glucides hauts.
- Samedi (repos) : glucides bas, le déficit se creuse ce jour-là.

## 4. Cibles par palier de poids

Le TDEE baisse avec le poids. Recale à chaque palier de 2 kg.

**Evan**

| Poids | TDEE (×1,6) | Apport cible | Protéines |
|---|---|---|---|
| 98 kg | ~3110 | ~2450 kcal | ~200 g |
| 94 kg | ~3050 | ~2400 kcal | ~195 g |
| 90 kg | ~2985 | ~2450 kcal (maintien) | ~190 g |

**Compagne**

| Poids | TDEE (×1,6) | Apport cible | Protéines |
|---|---|---|---|
| 83 kg | ~2530 | ~2050 kcal | ~170 g |
| 80 kg | ~2490 | ~2000 kcal | ~170 g |
| 78 kg | ~2450 | ~2050 kcal (maintien) | ~165 g |

## 5. La règle d'ajustement (le vrai pilotage)

On ne fait pas confiance au calcul, on fait confiance à **la balance sur 7 jours**.

Chaque dimanche, regarde la **moyenne des 7 pesées du matin** (voir
[tracking/poids.md](../tracking/poids.md)) :

- Perte de **0,5 à 0,8 kg** sur la semaine → **on ne touche à rien**.
- Perte **< 0,4 kg** deux semaines de suite → **−150 à −200 kcal/jour** (glucides).
- Perte **> 1 kg** OU baisse de perf / sommeil dégradé / faim ingérable → **+150 à 200 kcal/jour**.
- Poids qui stagne 10 jours → vérifier d'abord le sommeil et la rigueur avant de couper.

## 6. Garde-fous

- Plancher sans avis d'un diététicien : **~2100 kcal/j pour Evan**, **~1600 kcal/j pour la compagne**.
- Protéines : ne jamais sacrifier, même les jours bas.
- Si une séance muscu chute nettement en charges (voir `session-notes/`), c'est un
  signal que le déficit est trop agressif → remonter.
- Semaine de la poule (10–14 nov) : protocole spécifique **défini avec le coach**,
  pas improvisé ici.

## 7. Fiches repas — rotation de 4 semaines

Dossier [nutrition/](../nutrition/) :
- [README](../nutrition/README.md) — listes d'aliments, méthode des portions, protocole compléments, avant-séance
- [liste-courses.md](../nutrition/liste-courses.md) — index de la rotation + calcul de la semaine en cours
- [semaine-1](../nutrition/semaine-1.md) → [semaine-4](../nutrition/semaine-4.md) — 4 semaines types (liste de courses + plats + menus jour par jour, portions Evan / Compagne)

Envoyées automatiquement chaque samedi (routine `trig_015QM4a1cDFmWZn5KVTsaPtj`).

## 8. Suivi

- Poids : [tracking/poids.md](../tracking/poids.md), pesée chaque matin, moyenne 7 j le dimanche.
- Perf : [session-notes/](../session-notes/) — si les charges baissent, le signaler.
- Point hebdo : chaque dimanche, ajustement selon la règle du §5.
