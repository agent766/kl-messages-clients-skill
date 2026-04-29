# Skill messages-clients — version complète consolidée

**Note importante** : ce fichier consolide l'intégralité du skill `messages-clients` en un seul document. Le dossier de skill (dans `skills/messages-clients/`) a connu des problèmes de persistance pendant la session du 28 avril 2026, certains fichiers ont disparu et été recréés plusieurs fois. Ce fichier est la copie de référence stable.

Pour redéployer le skill : découper ce fichier selon les sections (séparées par `---FILE: <path>---`) et placer chaque section dans le bon emplacement.

---

# CAPTURÉ EVANEOS — État de l'aspiration du 28 avril 2026

## Portail Partner Connect

`https://travelsuite.evaneos.com/agency-manager/community` — accessible en NC.

5 sections : Live & Replays, Training Modules, Partner Forum, Resources Center, Learning Paths.

### Learning Paths actifs

1. **Learn how to optimize your pricing for better performance** — Pricing dans le sales process
2. **Family Sales Process: Everything you need to know to sell for families!** — adaptation du Sales Process Evaneos générique

### Family Sales Process — structure (8 sections)

1. Discover the Family Sales Process (intro)
2. Live Webinar (passé)
3. Module 1 – 1/2 Mastering Price Sensitivity with Family Travelers (Budget Qualification & Transparency)
4. Module 1 – 2/2 (Closing & Strategic Upselling)
5. Module 2 – 1/2 Designing Family-Centered Proposals (Family Profile & Activities)
6. Module 2 – 2/2 (Visual Impact, Storytelling & Presentation)
7. Module 3 – From Proposal to Yes : Effective Post-Quote Support (Post-Quote Follow-Up and Closing)
8. You're ready to sell to Family with confidence (conclusion)

### Insights chiffrés du Family Sales Process

- **85%** des familles priorisent les activités adaptées à l'âge
- **82%** valorisent une logistique fluide
- Un follow-up rapide et personnalisé booste la conversion **jusqu'à 25%**
- Les courtes vidéos ou messages vocaux personnalisés sont particulièrement efficaces

---FILE: SKILL.md---

```yaml
---
name: messages-clients
description: Rédige les messages clients pour les voyages en Écosse vendus par l'agence (Kilt & Licorne, Evaneos, Destination-Écosse). Utiliser dès qu'on prépare une réponse à un prospect ou un client : premier contact, accompagnement de devis Ezus, relance silencieuse, objection prix, comparaison concurrente, confirmation d'acompte, mises à jour hébergement, pré-départ, livraison du carnet de voyage, opérationnel arrivée, clôture de dossier, suivi post-voyage. Déclencher aussi quand l'utilisateur mentionne un nom d'agent (Nicolas, Marie, Alison, Angélina, Johanna, Emily, Carole, Anastassia), une plateforme (kiltetlicorne.fr, evaneos.fr, destination-ecosse.fr), un type de voyage (FIT, GIR, autotour, séjour guidé, open tour), une étape du processus de vente, ou parle de rédiger pour un client en Écosse. Intègre le sales process officiel Evaneos.
---
```

# Rédaction de messages clients — Agence voyage Écosse

Skill orchestrant la rédaction des messages clients à travers Kilt & Licorne, Evaneos, Destination-Écosse et 8 conseillers (Nicolas, Marie, Alison, Angélina, Johanna, Emily, Carole, Anastassia).

## Règle d'or : un chat = un client

Verrouiller dès le premier message :
1. L'agent
2. La plateforme d'origine
3. Le type de voyage (FIT / GIR, mode)

## Workflow

1. Identification : si éléments manquants, demander
2. Contexte client : étape, profil, faits, historique, lien Ezus
3. Chargement des références (agents/, plateformes/, etapes-vente/, ressources/)
4. Rédaction en français
5. Validation finale (séparation marques, hôtels, signature, CTA, mots IA)

Lister les points ouverts à la fin.

## Étapes du funnel

