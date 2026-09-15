# Connections

Registry of every system your AIOS can reach. Filled by `/onboard` from Q4-Q7 answers; expanded over time as you wire new tools. `/audit` checks this file for domain coverage and freshness.

*Domaines adaptés à un système de préparation sportive personnel (pas une entreprise).*

| # | Domaine | Outil | Mécanisme | Auth | Dernière vérif |
|---|---|---|---|---|---|
| 1 | Résultats & chiffres de perf | Suivi local : `tracking/poids.md`, `tracking/1rm.md` · Compétition : rien de formel | fichiers locaux | — | 2026-09-09 |
| 2 | Interactions coach / club | Facebook Messenger | not yet connected | — | — |
| 3 | Calendrier | Apple Calendar (iCloud, Mac + iPhone) | not yet connected | — | — |
| 4 | Communication | Outlook (mail principal) + Messenger | not yet connected | — | — |
| 5 | Suivi des tâches / séances | Notes personnelles (Apple Notes) | not yet connected | — | — |
| 6 | Intelligence de séance | Notes de séance (`session-notes/`) + vidéos (`videos/`) | fichiers locaux | — | 2026-09-09 |
| 7 | Connaissances / fiches | Fiches du coach (`training-plans/`) + `references/` | fichiers locaux | — | 2026-09-09 |

**Mechanism options:** `mcp` (MCP server), `script` (Python/Bash hitting an API, in `scripts/`), `export` (CSV/JSON dump pipeline), `key+ref` (`.env` key + `references/{tool}-api.md` guide), `not yet connected`.

When you wire a new tool, also save `references/{tool}-api.md` capturing endpoints, auth flow, and common queries — researched-once-saved-forever.
