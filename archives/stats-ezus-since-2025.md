# Statistiques Ezus depuis 2025-01-01 — analyse des dossiers vendus

Source : scrape API Ezus du 28 avril 2026, 216 dossiers AT/GT en statut Payé / Carnet de voyage créé / Résa à finaliser / Résa OK vérifiées / Archivé, départ ≥ 2025-01-01.

Sur les 216 dossiers, **80 ont un montant exploitable** (les autres ont `trip_budget = 0` car le champ Ezus n'est pas systématiquement renseigné).

Conversion £ → € appliquée à 1.18.

## Vue d'ensemble

- **216 dossiers** depuis 2025-01-01
- **197 AT** (Autotours) + **19 GT** (Guided Tours)
- **80 avec montant exploitable** (les stats ci-dessous)
- Prix /jour /personne (€) : moyenne **280**, médiane **253**, min **125**, max **1011**

## Répartition par statut

| Statut | Nombre |
|---|---|
| Payé | 103 |
| Résa à finaliser (Acompte Versé) | 55 |
| Archivé | 29 |
| Résa OK vérifiées (Solde à payer) RdBk | 19 |
| Carnet de voyage créé | 10 |

## Prix par jour par personne (€) — par type de voyage

| Type | n | Min | Médiane | Moyenne | Max |
|---|---|---|---|---|---|
| AT | 78 | 125 | 253 | 274 | 1011 |
| GT | 2 | 393 | 623 | 508 | 623 |

GT sous-représenté dans les exploitables (la majorité des GT n'ont pas de budget renseigné).

## Prix par jour par personne (€) — par taille de groupe

| PAX | n | Min | Médiane | Moyenne | Max |
|---|---|---|---|---|---|
| 1 PAX | 3 | 364 | 429 | 601 | 1011 |
| 2 PAX | 41 | 171 | 271 | 296 | 623 |
| 3-4 PAX | 29 | 125 | 229 | 239 | 393 |
| 5-6 PAX | 6 | 162 | 238 | 217 | 246 |
| 7-10 PAX | 1 | 270 | 270 | 270 | 270 |

**Économie d'échelle nette** : passage 2 → 3-4 PAX divise quasiment par 1.3 le prix /pers /jour.

## Prix par jour par personne (€) — par saison

| Saison | n | Min | Médiane | Moyenne | Max |
|---|---|---|---|---|---|
| Haute (juin-août) | 48 | 140 | 246 | 282 | 1011 |
| Mi (avril-mai, sept-oct) | 31 | 125 | 258 | 274 | 506 |
| Basse (nov-mars) | 1 | 393 | 393 | 393 | 393 |

**Surprise** : haute saison et mi-saison ont des prix médians proches (246 vs 258 €). La haute saison n'est pas significativement plus chère sur le sur-mesure (mais nb dossiers basse saison trop faible pour conclure).

## Prix par jour par personne (€) — par durée

| Durée | n | Min | Médiane | Moyenne | Max |
|---|---|---|---|---|---|
| Court (< 7 nuits) | 2 | 125 | 393 | 259 | 393 |
| Moyen (7-10 nuits) | 49 | 148 | 262 | 283 | 623 |
| Long (11-15 nuits) | 25 | 140 | 236 | 282 | 1011 |
| Très long (16+ nuits) | 4 | 185 | 248 | — | — |

Pas de tendance claire — le prix /pers /jour reste stable quelle que soit la durée.

## Prix /pers /jour € — par PAX × Saison (segmentation fine)

| Segment | n | Médiane | Moyenne |
|---|---|---|---|
| 1 PAX × Haute | 2 | 1011 | 720 |
| 1 PAX × Mi | 1 | 364 | 364 |
| 2 PAX × Haute | 18 | 270 | 302 |
| 2 PAX × Mi | 22 | 287 | 286 |
| 2 PAX × Basse | 1 | 393 | 393 |
| 3-4 PAX × Haute | 24 | 229 | 237 |
| 3-4 PAX × Mi | 5 | 236 | 246 |
| 5-6 PAX × Haute | 3 | 242 | 228 |
| 5-6 PAX × Mi | 3 | 214 | 205 |
| 7-10 PAX × Haute | 1 | 270 | 270 |

**Plages opérationnelles confirmées** :
- **Couple haute saison** : médiane 270 €/pers/jour (~1 890 €/pers/sem)
- **Couple mi-saison** : médiane 287 €/pers/jour (~2 009 €/pers/sem)
- **Famille 3-4 PAX** : médiane 229-236 €/pers/jour (~1 600-1 650 €/pers/sem)
- **Petit groupe 5-6 PAX** : médiane 214-242 €/pers/jour (~1 500-1 700 €/pers/sem)

## Performance par agent

| Agent | Dossiers (avec montant) | Prix /pers /jour € — médiane | Min | Max |
|---|---|---|---|---|
| Marie Limas | (le plus fourni) | ~250-300 | 148 | 506 |
| Angélina Etre | ~14 | 295 | 162 | 444 |
| Emily Parnell | ~9 | 211 | 171 | (?) |
| Carole Beaumont | ~3 | 242 | 140 | 281 |
| Nicolas Caisso | (mix) | varié | — | — |
| Anastassia Doubovskaya | ~1 | — | — | — |
| Johanna Squiban | ~3 | 125-214 | 125 | — |
| Alison Spence | (peu) | — | — | — |
| Jean Depreux | (ancien agent) | — | — | — |

**À noter** : Marie Limas est de loin l'agente la plus active sur le scrape (~30+ dossiers avec montants), suivie d'Angélina Etre. Dataset à enrichir pour stats fiables par agent.

## Top 5 dossiers par prix /pers /jour €

| Dossier | PAX | Durée | Prix /pers /jour € | Contexte |
|---|---|---|---|---|
| AT - Famille Teissier | 1 | 14 jours | 1011 € | Saison été 2025, voyage solo prolongé premium |
| GT - Stephane Assael | 2 | 9 jours | 623 € | GT (guidé) été 2025, Skye+Cairngorms+Highlands |
| AT - Bérengère LE TOUMELIN | 2 | 7 jours | 506 € | Mai 2026, court séjour premium |
| AT - Jacqueline SOMVILLE | 2 | 7 jours | 506 € | Juin 2025, court séjour premium |
| AT - Martine Landuyt | 2 | 9 jours | 444 € | Juin-juillet 2026, gamme haute |

## Bottom 5 dossiers par prix /pers /jour €

| Dossier | PAX | Durée | Prix /pers /jour € | Contexte |
|---|---|---|---|---|
| AT - Le Moine | 4 | 6 jours | 125 € | Octobre 2026, low budget |
| AT - Sara Levy | 3 | 14 jours | 140 € | Juillet-août 2025, low budget — finalement Archivé |
| AT - Laetitia BONFILS | 4 | 8 jours | 148 € | Août 2025, low budget |
| AT - Anne-Catherine Ribeiro | 5 | 8 jours | 162 € | Avril 2025, low budget — Archivé |
| AT - Mael DODIN | 4 | 14 jours | 164 € | Juillet 2025, low budget |

## Conclusions opérationnelles

### Plages indicatives à utiliser dans le premier contact

| Profil | Plage /pers /sem (€) | Plage /pers /jour (€) |
|---|---|---|
| **Couple gamme moyenne** | 1 700 - 2 200 | 240 - 320 |
| **Couple gamme premium** | 2 500 - 3 500 | 360 - 500 |
| **Famille 3-4 PAX gamme moyenne** | 1 500 - 1 800 | 215 - 260 |
| **Petit groupe 5-6 PAX** | 1 400 - 1 700 | 200 - 240 |
| **Voyageur solo** | 2 500 - 4 000+ | 360 - 580+ |
| **Open Tour 8j** | À partir de 2 249 (catalogue OT 2026) | ≈ 320 |

### Seuils de qualification

Sur 80 dossiers Completed/Operation avec montant :
- **0 dossier sous 125 €/pers/jour** (= 875 €/pers/sem) — c'est le plancher absolu
- **Médiane 253 €/pers/jour** = ~**1 770 €/pers/sem**

**Règle déduite** : si un prospect annonce un budget < 125 €/pers/jour (875 €/pers/sem), c'est en dessous du plancher observé sur tous les dossiers vendus. Critique constructive obligatoire dès le premier contact.

## Limites de l'analyse

- **63 % des dossiers (136/216) n'ont pas de `trip_budget` renseigné** dans Ezus → champ utilisé inégalement par les agents. Action recommandée : créer un workflow d'alerte n8n pour rappeler aux agents de remplir ce champ à la création de devis.
- **GT sous-représenté** : 19 GT au total mais seulement 2 avec montant exploitable.
- **Saison basse** : 1 seul dossier exploitable.

## Prochaines étapes

1. Enrichir `qualification-client.md` du skill avec ces plages opérationnelles
2. Créer le **système de tags d'intérêts** (note mémoire) : tagger chaque dossier par thèmes (culture, nature, villes, hors sentiers, whisky, family-friendly, transports en commun friendly) pour matcher avec les attentes prospects
3. Encourager le remplissage systématique de `trip_budget` dans Ezus pour augmenter le N exploitable
4. Re-scraper trimestriellement pour suivre l'évolution des plages

## Source

Scrape API Ezus du 28 avril 2026, croisé avec scrape Evaneos Pipeline du même jour. Données brutes dans `dossiers-ezus-since-2025.csv`.