01 Premier contact / 02 Découverte / 03 Envoi proposition (structure officielle Evaneos 2.1) / 04 Relance silencieuse (structures officielles 2.4 + 2.5) / 05 Objection prix / 06 Comparaison concurrents / 07 Modification devis / 08 Confirmation acompte / 09 MAJ hébergement / 10 Pré-départ / 11 Livraison carnet / 12 Opérationnel arrivée / 13 Clôture refus / 14 Post-voyage

## Règles transverses non négociables

- Séparation absolue des marques entre plateformes
- ByNativ : nommé uniquement sur DE. "Notre partenaire vols" générique toléré sur Evaneos officiel.
- Hôtels : jamais nommés avant booking
- Un seul CTA principal
- Pas de mots IA
- Pas d'emoji Unicode (smileys ASCII tolérés selon agent)
- Activités présentées comme suggestions
- Urgence seulement si réelle

## Conventions Evaneos

Variables officielles : `(**xxx**)`. Variables internes : `/*xxx*/`.

Nomenclature numérique : 0.x Hors process / 1.x Découverte / 2.x Offre / 3.x Vente / 4.x Perdu / 5.x Spécifiques.

---FILE: agents/nicolas.md---

# Nicolas (Nico)

- **Base** : Édimbourg, depuis 2015
- **Rôle** : Conseiller voyage, fondateur de l'agence
- **Plateformes** : Kilt & Licorne (principal), Evaneos (occasionnel), DE
- **Calendly** : `https://calendly.com/nico-caisso/30min`
- **WhatsApp** : `+447796691826` / `https://wa.me/447796691826`

## Voix

Direct, professionnel, expert local. Plus chaleureux et structuré sur Evaneos qu'en interne (cf. template 1.04 capturé). Phrases mixtes courtes/longues. Sobre. Exclamations rares. Pas de tirets longs. Pas d'emoji Unicode.

À privilégier : vocabulaire concret (lieux, distances, durées), présentation factuelle ("installé en Écosse depuis 2015"), différenciateurs précis ("guides salariés", "vans notre flotte"), plages tarifaires concrètes.

À éviter : adjectifs grandiloquents, "inoubliable", auto-louange ("j'ai pris soin", "fier de vous présenter").

## Voix observée (template 1.04)

- Présentation deux temps : nom/base/ancienneté + équipe chiffrée (6 experts + 3 chauffeurs)
- Différenciateurs concrets (guides salariés, vans propres, sans intermédiaires)
- Deux options claires (guide privé vs OT)
- Plage tarifaire transparente (ex : "à partir de 2249€ /pers pour 8 jours")
- Double WhatsApp + Calendly
- Sign-off : "Au plaisir de discuter de votre beau projet de voyage. Bien à vous, Nicolas"

## Signature

Sur KL : `Nicolas\nKilt & Licorne`
Sur Evaneos : `Bien à vous,\nNicolas`

## Pièges

- Ne pas inventer de détails sur les hôtels
- Sur Evaneos, suivre la structure officielle SANS auto-louange
- Pas de cross-promotion entre marques
- Sur Evaneos : jamais ByNativ, mais "notre partenaire vols" OK

---FILE: agents/alison.md---

# Alison

- **Base** : Île de Skye
- **Rôle** : Guide-chauffeur et planificatrice
- **Plateformes** : Evaneos (principal), The Camp Box
- **Calendly** : `https://calendly.com/alison_30min/30min`

## Voix

Chaud, personnel, posé, declaratif. Calme et matter-of-fact. **Phrases courtes** (signature). **Aucun point d'exclamation. Aucun tiret long. Aucun emoji Unicode. Aucun smiley ASCII** (le template officiel Evaneos 2.4 contient `;)`, Alison va plus loin).

## Sur Evaneos

Version plus dépouillée que la norme officielle. Là où 2.1 mettrait "C'est avec plaisir que je vous adresse une première version sur-mesure pour votre beau projet de voyage en Écosse !", Alison écrit "Voici une première version pour votre voyage en Écosse."

## Signature

`Alison`

## Particularités

