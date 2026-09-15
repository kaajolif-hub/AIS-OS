# AIS-OS Intake

This is the source-of-truth file for your AIOS. Fill it in by typing, voice-pasting (Wispr Flow / OS dictation), or running `/onboard` for a guided conversation. Whichever mode, this file is what `/onboard` reads to scaffold your Day-1 setup.

**Hard cap: 7 questions.** Each answerable in under 60 seconds. Don't overthink — you can edit and re-run `/onboard` any time.

---

## Q1 — Who are you, what do you sell, who do you sell it to?

Identity, offer, ICP. One paragraph each is fine.

```
Je m'appelle Evan Joliv. Je suis judoka, 1m76, je pèse actuellement 98 kg.
Objectif : peser 90 kg pour la saison sportive.
Ce n'est pas une activité commerciale — le "client" principal, c'est moi-même.
Cet AI OS est un système personnel de préparation physique et de gestion du poids
pour le judo de compétition.
```

---

## Q2 — Paste 1-2 things you've written recently. Don't edit them.

An email, a LinkedIn post, a DM, a doc — anything that sounds like you when you're not trying. **Paste verbatim.** Do not type these mid-conversation with Claude — chat-shaped samples are worse than no samples (voice contamination).

```
[Sample 1 — réponses d'Evan à un questionnaire post-ascension en montagne, collées brutes]

De quoi avais-je peur avant de vivre cette expérience ?
Alors, ce que j'ai ressenti lors de cette expérience n'était pas forcément de la peur, parce que, pour moi, c'était quelque chose de nouveau, une nouvelle expérience. Donc, j'étais plutôt excité et j'avais hâte de la vivre.

De quoi ai-je eu peur pendant l'ascension ?
Toujours pareil, pas de peur ressentie pendant l'ascension, beaucoup d'excitation, beaucoup de joie et surtout une envie de le refaire et d'aller plus loin, d'être capable de tout faire.

Qu'est-ce que je retiens de cette expérience et/ou qu'est-ce que j'ai appris sur moi ?
Ce que j'ai appris de cette expérience, c'est vraiment ce côté où tout le monde se pousse, tout le monde se tire vers le haut. J'ai fait la descente avec Cyrill, on a longuement discuté et j'ai appris à prendre sur moi et à voir les gens différemment.
Je pense que la montagne nous force à nous unir, à être plus forts, à être conscients des faiblesses et des forces de chacun. Et je te remercie pour cette ascension pour ça, pour m'avoir fait voir les choses différemment, et voir Cyrill différemment.

Quel lien je peux faire avec les valeurs de l'équipe (Tauturu ro'a, Audace, Honneur, Optimisation, Engagement) ?
Je fais le lien avec les deux principes du Tahoe qu'on a faits, le Tauturu où il y a eu beaucoup d'entraide, des attentes, où tout le monde s'aidait à grimper et surtout, surtout à descendre.
Et également beaucoup, l'engagement. Tout le monde s'est engagé. Tout le monde s'est lancé, chacun à son niveau, chacun à ses limites. Et ça, c'était vraiment bien. Et j'en parle encore aujourd'hui avec ma famille, mes proches, que même ceux qui n'ont fait que 20 minutes, je trouve ça génial que malgré eux et certainement leur peur, ils sont venus et se sont engagés à le faire. Et ça, j'ai trouvé ça top.
```

```
[Sample 2 — registre du coach/sélectionneur, pour référence — PAS la voix d'Evan]

Ia ora na tout le monde je viens de vous transmettre le programme prévisionnel du séminaire numéro 1 les 5 et 6 septembre. Le 5 se déroule au dojo de Tefana. Les convocations vous seront envoyées ces prochains jours.

a ora na les amis, suite à la présentation qui a été effectuée ce vendredi je vous transmets les informations utiles, notamment pour celles et ceux qui s'entraînent en autonomie, a savoir le projet de planification de l'entraînement. Je précise que c'est une planification générique. De toute évidence, toute préparation pointue caractéristique de la haute performance légitime des adaptations permettant une individualisation fine de l'entraînement.
Pour autant, les documents transmis sur lesquels je fais un focus aujourd'hui permettent de suivre un cadre de travail cohérent et harmonisé.
Si vous avez des questions, n'hésitez pas à me solliciter.
Pour la musculation, les effets sont largement bénéfiques à notre niveau de performance à partir de deux séances par semaine.
Les séances cardio peuvent venir compenser un manque d'entraînements en judo.
Considérons qu'à 3 séances de randori par semaine, le cardio est un peu moins prioritaire (si vous devez choisir) que les deux séances de musculation.
```

---

## Q3 — What are your 2-3 biggest priorities for the next 90 days?

Quarterly priorities. Not yearly aspirations. Things that, if not done by July, would make you say "I wasted Q2."

