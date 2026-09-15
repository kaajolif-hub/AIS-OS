# Decisions Log

Append-only record of meaningful decisions and why they were made. `/level-up` Phase 2 (Method interview) writes scoped automation specs here. You can also append manually whenever you decide something worth remembering.

**Format per entry:**

```
## YYYY-MM-DD — Short title

**Decision:** what was decided.

**Why:** the reasoning, constraints, and what would change your mind.

**Alternatives considered:** what else was on the table.

**Owner:** who's accountable.
```

Keep it terse. Future-you will thank present-you for capturing the *why*, not just the *what*.

---

## 2026-09-10 — Rester strict sur le programme endurance de force

**Decision:** Suivre le programme du Cycle 2 à la lettre : orientation **endurance
de force, 50-55 % 1RM**, 4 x 12. Dès la prochaine séance, revenir dans la bande :
DC ~58-64 kg, tirage ~42,5-47 kg, SDT ~80-88 kg, presse ~170-187 kg (1RM presse
= 340 kg). La séance du 2026-09-10 (DC 70 / tirage 55 / presse 220, soit ~60-65 %)
reste un écart ponctuel non reconduit.

**Why:** Priorité 2 du trimestre = respecter à la lettre les %1RM, séries et reps
du programme. Evan tranche pour la rigueur au programme plutôt que pour un
stimulus force ajouté.

**Alternatives considered:** Maintenir les charges plus lourdes du 10/09 et
assumer la séance du jeudi comme orientée force (position retenue plus tôt le
même jour, puis abandonnée).

**Owner:** Evan Joliv.

**Remplace :** l'entrée "Séance muscu du jeudi assumée en orientation force"
prise plus tôt le 2026-09-10.

## 2026-09-09 — Onboarding : AI OS de préparation judo (Evan Joliv)

**Decision:** Configurer cet AI OS comme un système personnel de préparation à la
compétition (pas une entreprise). Objectif structurant : 90 kg le 14 novembre
2026 pour la poule de sélection des Jeux du Pacifique 2027. Ajout de `tracking/`
(poids matinal + 1RM), `training-plans/` (fiches du coach), `session-notes/`
(modèle + une note par séance), `videos/` (index), et `context/coach.md` +
`context/calendar.md`.

**Why:** Evan s'entraîne en partie en autonomie sur un programme générique du
coach. Ses trois corvées (calcul des charges %1RM, gestion nutrition,
individualisation du programme) sont récurrentes et automatisables — d'où des
fichiers de suivi vivants plutôt que des notes éparses. La grille hebdo des
créneaux est déjà fixée et n'est pas gérée par l'AI OS.

**Alternatives considered:** Rester sur la structure business par défaut du kit
(domaines revenu/clients) — inadaptée. Ne créer aucun dossier et tout garder
dans `context/` — insuffisant pour un suivi quotidien du poids et des charges.

**Owner:** Evan Joliv.

## 2026-09-09 — Cadence : envoi automatique de la fiche muscu par mail

**Decision:** Créer 7 routines cloud "one-shot" (une par séance) qui envoient la
fiche muscu pré-générée à cadetjolif@hotmail.fr à 07:00 Tahiti le matin de chaque
séance des lun/mer/ven jusqu'au 25 sept (fin du Cycle 2). Envoi via le connecteur
Gmail (compte kaa.jolif@gmail.com). Fiche du 9 sept envoyée manuellement depuis
cette session.

**Why:** Option "fiches pré-générées + envois programmés" choisie par Evan. Le
contenu muscu du Cycle 2 est stable (endurance de force 50-55 % 1RM, 4x12), donc
pré-générer est fiable et évite de dépendre d'un accès cloud au repo. One-shot
plutôt que cron récurrent : pas d'envoi fantôme après la fin du cycle.

**Alternatives considered:** Routine cloud récurrente lisant le repo (nécessite
un repo GitHub privé + accès) ; envoi manuel à la demande. La première est le
bon choix quand le programme deviendra plus variable d'une semaine à l'autre.

**Owner:** Evan Joliv.