- **Travail itératif** : envoie en fragments. Claude **garde le contenu en attente** et compile seulement quand demandé
- Relit pour repérer les répétitions de mots
- Préfère les drafts sobres

## Pièges

- Surcharger en exclamations et adjectifs vendeurs
- Insérer emojis ou tirets longs
- Refaire un message déjà construit avant sa demande de compilation
- Coller un template officiel sans corriger les patterns auto-louangeurs

---FILE: agents/marie.md---

# Marie

- **Plateformes** : Destination-Écosse (principal)
- **Voix** : Professionnel, chaleureux, consultatif. Élégant sans théâtralité.
- **Calendly** : `https://calendly.com/desti-ecosse/30min`

Signature :
```
Marie
Destination-Écosse
destination-ecosse.fr
```

Particularités : structure plus formelle pour emails DE, gras toléré sur récap/pré-départ, transparence budget, ByNativ par son nom OK sur DE.

Pièges : ton trop direct, mention KL/Evaneos dans message DE, oubli ByNativ sur DE quand pertinent.

---FILE: agents/emily.md---

# Emily

Conseillère DE. Voix proche de Marie. Baseline Marie à affiner.

Mention ByNativ autorisée (DE uniquement).

Calendly : à confirmer (probable `desti-ecosse/30min`).

Signature :
```
Emily
Destination-Écosse
destination-ecosse.fr
```

---FILE: agents/johanna.md, angelina.md, carole.md, anastassia.md---

Profils vides. À compléter avec `_template.md`. Pour remplir : coller 3-5 messages réels et demander à Claude d'en dériver le profil.

---FILE: agents/_template.md---

```
# [Prénom]

## Identité
- Base / Rôle / Plateformes / Spécialité / Langues

## Voix
- Ton, registre, longueur, ponctuation
- Mots à privilégier / éviter

## Signature
[Bloc exact]

## Calendly
[lien]

## Particularités de workflow

## Pièges connus
```

---FILE: plateformes/evaneos.md---

# Plateforme : Evaneos

L'agence est **agent local Évanéos**. Sobre, personnel, sans cross-promotion.

## Agents : Alison (principal), Nicolas (occasionnel sur GT/OT)

## Ton (référence Alison)

Chaud, personnel, sobre, declaratif. Calme. Phrases courtes. Aucune emphase artificielle.

Note : Nicolas sur Evaneos est plus structuré (cf. 1.04).

## Mentions autorisées

- Expertise locale
- Équipe (par prénom)
- The Camp Box (entité juridique sur Evaneos)
- "Notre partenaire (vols)" en générique — sans nommer ByNativ

## Mentions interdites

- Kilt & Licorne (jamais)
- Destination-Écosse (jamais)
- ByNativ par son nom (réservé à DE)

## Format — règles strictes

- Aucun emoji Unicode
- Aucun tiret long
- Un seul CTA principal
- Signature courte

## Format — règles modulables (révisées après aspiration officielle)

- **Bullets** : tolérés pour listes administratives (next steps, jalons paiement). Le template 2.1 les utilise.
- **Smileys ASCII** (`;)`) : 2.4 en contient. Tolérés selon agent. **Interdits pour Alison**.
- **Exclamations** : très rares. **0 pour Alison**. Max 1 dans les autres voix.
- **Gras de section** : sur emails très structurés.

## Variables Evaneos officielles

```
(**prénom ou nom du voyageur**)
(**votre destination**)
(**date du voyage**)
(**lien vers la proposition**)
(**indiquer une date et une heure**)
(**court message personnalisé**)
```

À distinguer de `/*xxx*/` (interne agence).

## Sign-offs Evaneos officiels

- "Au plaisir de vous parler prochainement,"
- "Bien à vous,"
- "Merci pour votre aide," (en break-up)
- "Je vous remercie et vous souhaite une excellente journée,"

## Multi-canal mentionné

Légitimé par 2.5. Citer les canaux déjà tentés (mail + appel + WhatsApp) renforce la légitimité.

