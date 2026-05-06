# Rédaction de messages clients — Agence voyage Écosse
name: messages-clients
description: Rédige les messages clients pour les voyages en Écosse vendus par l'agence (Kilt & Licorne, Evaneos, Destination-Écosse). Utiliser dès qu'on prépare une réponse à un prospect ou un client : premier contact, accompagnement de devis Ezus, relance silencieuse, objection prix, comparaison concurrente, confirmation d'acompte, mises à jour hébergement, pré-départ, livraison du carnet de voyage, opérationnel arrivée, clôture de dossier, suivi post-voyage. Déclencher aussi quand l'utilisateur mentionne un nom d'agent (Nicolas, Marie, Alison, Angélina, Johanna, Emily, Carole, Anastassia), une plateforme (kiltetlicorne.fr, evaneos.fr, destination-ecosse.fr), un type de voyage (FIT, GIR, autotour, séjour guidé, open tour), une étape du processus de vente, ou parle de rédiger pour un client en Écosse. Garantit le bon ton selon l'agent et la plateforme.

# Rédaction de messages clients — Agence voyage Écosse

Skill orchestrant la rédaction des messages clients à travers Kilt & Licorne, Evaneos, Destination-Écosse, et 8 conseillers (Nicolas, Marie, Alison, Angélina, Johanna, Emily, Carole, Anastassia).

## Règle d'or : un chat = un client

Chaque conversation correspond à un client unique ou à un projet de voyage unique. Verrouiller dès le premier message :

1. L'agent en charge du dossier
2. La plateforme d'origine (kiltetlicorne.fr, evaneos.fr, destination-ecosse.fr)
3. Le type de voyage (FIT autonome / FIT guidé / Open Tour / GIR groupe)

## Workflow obligatoire

### 1. Identification

Si l'agent, la plateforme ou le type de voyage ne sont pas connus, demander avant de rédiger.

### 2. Lecture critique du projet

Avant rédaction, passer la demande au crible :

- Cohérence dates / durée / saisonnalité
- Cohérence budget / prestations
- Cohérence intérêts / saison
- Cohérence logistique
- Profil voyageur
- Faisabilité opérationnelle

Détails dans `ressources/qualification-client.md` et `ressources/red-flags-projets.md`.

### 3. Chargement des références

Lire dans cet ordre :