**Routines :** trig_01UjwZipDMTi9b7YjKEfqhWK (11), trig_01ApRqUvwcGtbehSxUvXXCAW
(14), trig_013hSyk7eGrhikw4Zbrq9kQB (16), trig_01MwCtBtA4CXHnEWmXGAt1gG (18),
trig_01VwzhbMWLhiKhEA9gZHMWyW (21), trig_01Y5UnV9kSYA4ZXgZFHPnLZg (23),
trig_011TxodkzLvageNxE3betZ4A (25). Gérer sur https://claude.ai/code/routines

## 2026-09-09 — Rotation nutrition sur 4 semaines + email hebdo complet

**Decision:** Remplacer les 7 fiches par-jour (`lundi.md`…`dimanche.md`, supprimées)
par **4 semaines types en rotation** : `nutrition/semaine-1..4.md`, chacune
autonome avec liste de courses (2 pers) + plats à préparer + menus jour par jour
(portions Evan/Compagne), les 3 cohérents. Thèmes : S1 base océan, S2 volaille &
taro, S3 mix & légumineuses, S4 poisson gras & varié. `liste-courses.md` devient
l'index de rotation. La routine du samedi (trig_015QM4a1cDFmWZn5KVTsaPtj) embarque
les 4 blocs, calcule `index = (semaines depuis lundi 2026-09-14) mod 4` pour la
semaine à venir, et envoie le bloc correspondant (courses + plats + tous les repas
de la semaine).

**Why:** Demande d'Evan : varier les repas chaque semaine sur un cycle de 4, et
recevoir chaque samedi la liste des repas de la semaine en corrélation avec la
liste de courses. Le cloud n'ayant pas accès au repo, les 4 semaines sont
intégrées à la routine.

**Alternatives considered:** 4 routines séparées (ne tournent pas proprement) ;
une routine lisant le repo (pas d'accès Git).

**Owner:** Evan Joliv (+ compagne). Recaler les 4 semaines types tous les ~15 j
selon les moyennes de balance, puis mettre à jour la routine.

## 2026-09-09 — Passage en version "2 personnes" (Evan + compagne)

**Decision:** La compagne d'Evan (25 ans, 166 cm, 83 kg → 78 kg) prépare la même
poule du 14 nov avec la même charge d'entraînement. Toute la nutrition passe en
2 profils : TDEE ~2530, apport de départ ~2050 kcal, ~170 g protéines. Les 7
fiches `nutrition/` et `liste-courses.md` passent en 2 colonnes / quantités pour 2.
`tracking/poids.md` dédoublé (2 journaux + 2 trajectoires). La routine de pesée
(trig_01WEWWqvxnz7zvn8MMUS3oKk) demande désormais les 2 poids. Nouvelle routine
hebdo (trig_015QM4a1cDFmWZn5KVTsaPtj, cron 4 18 * * 6 = samedi 08h04 Tahiti) qui
envoie liste de courses + plan repas jour par jour de la semaine à venir.

**Why:** Demande explicite d'Evan : liste de courses + plan détaillé jour par
jour, quantités pour 2, envoyé chaque samedi matin. Portions différenciées car
besoins caloriques distincts (ne pas juste doubler).

**Alternatives considered:** Doubler les portions d'Evan — inadapté (la compagne
mangerait ~400 kcal de trop/j). Un plan cloud lisant le repo — pas d'accès Git.

**Owner:** Evan Joliv (+ compagne). À faire valider par un diététicien du sport.
À recaler tous les ~15 jours selon les moyennes de balance.

## 2026-09-09 — Fiches repas jour par jour + âge confirmé (28 ans)

**Decision:** Âge d'Evan = 28 ans → recalage de context/nutrition.md (MB ≈ 1945,
TDEE ≈ 3110, apport de départ ~2450 kcal, ~200 g protéines). Création du dossier
`nutrition/` : README (listes d'aliments locaux, méthode des portions, protocole
créatine 3-5 g/j tous les jours + whey 25-30 g x1-2/j, apport avant-séance,
hydratation) et 7 fiches repas calées sur la séance du jour (horaires, aliments,
quantités en grammes, timing pré/post-entraînement).