---FILE: plateformes/kiltetlicorne.md---

# Plateforme : Kilt & Licorne

Marque historique. Voix la plus libre.

Agents : Nicolas (principal).

Ton : Direct, professionnel, expert local. Ancré dans le terrain. Expertise prouvée par le contenu.

Mentions autorisées : équipe Édimbourg + Skye, véhicules et guides salariés (différenciateur), petits groupes (max 8 OT), sur-mesure, support 24/7 français.

Mentions interdites : Evaneos, DE, ByNativ.

Format : Pas de bullets en routine. Pas de gras systématique. Un CTA. Signature : prénom + ligne plateforme.

```
Nicolas
Kilt & Licorne
```

---FILE: plateformes/destination-ecosse.md---

# Plateforme : Destination-Écosse

Plus consultatif et premium que KL. **ByNativ par son nom** uniquement ici.

Agents : Marie (principale), Emily.

Ton : Professionnel, chaleureux, consultatif. Élégant sans théâtralité.

Mentions autorisées : ByNativ par son nom, expertise francophone sur place, accompagnement bout en bout.

Mentions interdites : KL, Evaneos.

Format : gras de section toléré sur emails structurés, bullets tolérés ponctuellement, signature complète.

```
Marie
Destination-Écosse
destination-ecosse.fr
```

---FILE: etapes-vente/03-envoi-proposition.md---

# Étape 03 — Envoi de la proposition

## Pré-requis

**Fetcher le lien Ezus** avant rédaction.

## Structure officielle Evaneos (template 2.1)

1. Salutation + variable client
2. Phrase d'ouverture engageante mentionnant le projet de voyage
3. Annonce du programme : nuits + date départ
4. **Trois sections explicatives** : choix des étapes / hébergements / transports
5. Lien Ezus
6. Mention partenaire vols si pertinent
7. **Next steps administratives en bullets** : formulaire, IDs participants, lien acompte XX%
8. Engagement sur un rappel téléphonique daté
9. Sign-off : "Au plaisir de vous parler prochainement,"

15-25 lignes.

## Variations plateforme

- KL : marge pour opinion d'expert, structure plus libre
- Evaneos : suit la structure officielle 2.1, sobre, norme Alison plus dépouillée
- DE : structure plus formelle, ByNativ par son nom si vols inclus

## Cadres récurrents

- **Logique de rayonnement** : si plusieurs nuits sur une base + exploration autour
- **Activités = suggestions**, jamais obligations

## Pièges du template officiel à corriger

- "fièr(e) de vous présenter" : auto-louange
- "j'ai pris soin et passé du temps" : auto-louangeur
- "votre beau projet de voyage" : générique
- 3 `(**Expliquer...**)` mal remplis = message creux

## Notes

- Sur Evaneos : jamais ByNativ par son nom
- Bullets pour next steps : OK (validé par 2.1)
- Message vocal court / vidéo avec devis : booste conversion +25% (Family Sales Process Module 3)

---FILE: etapes-vente/04-relance-silence.md---

# Étape 04 — Relance silencieuse

- Relance n°1 : J+5 à J+10
- Relance n°2 : J+10 à J+15
- Break-up email : J+15 à J+30

## Structure officielle — Relance n°1 (2.4)

1. Salutation + variable client
2. Phrase d'accroche personnalisée courte
3. Tentative téléphone factuelle
4. Question de réception du mail
5. Disponibilité pour échanger
6. **Réassurance sociale** : avis clients, blog, presse
7. Demande de créneaux horaires
8. Sign-off

8-15 lignes.

## Structure officielle — Break-up (2.5)

1. Reprise factuelle des canaux déjà tentés
2. Annonce du contexte de clôture (factuel, pas menace)
3. Empathie sur raisons probables (très occupé OU plus intéressé)
4. **Question fermée** : permission de clôturer
5. **Question ouverte alternative** : "que recommanderiez-vous comme prochaine étape ?"
6. Sign-off court : "Merci pour votre aide,"

5-8 lignes.

## Pièges du template officiel à corriger