```
Échéance cible : 90 kg le 14 novembre 2026 (poule de sélection pour les Jeux
du Pacifique 2027 à Tahiti — Evan est Tahitien).

1. Descente de poids : 98 → 90 kg d'ici le 14 novembre 2026, via nutrition.
2. Musculation : gros focus. Respecter STRICTEMENT les %1RM, séries et
   répétitions prescrits par le programme (le principal risque d'échec identifié
   est de ne pas les respecter en séance).
3. Volume de randori + technique : monter le volume selon le programme,
   travailler la technique.
4. Sommeil : l'améliorer (levier de la descente de poids et de la récup).

Maxes actuels (1RM) :
- Développé couché : 116 kg
- Soulevé de terre (deadlift) : 160 kg
- Tirage barre : 85 kg

Programme en cours (transmis par le coach) — Cycle 2, semaines 4 à 6
(07 sept → 27 sept 2026), semaine 5 (14-20 sept) en cours :
- Musculation : Volume 4 à 6 / Intensité 2 à 4
- Randori : 15 à 25 min — nombre 4 à 5, durée 4 à 5 min
- Endurance de force : 50-55 % 1RM, 4x12 (3 ateliers) + 4x12 (3 mouvements
  complémentaires) + gainage (3 ateliers)
- Capacité aérobie : circuit 5x12 min
- Endurance fondamentale : effort continu 60 min à très faible intensité

Référence de charge : abaque d'orientation de la charge en musculation
(d'après S. Lemaitre / preparation-physique.net) — %1RM ↔ reps ↔ séries ↔ récup
selon l'objectif (Vitesse-Explosivité, Endurance de Force, Puissance, Force Max,
Hypertrophie). À reporter dans references/.
```

---

## Q4 — Where does revenue actually land, and where is it tracked?

Multiple answers OK. Stripe? Skool? GoHighLevel? QuickBooks? A spreadsheet?

```
Adapté : suivi des résultats et des chiffres de perf.

- Poids corporel : pesée chaque matin (actuellement 98 kg). Rien de noté nulle
  part aujourd'hui. → DEMANDE : créer un tableau de suivi du poids matinal
  (date, poids du matin, écart vs objectif 90 kg, note).
- Musculation / 1RM : rien de noté. → DEMANDE : créer un tableau de suivi des
  1RM sur les 3 ateliers cités (développé couché, soulevé de terre, tirage barre).
  Valeurs de départ : DC 116 kg, SDT 160 kg, tirage barre 85 kg.
- Résultats de compétition / classement : rien de formel.
```

---

## Q5 — Where do you talk to customers, your team, and the outside world day-to-day?

Email (which one — Gmail / Outlook)? Slack? Teams? DMs (Skool / Discord / iMessage)? Phone?

```
- Coach / sélectionneur : principalement Facebook Messenger, et aussi par mail.
- Boîte mail principale : Outlook.
- Calendrier (auto-déduit de la messagerie) : Outlook Calendar — à confirmer.
```

---

## Q6 — Where do meeting recordings, notes, and important docs live?

Granola? Otter? Fireflies? Google Drive? Notion? Dropbox? A folder on your desktop you keep meaning to organize?

```
Aujourd'hui : rien n'est rangé correctement. Demandes explicites :

- Créer un dossier qui rassemble toutes les fiches d'entraînement proposées par
  le coach (programmes, plannings de séminaire, abaques) — rangées proprement.
- Pas de notes de séance aujourd'hui → créer un système / dossier de notes de
  séance (avec un modèle).
- Créer un dossier pour les vidéos : randoris, techniques, combats — en
  compétition comme à l'entraînement.
- Pas de calendrier utilisé. Evan est sur Mac + iPhone → Apple Calendar (iCloud).
  Veut un calendrier adapté à sa prépa.
```

---

## Q7 — What's the one task that eats your week, and where do you currently track work?

The single biggest time-suck or recurring drudgery. Plus where tasks/projects live (ClickUp / Asana / Linear / Notion / a notebook).

```
Corvées récurrentes qui coûtent le plus de temps :
1. Gérer la nutrition (calculs) pour la descente de poids.
2. Préparer les fiches de séance : calculer les charges à partir des %1RM pour
   chaque séance de musculation.
3. Adapter le programme générique du coach à soi-même (individualisation).

Ce qui NE bouge pas : la planification des créneaux muscu / judo / cardio de la
semaine est déjà établie et fixe :
- Lundi : musculation à partir de 20h00
- Mardi : judo 17h30 – 19h00
- Mercredi : musculation à partir de 15h45
- Jeudi : judo 17h30 – 19h00
- Vendredi : musculation à partir de 16h00
- Dimanche : vélo longue durée (> 1h)
- Samedi : repos
(3 muscu, 2 judo, 1 sortie vélo — voir context/calendar.md)

Suivi des séances à faire : notes personnelles rédigées par Evan lui-même
(ex. la séance du jour est dans ses notes). Pas d'outil de gestion de tâches.
```

---

When this file is filled, run `/onboard` (or re-run it) and the wizard will scaffold your Day-1 file set: `context/`, `references/voice.md`, populated `connections.md`, and a filled `CLAUDE.md`.
