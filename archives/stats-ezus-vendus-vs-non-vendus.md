# Statistiques Ezus étendues — vendus vs non-vendus

Source : scrape API Ezus du 28 avril 2026, **430 dossiers AT/GT** depuis 2025-01-01 :
- **216 convertis** (Payé / Carnet créé / Résa à finaliser / Résa OK / Archivé après vente)
- **214 non convertis** (First Itinerary Creation / Itinerary Validated / Fine Tuning)

Sur les 430 dossiers, **191 ont un montant exploitable** (80 convertis + 111 non convertis). Conversion £ → € à 1.18.

## Insight principal

**Les dossiers convertis et non convertis ont des prix /jour /pers très proches** :
- Convertis : médiane **253 €**, moyenne 280 €, min 125, max 1011
- Non convertis : médiane **262 €**, moyenne 272 €, min 68, max 787

**Le prix n'est PAS le facteur principal de conversion**. Ce sont d'autres dimensions qui font la différence : qualité de l'itinéraire, timing de réponse, suivi commercial, comparaison concurrentielle, adéquation profil/proposition.

## Taux de conversion par segment

### Par taille de groupe — insight très fort

| PAX | Total | Convertis | **Taux** | Médiane convertis | Médiane non convertis |
|---|---|---|---|---|---|
| 1 PAX | 10 | 3 | **30 %** | 429 € | 429 € |
| 2 PAX | 186 | 90 | 48 % | 271 € | 286 € |
| 3-4 PAX | 156 | 84 | 54 % | 229 € | 231 € |
| **5-6 PAX** | 46 | 29 | **63 %** ★ | 238 € | 222 € |
| 7-10 PAX | 28 | 8 | **29 %** | 270 € | 286 € |
| 11+ PAX | 4 | 2 | 50 % | — | — |

**Conclusion** : le **5-6 PAX convertit 2x mieux que le solo et le grand groupe**. Plage qualité/prix optimale.

**Les voyageurs solo et les grands groupes (7+) sont plus difficiles à convertir** : prix /pers élevé pour les solos (les "rentabilités" sont moins bonnes), processus de décision long pour les grands groupes.

### Par saison — surprise faible

| Saison | Total | Convertis | Taux | Médiane convertis € | Médiane non convertis € |
|---|---|---|---|---|---|
| Basse (nov-mars) | 18 | 10 | 56 % | 393 | 262 |
| Haute (juin-août) | 217 | 113 | 52 % | 246 | 247 |
| Mi (avril-mai, sept-oct) | 195 | 93 | 48 % | 258 | 274 |

Les écarts de conversion par saison sont **faibles** (48 à 56 %). La saison n'est pas un grand discriminant.

### Par type de voyage

| Type | Total | Convertis | Taux | Médiane convertis € | Médiane non convertis € |
|---|---|---|---|---|---|
| AT (Autotour) | 383 | 197 | 51 % | 253 | 257 |
| GT (Guided Tour) | 47 | 19 | **40 %** | — | — |

**GT convertit moins** que AT (40 % vs 51 %) — les voyages guidés (plus chers, plus engageants) ont un cycle de vente plus long et plus exigeant.

## Performance par agent — insight stratégique majeur

| Agent | Dossiers travaillés | Convertis | **Taux conversion** | Médiane prix convertis € |
|---|---|---|---|---|
| **Carole Beaumont** | 21 | 18 | **86 %** ★★★ | 242 |
| Marie Limas | 119 | 70 | **59 %** | 262 |
| Alison Spence | 24 | 13 | 54 % | — |
| Angélina Etre | 104 | 52 | 50 % | 295 |
| Nicolas Caisso | 68 | 33 | 49 % | — |
| Johanna Squiban | 24 | 8 | 33 % | 125 |
| **Emily Parnell** | 63 | 16 | **25 %** ⚠ | 211 |
| Anastassia Doubovskaya | 1 | 1 | 100 % | — |
| Jean Depreux (ancien) | 4 | 4 | 100 % | — |