- "Comment allez-vous ?" : ouverture creuse
- `;)` à éviter sur Alison
- "nos chers clients" : daté
- "complètement convaincu(e)" : présume

## Multi-canal mentionné

Légitimé par 2.5. Citer les canaux déjà tentés.

---FILE: etapes-vente/01-premier-contact.md, 02-decouverte-besoins.md, 05 à 14---

Voir contenus structurés dans le repo. Étapes secondaires couvrent le funnel complet (premier contact, découverte besoins, objection prix, comparaison concurrents, modification devis, confirmation acompte, MAJ hébergement, pré-départ, livraison carnet, opérationnel arrivée, clôture refus, post-voyage).

Chaque fiche contient : Quand, Objectif, Structure, Variations plateforme, Pièges, Référence Evaneos.

---FILE: ressources/regles-redaction-transverses.md---

## 1. Séparation absolue des marques

| Plateforme | Mentions interdites |
|---|---|
| KL | Evaneos, DE, ByNativ |
| Evaneos | KL, DE, ByNativ par son nom |
| DE | KL, Evaneos |

ByNativ : nommé uniquement sur DE. "Notre partenaire vols" générique toléré sur Evaneos officiel.

## 2. Hôtels jamais nommés avant booking

## 3. Pas de mots IA

À éviter : "il est important de noter", "en conclusion", "fascinant", "crucial", "magique", "inoubliable", "j'ai pris soin", "fière de vous présenter".

## 4. Bullets — règle nuancée

Tolérés pour listes administratives (next steps après devis, jalons paiement, check-list pré-départ). Validé par template officiel 2.1.

## 5. Gras de section — règle nuancée

Sur emails très structurés (récap final, confirmation acompte, pré-départ DE).

## 6. Un seul CTA principal par message

## 7. Apologies parcimonieuses

## 8. Activités = suggestions

## 9. Urgence : seulement si réelle

## 10. Variété syntaxique

## 11. Ponctuation par plateforme

| Plateforme | Exclamations | Tirets longs | Emojis Unicode | Smileys ASCII |
|---|---|---|---|---|
| KL | Très rares | Évités | Non | Tolérés selon agent |
| Evaneos | Rares (max 1, 0 pour Alison) | Aucun | Non | Tolérés sauf Alison |
| DE | Rares | Tolérés | Non | Non en routine |

## 12. Conventions Evaneos

Variables officielles : `(**xxx**)`. Variables agence : `/*xxx*/`.

## 13. Multi-canal mentionné dans les relances

## 14. Toujours signer

## 15. Lister les points ouverts

---FILE: ressources/sales-process-evaneos.md---

# Sales Process Evaneos — référence officielle

Aspiration faite le 28 avril 2026.

## Trois piliers

1. SENSIBILITÉ PRIX (Budget Qualification & Transparency / Closing & Strategic Upselling)
2. CONCEPTION DE LA PROPOSITION (Profil & activités / Storytelling visuel)
3. SUIVI POST-DEVIS (Follow-Up & Closing)

## Nomenclature

| Code | Famille |
|---|---|
| 0.x | Hors process |
| 1.x | Découverte / premier contact |
| 2.x | Offre / devis |
| 3.x | Vente / paiement |
| 4.x | Perdu / clôture / after-sale |
| 5.x | Spécifiques (solo OT) |

## Templates capturés (voir `templates-bruts/evaneos/`)

- 1.04 Demandes séjour accompagnés GT - OT ? (Nicolas, agence)
- 2.1 Offre - Envoi du 1er devis (officiel)
- 2.4 Offre - Relance voyageur n°1 (officiel)
- 2.5 Offre - Break-up email (officiel)

## À capturer

Officiels : 1.1, 1.2, 1.3, 1.4, 1.6, 1.7, 1.8, 2.2, 2.3, 3.1, 3.2, 3.3, 4.1, 4.2, 4.3.

Internes : 1.1.5.5 Familles, 1.1.7 OT Lassies, 1.25 Famille sans budget, 1.9 OT 8 jours, 3.1.1 Acompte.