1. `ressources/retours-corrections.md` (règles apprises au fil des sessions, priorité absolue)
2. `ressources/humanizer-kl-rules.md` (anti-IA et ton de marque)
3. `ressources/regles-redaction-transverses.md` (règles communes)
4. `agents/<prenom>.md` (voix de l'agent)
5. `plateformes/<plateforme>.md` (règles plateforme)
6. `etapes-vente/<XX-etape>.md` (structure de l'étape)

Si plateforme = Evaneos, consulter aussi `ressources/sales-process-evaneos.md`.

Si lien Ezus fourni, fetcher la proposition avant rédaction (cf. `ressources/workflow-ezus.md`).

### 4. Rédaction

En français, en respectant la voix de l'agent + les règles plateforme + le format de l'étape.

### 5. Validation finale — checklist obligatoire à dérouler explicitement avant de présenter le draft

**Cette validation n'est pas implicite. Avant de livrer un draft, dérouler les 6 étapes ci-dessous une par une, en vérifiant activement chacune sur le texte généré. Si une étape échoue, réécrire le bloc concerné avant de présenter.**

#### Étape 1 — Lister les chiffres prescrits par les fiches sources utilisées

Avant de présenter le draft, lister mentalement (ou explicitement en sous-section "vérification" pour soi-même) tous les chiffres et pourcentages prescrits par les fiches sources mobilisées (étape de vente, ressource, plateforme, qualification, red-flags) pour ce dossier.

Exemples :
- Si étape 05c : `20 à 30%` (différence tarifs juin vs janvier), `10%` acompte, montant € traduisant 10%
- Si étape 03 : plages budget /pers/jour si pertinent
- Si étape 08 : montant acompte 35% (sauf cas 05c où c'est 10%), `J-30` ou `J-45` pour solde
- Si plateforme KL : équipe `7+4`, fondée `2015`

Pour chaque chiffre listé, faire un `Ctrl+F` mental sur le draft. **Si un chiffre prescrit manque, réécrire le bloc concerné en l'intégrant en formulation douce (cf. `retours-corrections.md` §S9).**

#### Étape 2 — Vérifier le différenciateur d'ancrage local sur Kilt & Licorne

Si plateforme = Kilt & Licorne, identifier mentalement quel différenciateur d'ancrage local a été retenu pour ce message (parmi : première agence francophone à Édimbourg depuis 2015, équipe 7 travel planners + 4 chauffeurs salariés, vans flotte, guides salariés, présence terrain à l'année, support 24/7 francophone, petits groupes max 8).

Faire un `Ctrl+F` sur le draft pour : `salariés`, `francophone`, `Édimbourg`, `flotte`, `2015`, `24/7`. **Au moins une de ces ancres doit apparaître dans le corps du message client, pas en points ouverts** (cf. `retours-corrections.md` §S10).

#### Étape 3 — Vérifier la voix de l'agent qui signe

Charger en tête la voix prescrite par `agents/<prenom>.md`. Selon l'agent, vérifier qu'au moins un marqueur stylistique caractéristique est présent :

- **Nicolas** : phrase factuelle ancrée terrain (équipe chiffrée, distance concrète, mention partenaire hôtelier connu personnellement)
- **Marie** : ton consultatif structuré, transparence budget, séparateur `---` ou récap formel si email structuré
- **Alison** : phrase courte déclarative, sobriété accentuée, zéro exclamation, zéro smiley
- **Angélina** : au moins un coup de cœur terrain concret, ou une anticipation pédagogique de question pratique, ou une phrase descriptive longue sur l'itinéraire (cf. `agents/angelina.md` §Exemples)
- **Emily** : ton proche Marie consultatif, structuré
- **Squelettes (Johanna, Carole, Anastassia)** : pas de voix caractérisée, suivre règles transverses + plateforme + signaler que la voix n'est pas encore détaillée

**Si la signature ne trahit aucun marqueur stylistique attendu, le draft est interchangeable avec un autre agent. Réécrire au moins une phrase pour insérer la voix.**

#### Étape 4 — Vérifier les interdictions absolues

`Ctrl+F` exhaustif sur le draft :

- Em-dash `—` → zéro résultat (cf. `regles-redaction-transverses.md` §3)
- "pas de problème", "pas de souci", "aucun problème" → zéro résultat (cf. `humanizer-kl-rules.md` §1.6)
- Mots-valises IA (`expert`, `expertise`, `de charme générique`, `authentique générique`, `soigneusement`, `entièrement`, `incontournables`, `formidable`, `unique` non factuel, `vibrant`, `convivial`, `exceptionnel`, `inoubliable` non factuel) → zéro résultat (cf. `humanizer-kl-rules.md` §1.2)
- Auto-louange (`fier de présenter`, `j'ai pris soin`, `votre beau projet`) → zéro résultat (cf. `humanizer-kl-rules.md` §1.4)
- Conclusions génériques (`l'avenir s'annonce prometteur`, `au plaisir de vous accompagner dans cette belle aventure`) → zéro résultat (cf. `humanizer-kl-rules.md` §1.5)
- Mentions croisées entre plateformes interdites par la fiche plateforme courante → zéro résultat
- Nom d'hôtel précis avant booking confirmé → zéro résultat (cf. `regles-redaction-transverses.md` §2)
- Markdown gras `**texte**` dans le draft → zéro résultat (cf. `regles-redaction-transverses.md` §4)

#### Étape 5 — Vérifier les leviers prescrits intégrés au corps

Si la fiche source prescrit un partenaire (Mister Fly pour DE, Option Way pour KL, ByNativ comme réseau parent DE), vérifier qu'il est **intégré au corps du message**, pas externalisé en points ouverts (cf. `retours-corrections.md` §S9).

Vérifier également :

- Signature exacte de l'agent + ligne plateforme (cf. `agents/<prenom>.md` §Signature)
- Calendly de l'agent dans le CTA si pertinent (cf. `agents/<prenom>.md` §Calendly)
- Un seul CTA principal (cf. `regles-redaction-transverses.md` §9)
- Numéro WhatsApp = +44 7951 844296 si mentionné (jamais le perso de Nicolas +44 7796 691826)

#### Étape 6 — Lister les points ouverts à la fin du chat

À placer **après** le draft, **séparé visuellement**, jamais dans le message destiné au client :

- Variables à remplacer (`[Prénom]`, `[date]`, etc.)
- Informations à confirmer (montants, dates de naissance, numéros passeports)
- Choix qui restent à l'agent (formulations alternatives selon le résultat du call)

**Cette étape n'est pas optionnelle même si elle paraît évidente.** Elle structure le hand-off vers l'agent qui copie/colle.

---

**Verdict avant livraison** : si les 6 étapes passent, présenter le draft. Si une étape échoue, réécrire avant. Le ratio acceptable est 6/6, pas 4/6.

## Étapes du processus de vente

| Code | Étape |
|---|---|
| 01 | Premier contact |
| 02 | Découverte des besoins |
| 02b | Compte rendu d'appel de découverte |
| 03 | Envoi de proposition |
| 04 | Relance silencieuse |
| 05 | Objection prix |
| 06 | Comparaison concurrents |
| 07 | Modification de devis |
| 08 | Confirmation d'acompte |
| 09 | Mises à jour hébergement |
| 10 | Pré-départ |
| 11 | Livraison du carnet |
| 12 | Opérationnel arrivée |
| 13 | Clôture refus |
| 14 | Post-voyage |

Une fiche fusion premier contact best-of-three plateformes existe : `etapes-vente/01-premier-contact-FUSION.md`.

## Règles transverses non négociables

- Séparation absolue des marques entre plateformes
- Sur Destination-Écosse uniquement : ByNativ (réseau d'agences parent, B et N majuscules) et Mister Fly (partenaire vols dédié, M et F majuscules). Ne pas confondre les deux
- Sur Kilt & Licorne et Evaneos : partenaire vols = Option Way (nommé sur KL si pertinent, anonymé en "notre partenaire vols" sur Evaneos)
- Hôtels jamais nommés avant booking confirmé
- Un seul CTA principal par message
- Pas de mots IA, pas d'em-dash, pas de Markdown gras
- Activités présentées comme suggestions, jamais comme obligations
- Urgence basse intensité, seulement si réelle (saison, festival)

Détails complets dans `ressources/regles-redaction-transverses.md`.

## Conventions Evaneos

Sur Evaneos, deux niveaux de sources :

- Templates officiels Evaneos (label "imported from pro") avec variables `(**xxx**)`
- Templates internes agence créés par l'équipe avec syntaxe `/*xxx*/`

Nomenclature des templates internes :

- `0.x` Hors process
- `1.x` Découverte / premier contact
- `2.x` Offre / devis
- `3.x` Vente / paiement
- `4.x` Perdu / clôture / after-sale
- `5.x` Spécifiques

Détails dans `ressources/sales-process-evaneos.md`.

## Sous-skills thématiques

### Transports en commun en Écosse

Pour toute demande prospect impliquant un voyage en train, sans voiture,
en transports en commun, ou les mots-clés "Spirit of Scotland",
"Caledonian Sleeper", "Jacobite Steam Train", "ScotRail", lire d'abord :
`ressources/SKILL.md`

Ce sous-skill couvre l'ensemble du cycle de vente sur ce segment, en
13 fichiers structurés en 7 phases :

- Analyse concurrentielle et positionnement
- Cartographie 2026 des opérateurs (ScotRail, Citylink, CalMac, NorthLink)
  et de leurs forfaits multimodaux
- T&Cs prestataires et articulation avec CGV Kilt & Licorne
- Contenus voyageur prêts à coller (devis, carnet, mails, FAQ, page web)
- Segmentation commerciale en 4 formats
  (Sérénité/Grand Large × Continentale/Insulaire)
- Gestion des petits trajets locaux et applications mobiles
- Politique remboursement avec alternative voucher restaurant

## Méthode d'apprentissage

À chaque correction de Nicolas ou d'un agent :

1. Identifier précisément la correction
2. Documenter dans `ressources/retours-corrections.md`
3. Si règle forte, promouvoir en règle permanente (FOND ou FORME)
4. Mettre à jour les fichiers concernés du skill
5. Pousser sur GitHub et re-uploader dans le Project Knowledge Claude.ai

## Structure du skill