**Lecture** :
- **Carole Beaumont** : meilleur taux à 86 % (mais sur petit volume — à confirmer avec plus de dossiers)
- **Marie Limas** : performance stable et élevée (59 % sur le plus gros volume — 119 dossiers traités)
- **Emily Parnell** : 63 dossiers travaillés mais seulement 25 % convertis = 47 dossiers d'effort sans vente. À investiguer urgence.
- **Johanna Squiban** : 33 % seulement, à creuser également.

### Hypothèses à creuser sur les écarts de performance

1. **Profils traités** : les agents à faible conversion héritent-ils de profils plus difficiles (budgets bas, demandes vagues, GT complexes) ?
2. **Anciennneté** : Marie et Carole ont-elles plus d'expérience ?
3. **Suivi commercial** : intensité et rapidité des relances ?
4. **Spécialisation** : Emily semble avoir beaucoup de profils à budget / pax atypiques

## Plages opérationnelles consolidées (pour qualification client)

Combinant convertis et non-convertis (191 dossiers exploitables) :

| Profil | Plage typique /pers /jour € | /pers /sem € |
|---|---|---|
| **Couple gamme moyenne** (le plus fréquent) | 240-320 | 1 700-2 200 |
| **Couple gamme premium** | 360-500 | 2 500-3 500 |
| **Famille 3-4 PAX gamme moyenne** | 215-260 | 1 500-1 800 |
| **Petit groupe 5-6 PAX** (best conversion!) | 200-240 | 1 400-1 700 |
| **Voyageur solo** | 360-580+ | 2 500-4 000+ |
| **Grand groupe 7+ PAX** | 200-300 | 1 400-2 100 |

### Plancher absolu observé sur dossiers vendus

**125 €/pers/jour** = ~875 €/pers/sem. Aucun dossier vendu en dessous.

### Plancher observé sur non-vendus (souvent indication de projet non viable)

**68 €/pers/jour** = ~476 €/pers/sem. Ces dossiers n'ont pas converti — le projet était sous-évalué dès le départ.

## Top 10 dossiers les plus chers par /pers /jour € (vendus + non vendus)

| Rang | Dossier | Status | PAX | Durée | €/jour/pers |
|---|---|---|---|---|---|
| 1 | AT - Famille Teissier | Vendu | 1 | 14j | **1 011 €** |
| 2 | GT-OussamaElAyoubi | Non vendu (FIC) | 8 | 3j | 787 € |
| 2 | AT - Hélène Tête | Non vendu (FIC) | 1 | 3j | 787 € |
| 4 | GT - Stephane Assael | Vendu | 2 | 9j | 623 € |
| 5 | AT - Nathalie Segard | Non vendu (FIC) | 3 | 6j | 583 € |
| 6 | AT - Bérengère LE TOUMELIN | Vendu | 2 | 7j | 506 € |
| 6 | AT - Jacqueline SOMVILLE | Vendu | 2 | 7j | 506 € |
| 8 | AT - Adeline VOTTE | Non vendu (FIC) | 3 | 3j | 500 € |
| 9 | AT - Christina MALKOUN | Non vendu (FIC) | 2 | 3j | 492 € |
| 10 | AT - Martine Landuyt | Vendu | 2 | 9j | 444 € |

**Pattern** : courts séjours + petits groupes = prix /pers /jour les plus élevés. La durée fait diluer le coût fixe (acheminement, transferts, conception).

## Bottom 10 dossiers (les moins chers /pers /jour €)

| Rang | Dossier | Status | PAX | Durée | €/jour/pers |
|---|---|---|---|---|---|
| 1 | AT - Marie CHION | Non vendu (FIC) | 4 | 11j | **68 €** |
| 2 | AT - Brice BEQUET | Non vendu (FIC) | 3 | 10j | 100 € |
| 3 | AT - Annelore Perez | Non vendu (FIC) | 4 | 22j | 107 € |
| 4 | AT - Erika DI LUZIO | Non vendu (FIC) | 3 | 10j | 110 € |
| 5 | AT - Claire Larcher | Non vendu (FIC) | 3 | 18j | 120 € |
| 6 | AT - Yann LEFETZ | Non vendu (FIC) | 4 | 14j | 125 € |
| 6 | AT - Cécile Bremond | Non vendu (FIC) | 8 | 8j | 125 € |
| 6 | AT - Le Moine | Vendu | 4 | 6j | 125 € |
| 9 | AT - Sara Levy | Vendu→Archivé | 3 | 14j | 140 € |
| 10 | AT - Caterina FARRE | Non vendu (FIC) | 3 | 7j | 143 € |