## Family Sales Process

### Module 1 — Mastering Price Sensitivity

Insight : familles avec budget strict. Reconnaître + respecter = confiance.

### Module 2 — Designing Family-Centered Proposals

Insight : 85% priorisent activités adaptées à l'âge, 82% valorisent logistique fluide.

### Module 3 — From Proposal to Yes

Insight : +25% conversion avec follow-up rapide. Vidéos courtes / messages vocaux efficaces.

---FILE: templates-bruts/evaneos/1-04-demandes-sejour-accompagnes-GT-OT.md (Nicolas, agence)---

```
Bonjour /*Nom du client*/,

Je suis ravi de recevoir votre projet de voyage en Écosse, qu'Evaneos nous a transmis.

Je m'appelle Nicolas, installé en Écosse depuis 2015 et je suis le créateur de la première agence basée à Édimbourg et spécialisée dans le voyage sur mesure pour les voyageurs francophones.
Notre équipe est composée de 6 experts/travels planners et 3 chauffeurs/guides, toutes et tous passionnés de l'Écosse pour vous proposer la meilleure expérience de voyage.

C'est un plaisir de vous faire partager notre expertise d'agence locale pour vous organiser un voyage sur-mesure inoubliable.
Les avantages de notre agence : Nos guides-chauffeurs sont salariés, nos vans notre flotte. Résultat ?
Une qualité constante, au meilleur prix, sans intermédiaires.

Concernant votre projet de voyage accompagné en Écosse, nous avons 2 offres de services à vous proposer :

Notre service de guide/chauffeur français privé, où l'itinéraire est conçu suivant vos attentes et où vous avez l'exclusivité du service guide/chauffeur + véhicule.
C'est notre service le plus exclusif et qui vous apportera l'expérience voyage la plus authentique et personnalisée grâce à notre expertise du pays.
Au niveau du tarif, en fonction des logements nécessaires et de la composition de votre groupe, il faudrait compter sur environ xxxx/jour incluant donc la prestation guide/chauffeur véhiculé et les hébergements.

La seconde option, serait que vous preniez part à un de nos séjours organisés en petits groupes (8 personnes max).
Cette offre présente le meilleur qualité/prix d'expérience voyage car vous diviser le coût de la prestation guide/chauffeur à plusieurs.
Les dates sont fixes et les hébergements sont déjà réservés pour garantir la bonne disponibilité et le prix du séjour.
Comptez sur un tarif à partir de 2249€ /pers pour 8 jours / 7nuits

Nous pourrions échanger par téléphone afin que je puisse cerner vos attentes et vous proposer les meilleures dates.

Je suis disponible afin d'échanger au sujet de projet par téléphone au +447796691826 (https://wa.me/447796691826) ou vous pouvez réserver un créneau sur mon calendrier afin que nous puissions organiser un échange téléphonique.
https://calendly.com/nico-caisso/30min

Au plaisir de discuter de votre beau projet de voyage.
Bien à vous,
Nicolas
```

---FILE: templates-bruts/evaneos/2-1-offre-envoi-1er-devis-OFFICIEL.md (officiel Evaneos)---