**Why:** Evan a demandé des fiches détaillées par jour de la semaine, avec prise
en compte de ses compléments (créatine + whey) et de l'apport avant entraînement.
Les séances tardives (lundi 20h) et d'après-midi (mer/ven) imposent des
structures de repas différentes selon les jours.

**Alternatives considered:** Un seul menu type répété 7 jours — inadapté vu les
horaires de séance variables et le jour de repos / la sortie vélo longue.

**Owner:** Evan Joliv. À faire valider par un diététicien du sport (descente
rapide). Point ouvert : garder ou arrêter la créatine 10-14 j avant la pesée —
décision coach.

## 2026-09-09 — Nutrition + rappel de pesée quotidien

**Decision:** Créer `context/nutrition.md` : méthode de calcul du déficit (Mifflin-St
Jeor × facteur d'activité 1,6, déficit 600-750 kcal, ~2500 kcal au départ,
protéines ~2,2 g/kg poids cible, glucides périodisés), cibles par palier de poids,
et une règle de pilotage basée sur la moyenne 7 jours de la balance. Créer une
routine cloud quotidienne (trig_01WEWWqvxnz7zvn8MMUS3oKk, cron 2 16 * * * UTC =
06:02 Tahiti) qui envoie à cadetjolif@hotmail.fr la question du poids du matin +
l'objectif du jour calculé sur la trajectoire linéaire 98 kg (9 sept) → 90 kg
(14 nov).

**Why:** Evan veut un cadre nutritionnel chiffré et un rappel matinal "sur Claude"
à 6h. Le calcul dépend de l'âge (non fourni — hypothèse 20 ans, à recaler). Sans
repo GitHub accessible au cloud, la routine ne peut pas écrire dans
tracking/poids.md : Evan répond, la valeur est reportée ensuite en session locale
(ou plus tard via un repo privé).

**Alternatives considered:** CronCreate (session-only, expire à 7 jours) et
PushNotification (ponctuel, lié à la session) — aucun n'est durable. Routine cloud
avec repo privé pour boucler l'écriture automatique : à faire quand le repo sera
poussé.

**Owner:** Evan Joliv.

## 2026-09-06 - Audit evidence and routing maintenance

**Decision:** Ship audit rubric v2 and a small /link skill. Audit scores working evidence across the Four Cs, checks operating-manual routing and freshness, and passes one concrete gap into /level-up. A selected repair can improve an existing workflow instead of creating another skill.

**Why:** File counts, configured keys, named rituals, and recent edits do not prove an operational AIOS. Source findability and freshness need explicit checks.

**Alternatives considered:** Keeping presence-based scoring or requiring a hot cache. Neither reliably establishes retrieval quality or successful execution.

## 2026-09-06 - Portable skills and automatic audit history

**Decision:** Ship all four skills for Claude Code and Codex, with bundled resources, matching operating manuals, and a script for regenerating Codex copies. Audit reports are saved automatically, preserve previous runs, and track findings across comparable inspections.

**Why:** Students need the same shared guidance when switching assistants and evidence of actual improvements over time. Intentional runtime adaptations, unknown verification, and confirmed defects are reported separately.

## 2026-09-06 - Portable 3D Brain skill

**Decision:** Add `/3d-brain` for Claude Code and Codex. Ask for a name and categories, map selected local folders, and scaffold a bundled, configurable application with spherical placement, Cinema, and interactive growth replay.

**Why:** Shipping the working renderer preserves the intended appearance and interactions across AIOS installations. A prose-only prompt would produce inconsistent recreations. User config and graph data remain local; the public package includes only code, documentation, dependency notices, and fictional test inputs.

## 2026-09-06 - Add ongoing context interviews

**Decision:** Adapt Herk-2's grill-me skill for the student kit and ship matching Claude/Codex packages. Save every answer to brainstorms/, preserve resumable Q&A history, and update canonical context only with confirmed facts during requested context-building sessions.

**Why:** Onboarding is an initial snapshot. Ongoing interviews capture changing priorities, decisions, and preferences while keeping tentative ideas distinct from current business facts.