**Pattern** : 9/10 du bottom 10 sont des **non-vendus**. Confirme que les très petits budgets ne convertissent pas.

## Conclusions opérationnelles pour le système d'apprentissage

### 1. Calibration plancher

**Si un prospect annonce moins de 125 €/pers/jour (875 €/pers/sem), critique constructive obligatoire dès le premier mail.** En dessous de ce seuil, on n'a aucun dossier vendu sur 80.

### 2. Segments à privilégier

- **Familles 5-6 PAX** : 63 % de conversion = pépite à valoriser
- **Familles 3-4 PAX** : 54 %, segment principal
- **Couples 2 PAX** : 48 %, gros volume mais effort à mettre

### 3. Segments à faire évoluer

- **Voyageurs solo** : 30 % de conversion, à améliorer (proposer plus systématiquement les OT 100 % Féminin ?)
- **Grands groupes 7+ PAX** : 29 % seulement — il faudrait analyser pourquoi (process décisionnel ? prix ?)
- **Guided Tours** : 40 % vs 51 % AT — cycle de vente à raccourcir ou à mieux qualifier en amont

### 4. Le prix n'est pas le combat principal

Médianes convertis vs non convertis quasi identiques sur tous les segments. **Ce qui fait la différence** :
- Vitesse de réponse au premier contact
- Adéquation itinéraire / attentes
- Suivi commercial (relances, calls)
- Storytelling visuel de la proposition (insight Family Sales Process Module 2)
- Follow-up post-devis personnalisé (insight Family Sales Process Module 3 : +25 % conversion)

### 5. Performance agents — terrain d'amélioration

**Emily Parnell : 25 % conversion sur 63 dossiers travaillés** = effort de conception sur 47 dossiers sans vente. C'est le poste d'amélioration n°1 de l'agence (gain potentiel : ~15 dossiers vendus si elle alignait sur 50 %).

Action recommandée : audit des dossiers Emily perdus pour identifier le pattern.

## Limites de l'analyse

- **63 % des dossiers (272/430) n'ont pas de `trip_budget` renseigné dans Ezus** → champ utilisé inégalement. Workflow n8n d'alerte à mettre en place.
- **Stats par agent biaisées** par les volumes différents — Carole 21 dossiers vs Marie 119
- **Saisons basse sous-représentées** (18 dossiers seulement)
- **Prix dérivés du `trip_budget`** = estimation initiale et pas forcément le prix réellement vendu (peut différer après ajustements)

## Données brutes

CSV complet (430 dossiers × 15 colonnes) disponible sur demande. Précédent CSV `dossiers-ezus-since-2025.csv` ne contenait que les 216 vendus — à régénérer pour intégrer les non-vendus si besoin.

## Prochaines étapes

1. **Audit Emily Parnell** : identifier les patterns récurrents des 47 non-conversions
2. **Workflow n8n** : alerte aux agents pour systématiser le remplissage de `trip_budget` dans Ezus
3. **Système de tags d'intérêts** (note mémoire en attente) pour matcher prospect ↔ dossiers similaires sur des critères qualitatifs (whisky, randonnée, family-friendly, etc.)
4. **Re-scrape trimestriel** pour suivre l'évolution des taux de conversion

## Source

Scrape API Ezus du 28 avril 2026, 430 dossiers AT/GT depuis 2025-01-01, statuts : Payé / Carnet de voyage créé / Résa à finaliser / Résa OK vérifiées / Archivé / First Itinerary Creation / Itinerary Validated / Fine Tuning. Token JWT à régénérer pour scrape suivant.