```
Bonjour (**prénom ou nom du voyageur**),

C'est avec plaisir que je vous adresse une première version sur-mesure pour votre beau projet de voyage en/au (**votre destination**)! Je suis fièr(e) aujourd'hui de vous présenter le résultat de mon travail.

Afin de répondre au mieux à vos envies, et tel que discuté, veuillez trouver ci-joint le programme que je vous recommande sur une base de XX nuits avec un départ le (**date du voyage**).

Comme discuté par téléphone, j'ai pris soin et passé du temps à sélectionner les prestations qui j'espère correspondent le mieux à vos attentes :
(**Expliquer brièvement le choix des étapes, mettre en avant les points forts du parcours**)
(**Expliquer le choix des hébergements, mettre en avant les points forts (emplacement, adapté aux familles, aux couples etc.) en fonction des attentes du voyageur.**)
(**Expliquer le choix des transports**)
(**OPTIONNEL : n'hésitez pas dès maintenant votre sélection personnalisée en cliquant ici :**)
(**lien vers la proposition**)

Si vous faites le choix d'acheter vos vols chez notre partenaire, je serai informé(e) automatiquement de vos vols et de tout changement éventuel afin de prendre immédiatement les dispositions nécessaires au bon déroulement de votre voyage.

Après notre prochain appel, je pourrais vous envoyer une version finalisée de votre programme. Si elle vous convient, les prochaines étapes seront :
- me renvoyer renseigné le formulaire d'inscription ci-joint
- envoi du nom et prénom des participants ainsi que leur dates de naissance
- un lien de paiement vous sera ensuite envoyé pour régler un acompte de XX%. Les réservations seront effectuées dès que l'acompte sera réglé.
- après le paiement de l'acompte, je pourrais bloquer vos prestations !

Comme convenu, je vous rappelle le (**indiquer une date et une heure**), afin de recueillir votre avis sur cette proposition.

Au plaisir de vous parler prochainement,
```

---FILE: templates-bruts/evaneos/2-4-offre-relance-voyageur-n1-OFFICIEL.md (officiel Evaneos)---

```
Bonjour (**prénom ou nom du voyageur**),

Comment allez-vous? Ici… (**court message personnalisé**)

J'ai essayé de vous contacter par téléphone mais je n'ai pas réussi à vous joindre.

Je vous ai envoyé votre proposition par e-mail. L'avez-vous bien reçue?

Je serais heureux(se) de faire un point avec vous pour discuter de ce programme, n'hésitez donc pas à m'envoyer un mail ou à me donner vos disponibilités, si vous aviez des questions ou un autre changement à faire, pour être complètement convaincu(e) par notre offre de voyage.

Pour en savoir un peu plus sur notre agence et voir pourquoi les voyageurs et Evaneos nous font confiance, je vous invite à consulter les avis de nos chers clients, peut-être serez-vous le prochain à nous raconter vos vacances en XX ;)
Cliquez ici : (**lien vers du contenu inspirant : vidéos, blogs, photos, articles de presse etc...**)

Avec le décalage, je suis disponible du lundi au vendredi entre XXh et XXh de France, avez-vous du temps libre dans ce créneau pour que je vous appelle?

Je vous remercie et vous souhaite une excellente journée,

Bien à vous,
```

---FILE: templates-bruts/evaneos/2-5-offre-break-up-email-OFFICIEL.md (officiel Evaneos)---

```
Bonjour (**prénom ou nom du voyageur**),

Je vous écris suite à mon précédent mail et au message vocal que je vous ai envoyé,

Nous sommes à l'étape de clôture des dossiers encore ouverts de ce mois-ci.

En général, quand je n'ai plus de nouvelles d'un voyageur à ce stade, c'est soit qu'il est très occupé, soit qu'il n'est plus intéressé.

Si vous n'êtes plus intéressé, est-ce que j'ai votre permission pour clôturer votre dossier ?

Si vous êtes encore partants, que recommanderiez-vous comme prochaine étape ?

Merci pour votre aide,
```

---

# ANALYSE CRITIQUE DES TEMPLATES EVANEOS

## Forces du système Evaneos

- Nomenclature claire (0.x → 5.x)
- Variables documentées `(**xxx**)`
- Multi-canal intégré (mail + tel + WhatsApp)
- Structure break-up reconnue
- Templates couvrent toute la chaîne
- Profils différenciés (décidés/indécis, familles, solo)

## Faiblesses

- Tonalité datée ("ravi de recevoir", "nos chers clients", "Comment allez-vous ?")
- Auto-louange dans 2.1 ("fièr(e)", "j'ai pris soin")
- Adjectifs amplificateurs ("beau projet", "inoubliable")
- Variables très demandantes (3 placeholders dans 2.1)
- Smileys ASCII dans 2.4
- Tournures inclusives forcées
- Sign-offs hétérogènes

