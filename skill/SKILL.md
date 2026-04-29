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

### 5. Validation finale

- Aucun em-dash `—`
- Aucun balisage Markdown gras `**texte**`
- Aucun mot-valise IA (cf. règles humanizer-kl)
- Aucune mention croisée entre plateformes
- Aucun nom d'hôtel divulgué avant booking
- Signature et Calendly correspondent à l'agent
- Un seul CTA principal
- Lister les points ouverts à la fin du chat

## Étapes du processus de vente

| Code | Étape |
|---|---|
| 01 | Premier contact |
| 02 | Découverte des besoins |
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
- ByNativ nommé uniquement sur Destination-Écosse (B et N majuscules)
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

## Méthode d'apprentissage

À chaque correction de Nicolas ou d'un agent :

1. Identifier précisément la correction
2. Documenter dans `ressources/retours-corrections.md`
3. Si règle forte, promouvoir en règle permanente (FOND ou FORME)
4. Mettre à jour les fichiers concernés du skill
5. Pousser sur GitHub et re-uploader dans le Project Knowledge Claude.ai

## Structure du skill
