# Sales Process Evaneos — référence officielle

À consulter dès qu'on rédige un message sur Evaneos, pour rester aligné sur le cadre officiel de la marketplace.

Source : aspiration du portail Partner Connect Evaneos faite le 28 avril 2026.

---

## Trois piliers du sales process Evaneos

| Pilier | Focus |
|---|---|
| 1. Sensibilité prix | Budget Qualification & Transparency, Closing & Strategic Upselling |
| 2. Conception de la proposition | Profil voyageur & activités, Storytelling visuel |
| 3. Suivi post-devis | Follow-Up & Closing, multi-canal |

---

## Nomenclature des templates

| Code | Famille |
|---|---|
| 0.x | Hors process |
| 1.x | Découverte / premier contact |
| 2.x | Offre / devis |
| 3.x | Vente / paiement |
| 4.x | Perdu / clôture / after-sale |
| 5.x | Spécifiques (solo OT, etc.) |

### Templates capturés à ce jour

| Code | Titre | Source |
|---|---|---|
| 1.04 | Demandes séjour accompagnés GT - OT ? | Interne agence (Nicolas) |
| 2.1 | Offre - Envoi du 1er devis | Officiel Evaneos |
| 2.4 | Offre - Relance voyageur n°1 | Officiel Evaneos |
| 2.5 | Offre - Break-up email | Officiel Evaneos |

### Templates à capturer (priorité sessions futures)

Officiels : 1.1, 1.2, 1.3, 1.4, 1.6, 1.7, 1.8, 2.2, 2.3, 3.1, 3.2, 3.3, 4.1, 4.2, 4.3.

Internes : 1.1.5.5 Familles, 1.1.7 OT Lassies, 1.25 Famille sans budget, 1.9 OT 8 jours, 3.1.1 Acompte.

---

## Family Sales Process — modules

### Module 1 — Mastering Price Sensitivity

Insight : familles avec budget strict. Reconnaître la contrainte + la respecter ouvertement = créer la confiance.

Application : poser le budget tôt dans le premier message, sans fausse pudeur (cf. `humanizer-kl-rules.md` et `regles-redaction-transverses.md` §17).

### Module 2 — Designing Family-Centered Proposals

Insights statistiques (Evaneos) :

- 85% des familles priorisent les activités adaptées à l'âge des enfants
- 82% valorisent une logistique fluide (étapes, temps de route, hébergements proches)

Application : dans la proposition, mettre en avant explicitement les activités enfants et la logistique simplifiée.

### Module 3 — From Proposal to Yes

Insight : un follow-up rapide post-envoi du devis booste la conversion de **+25%**. Les vidéos courtes ou les messages vocaux personnalisés sont particulièrement efficaces.

Application : prévoir un point téléphonique daté dans le mail d'envoi du devis (cf. `etapes-vente/03-envoi-proposition.md`), et tenir le créneau.

---

## Conventions de variables

### Variables Evaneos officielles

```
(**prénom ou nom du voyageur**)
(**votre destination**)
(**date du voyage**)
(**lien vers la proposition**)
(**indiquer une date et une heure**)
(**court message personnalisé**)
```

### Variables internes agence

`/*xxx*/` (à distinguer du format officiel ci-dessus).

Si copie d'un template officiel : remplacer **toutes** les variables avant envoi. Un placeholder oublié = message creux.

---

## Indicateur Evaneos : notation 1-5 étoiles voyageur

Les templates Evaneos utilisent une notation 1-5 étoiles pour qualifier le voyageur dès la prise de contact.

| Étoiles | Description | Templates adaptés |
|---|---|---|
| 1-2 | Voyageur indécis, en exploration | Templates pédagogiques (1.2, 1.8) |
| 3-5 | Voyageur décidé, demande précise | Templates directs (1.1, 1.6, 1.7) |

Si on connaît la notation Evaneos d'un client, adapter le ton du premier contact.

---

## Faiblesses du système officiel à corriger systématiquement

Les templates officiels Evaneos sont datés et auto-louangeurs. Audit rapide à faire avant tout copy-paste :

| Pattern à corriger | Présent dans | Correction |
|---|---|---|
| "ravi de recevoir" / "Comment allez-vous ?" | Templates 1.x, 2.4 | Ouverture concrète sur le projet |
| "je suis fièr(e)", "j'ai pris soin" | 2.1 | Supprimer, structure factuelle |
| "votre beau projet de voyage" | 2.1, 1.04 | Reformuler avec des éléments concrets du projet |
| "nos chers clients" | 2.4 | Supprimer ou reformuler |
| "complètement convaincu(e)" | 2.4 | Supprimer (présume) |
| Smiley `;)` | 2.4 | Supprimer (interdit pour Alison, à arbitrer pour les autres) |
| "inoubliable" | 1.04 | Remplacer par fait concret |

Détails complets dans `humanizer-kl-rules.md` §1.4.

---

## Patterns Evaneos officiels qui ont fait évoluer les règles internes

| Règle initiale skill v1 | Réalité Evaneos officielle | Règle finale |
|---|---|---|
| Pas de bullets sur Evaneos | Template 2.1 utilise des bullets pour next steps | Bullets autorisés pour listes administratives |
| Pas d'emoji ni smiley | Template 2.4 contient `;)` | Smileys ASCII tolérés selon agent (interdits pour Alison) |
| Variables `/*nom*/` | Officiel utilise `(**nom**)` | Documenter les deux conventions |
| ByNativ réservé à DE | Template 2.1 mentionne "notre partenaire" | Sur Evaneos, "notre partenaire vols" générique OK |

---

## Multi-canal légitimé

Le template 2.5 valide explicitement la mention multi-canal dans les relances.

Citer les canaux déjà tentés (mail + appel + WhatsApp + message vocal) renforce la légitimité du message et n'est pas perçu comme du harcèlement.

Exemples de formulation acceptées :

- "Je vous écris suite à mon précédent mail et au message vocal que je vous ai envoyé."
- "J'ai essayé de vous contacter par téléphone mais je n'ai pas réussi à vous joindre."

---

## Articulation avec les autres fiches

| Fiche | Rôle |
|---|---|
| `sales-process-evaneos.md` (ce fichier) | Référence officielle Evaneos |
| `plateformes/evaneos.md` | Règles spécifiques à la plateforme (ton, mentions, format) |
| `etapes-vente/03-envoi-proposition.md` | Structure du devis (basée sur 2.1) |
| `etapes-vente/04-relance-silence.md` | Relances (2.4 et 2.5) |
| `humanizer-kl-rules.md` | Anti-IA et anti-templates datés |

---

## Versioning

| Date | Changement |
|---|---|
| 2026-04-28 | Aspiration du portail Partner Connect Evaneos |
| 2026-05-06 | Création du fichier atomique, extraction depuis archives/messages-clients-skill-COMPLET.md |