## Patterns Evaneos officiels qui contredisent les règles initiales

| Règle skill v1 | Réalité Evaneos | Action |
|---|---|---|
| Pas de bullets sur Evaneos | 2.1 utilise des bullets pour next steps | Bullets autorisés pour listes admin |
| Pas d'emoji | 2.4 contient `;)` | Smileys ASCII tolérés selon agent |
| Variables `/*nom*/` | Officiel utilise `(**nom**)` | Documenter les deux conventions |
| ByNativ = DE | 2.1 mentionne "notre partenaire" | Sur Evaneos, "notre partenaire" générique OK |

## Recommandations appliquées au skill

1. `agents/nicolas.md` : voix réelle Evaneos
2. `plateformes/evaneos.md` : règles nuancées (bullets/smileys), conventions officielles
3. `etapes-vente/03-envoi-proposition.md` : structure officielle 2.1
4. `etapes-vente/04-relance-silence.md` : structures officielles 2.4 et 2.5
5. `ressources/regles-redaction-transverses.md` : règles nuancées
6. `ressources/sales-process-evaneos.md` : NOUVEAU (référence officielle)

---

# LIENS UTILES

## Calendly par agent

| Agent | Lien |
|---|---|
| Nicolas | `https://calendly.com/nico-caisso/30min` |
| Alison | `https://calendly.com/alison_30min/30min` |
| Marie | `https://calendly.com/desti-ecosse/30min` |
| Emily, Johanna, Angélina, Carole, Anastassia | À confirmer |

## WhatsApp

- Nicolas : `+447796691826` / `https://wa.me/447796691826`

## ETA UK (toutes plateformes)

`https://www.akissfromuk.com/post/eta-uk-guide-pas-a-pas`

## ByNativ — uniquement sur DE

## Autres

- Ezus : `https://pages.ezus.io/thecampbox/[client-folder]/index.html` (espaces : `%20`)
- CalMac : `https://www.calmac.co.uk` (Mallaig–Armadale pour Skye)
- Historic Environment Scotland : `https://www.historicenvironment.scot`
- Walkhighlands : `https://www.walkhighlands.co.uk`

## Portails Evaneos

- Partner Connect : `https://travelsuite.evaneos.com/agency-manager/community`
- Message Templates : `https://travelsuite.evaneos.com/request-manager/templates/list`

---

# WORKFLOW EZUS

Format URL : `https://pages.ezus.io/thecampbox/[client-folder]/index.html` (espaces `%20`).

Fetcher systématiquement avant rédaction des étapes 03, 07, 09, 10, 11.

Quoi extraire :
- Logique itinéraire (rayonnement vs étapes A→B)
- Bases de séjour, durée, expériences fortes
- Mode de voyage
- Catégorie d'hébergement (sans noms)
- Prix, inclusions

**Règle absolue** : ne pas citer les noms d'hôtels avant booking, même si présents dans Ezus.

---

# GLOSSAIRE FIT / GIR

- **FIT** : voyageur individuel ou petit groupe (couple, famille). Sur-mesure pour ce groupe seul.
  - **FIT autonome** : autotour, client conduit
  - **FIT avec accompagnement ponctuel** : autonomie + guide certaines journées
  - **FIT entièrement guidé** : guide-chauffeur salarié
- **GIR** : groupe constitué (CE, association, incentive). Décideur souvent non voyageur.
- **Open Tour** : dates fixes, voyageurs ne se connaissent pas, max 8 participants.
- **Rayonnement** : plusieurs nuits sur une base, exploration autour.
- **Étape A→B** : chaque nuit dans un lieu différent.
- **CalMac** : Caledonian MacBrayne, ferries écossais.
- **Explorer Pass** : Historic Environment Scotland, châteaux.
- **ETA UK** : visa électronique obligatoire.

## Profils Evaneos

Notation 1-5 étoiles dans les templates Evaneos :
- 1-2*** : voyageurs indécis, en exploration
- 3-5*** : voyageurs décidés, demande précise

---

# FIN DU FICHIER CONSOLIDÉ
