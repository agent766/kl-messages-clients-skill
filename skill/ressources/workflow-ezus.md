# Workflow Ezus — proposition client

À consulter quand un lien Ezus est partagé dans le chat (ex : `https://pages.ezus.io/thecampbox/[client-folder]/index.html`) avant de rédiger un message qui s'appuie sur la proposition.

---

## Principe général

Ezus (Travel Studio) est l'outil de devis et de réservation utilisé par l'agence pour produire les propositions client (HTML, mobile-friendly).

Chaque proposition client est hébergée à une URL stable de la forme :

```
https://pages.ezus.io/thecampbox/[client-folder]/index.html
```

L'arborescence d'une proposition contient typiquement :

- `index.html` : sommaire / page d'accueil
- Pages par jour (J1, J2, etc.) avec étapes, hébergements, activités
- Récapitulatif tarifaire
- Conditions générales
- Documents annexes (carnet de voyage, facture, etc.)

---

## Avant de rédiger un message qui référence une proposition Ezus

### 1. Récupérer les éléments factuels

Extraire de la proposition (manuellement ou via fetch) :

- Nombre de nuits / jours
- Dates de départ et de retour
- Composition voyageurs
- Régions traversées
- Type d'hébergement (sans nommer les hôtels avant booking confirmé, cf. `regles-redaction-transverses.md` §2)
- Activités principales
- Mode de transport (auto-tour, guide privé, OT, train, ferries)
- Montant terrestre (et préciser hors-vols, assurance, restauration)

### 2. Vérifier la cohérence

- Itinéraire ↔ dates ↔ saison
- Budget ↔ gamme proposée
- Profil voyageur ↔ rythme proposé
- Distances quotidiennes raisonnables (cf. `red-flags-projets.md` §3.4)

Si écart, le signaler dans le message accompagnant l'envoi (cf. `etapes-vente/03-envoi-proposition.md`).

### 3. Préparer les blocs explicatifs

Le template Evaneos 2.1 demande **trois blocs explicatifs** dans le mail d'envoi :

1. Choix des étapes (pourquoi ce circuit, points forts du parcours)
2. Choix des hébergements (emplacement, ambiance, adaptation au profil)
3. Choix des transports (logique mode + niveau d'autonomie)

Ces blocs ne reprennent pas la proposition Ezus mot pour mot, ils en font la synthèse commerciale.

---

## Conventions de référence dans les messages

### Lien Ezus dans le message

Toujours présenter le lien comme un appel à l'action clair :

> "Voici la proposition que je vous ai construite : [lien Ezus]"

Pas de "veuillez trouver ci-joint" ou de "n'hésitez pas à consulter".

### Pas d'incrustation d'images Ezus

Ne pas copier-coller des captures de la proposition dans le mail. Le lien suffit, la proposition est mobile-friendly.

### Versions successives

Si plusieurs versions de la proposition sont envoyées (ex : v1 puis v2 après modifications), :

- Mentionner explicitement quelle version est concernée
- Lister les changements effectués depuis la dernière version
- Garder le même lien Ezus si l'agence a mis à jour la proposition existante (Ezus écrase la version)

---

## Pièges fréquents

### 1. Mention d'un hôtel par son nom dans le mail

La proposition Ezus peut afficher des hôtels par leur nom **avant booking confirmé** (option commerciale). Le mail accompagnant la proposition ne doit **jamais** nommer un hôtel non confirmé (cf. `regles-redaction-transverses.md` §2).

### 2. Référence à un prix qui a changé

Si la proposition Ezus a été mise à jour (changement de saison, nouvelle gamme), vérifier que le prix mentionné dans le mail correspond à la version actuellement en ligne.

### 3. Lien obsolète

Vérifier que le lien Ezus est valide avant envoi. Une proposition supprimée ou archivée renvoie une 404.

### 4. Cross-promotion via Ezus

Le subdomain `pages.ezus.io/thecampbox/` est commun aux propositions Evaneos et Kilt & Licorne (entité juridique The Camp Box). Ne **pas** mentionner cette infrastructure dans un message Destination-Écosse.

---

## API Ezus (si récupération automatique)

L'API Ezus (api.ezus.app) permet de récupérer les détails d'une proposition par référence.

Conventions à respecter (voir `CLAUDE.md` racine projet) :

- Paramètre = `reference` (jamais `project_reference`)
- `day.accomodations` avec UN seul `m` (pas `accommodations`)
- Comparaisons de chaînes : toujours normaliser en NFC avant de comparer
- `proj.currency` retourne `'€'`, pas `'EUR'`
- `item.currency` et `item.exchange_rate` n'existent **PAS** dans l'API
- Rate limit Ezus : max 5 appels parallèles
- Toujours tester sur des entités de test avant la production

---

## À enrichir

Cette fiche est un squelette. À étoffer avec :

- Cas d'usage concrets de fetch + reformulation
- Exemples de blocs explicatifs (étapes / hébergements / transports) bien rédigés
- Mapping des champs Ezus utiles pour les messages clients
- Workflow de mise à jour de proposition (v1 → v2)

---

## Articulation avec les autres fiches

| Fiche | Rôle |
|---|---|
| `workflow-ezus.md` (ce fichier) | Récupération et utilisation de la proposition Ezus |
| `etapes-vente/03-envoi-proposition.md` | Mail d'envoi du devis (s'appuie sur la proposition Ezus) |
| `etapes-vente/07-modification-devis.md` | Mise à jour de proposition (v1 → v2) |
| `regles-redaction-transverses.md` §2 | Hôtels jamais nommés avant booking confirmé |

---

## Versioning

| Date | Changement |
|---|---|
| 2026-05-06 | Création initiale (squelette) |
