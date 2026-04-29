# kl-messages-clients-skill

Skill de rédaction des messages clients pour l'agence francophone basée en Écosse, à travers ses trois plateformes (Kilt & Licorne, Evaneos, Destination-Écosse) et ses huit conseillers voyage.

## À quoi ça sert

Quand un agent doit répondre à un prospect ou un client, ce repo fournit :

- Les profils de voix des 8 agents (Nicolas, Marie, Alison, Angélina, Johanna, Emily, Carole, Anastassia)
- Les règles spécifiques par plateforme (KL / Evaneos / DE)
- Les structures par étape de vente (premier contact, devis, relance, acompte, pré-départ, etc.)
- Les templates capturés (Evaneos officiels et internes, Destination-Écosse / ByNativ)
- Une fiche mémoire vivante des corrections apprises au fil des sessions
- Les données dossiers (CSV) issues du scrape API Ezus

## Comment l'utiliser dans Claude.ai

1. Créer ou ouvrir le projet "Templates / Communication clients" sur claude.ai
2. Coller le contenu de `PROJECT-INSTRUCTIONS.md` dans les Custom Instructions du projet
3. Uploader tous les fichiers `.md` du skill dans le Project Knowledge
4. Ouvrir une nouvelle conversation pour rédiger un message client

## Structure

- `skill/` — orchestrateur, agents, plateformes, étapes, ressources, templates
- `data/` — exports CSV et stats analytics issues du scrape Ezus
- `workflow/` — workflows n8n pour scrapes périodiques et automations futures
- `PROJECT-INSTRUCTIONS.md` — à coller dans Custom Instructions du projet Claude.ai

## Workflow d'apprentissage

À chaque session de rédaction qui aboutit à une correction :

1. Claude propose la mise à jour de `skill/ressources/retours-corrections.md`
2. Cette mise à jour est commitée sur GitHub
3. Le fichier est re-uploadé dans le Project Knowledge

Le repo est ainsi la **source de vérité versionnée** du skill.

## Confidentialité

Repo **privé**. Ne jamais basculer en public.

- Les fichiers du `skill/` sont anonymes et peuvent en théorie être partagés
- Les fichiers `data/` contiennent des références clients réelles et restent strictement internes
- Aucune clé API, aucun token, aucun mot de passe ne doit être commité (cf. `.gitignore`)

## État actuel

Première version migrée depuis l'environnement Cowork local le 28 avril 2026.

## Versioning

Chaque correction de Nicolas ou d'un agent fait l'objet d'un commit dédié dans `skill/ressources/retours-corrections.md`.
