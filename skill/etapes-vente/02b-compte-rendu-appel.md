# Étape 02b — Compte rendu d'appel de découverte

## Objectif

Envoyer au client, après l'appel de découverte, un message qui :

1. Reformule ce que l'agent a compris du projet (synthèse fluide, pas de retranscription mécanique)
2. Confirme les points validés ensemble
3. Liste les points restés ouverts ou à affiner
4. Pose les prochaines étapes concrètes

Ce message n'est pas un devis. Il ne propose pas de prix. Il ferme la boucle de compréhension et évite les malentendus avant que le travail de construction du voyage commence.

---

## Déclencheur

L'agent colle ses notes brutes d'appel dans le chat (peu importe le format : fragments,
tirets, abréviations) et indique :

- Le nom du client
- La plateforme
- L'agent qui signe

Claude structure et rédige le message à partir de ces notes.

---

## Canal de diffusion

Ce message est copié/collé depuis le draft Claude vers la plateforme d'origine :

- Evaneos : messagerie Evaneos (les notes d'appel sont saisies dans le champ dédié de la
  plateforme, séparé du fil client)
- Destination-Écosse : email via l'interface DE
- Kilt & Licorne : email direct

Le draft livré par Claude doit être propre, sans aucun balisage Markdown, prêt à coller
sans retouche autre que la date de livraison de la proposition si elle n'est pas encore
connue.

---

## Structure du message

### 1. Accroche courte

Phrase directe. Pas de "un grand merci pour notre échange" ni de "c'était un plaisir".

Exemples :
> "Suite à notre échange de [jour], voici ce que j'ai retenu de votre projet."
> "Je voulais revenir vers vous rapidement pour m'assurer que j'ai bien compris l'essentiel."

Adapter selon la voix de l'agent (cf. `agents/<prenom>.md`).

### 2. Synthèse du projet compris

Bloc narratif, 3 à 5 phrases. Pas une liste. L'agent écrit comme s'il résumait ce qu'il
a entendu à un collègue : contexte du voyage, composition du groupe, attentes principales,
contraintes identifiées.

Inclure si présents dans les notes :

- Dates et durée
- Composition du groupe (âges si famille)
- Régions / circuit envisagé
- Centres d'intérêt (nature, culture, whisky, randonnée, généalogie, etc.)
- Rythme souhaité (posé / intensif)
- Gamme d'hébergement (simple, charme, premium)
- Contraintes spécifiques (mobilité, allergie, budget déclaré, conduite à gauche)
- Type de voyage (FIT autonome, FIT guidé, Open Tour, GIR)

Ne jamais inventer ce qui n'est pas dans les notes. Si une information est absente ou
ambiguë, la signaler dans les points ouverts plutôt qu'interpréter.

### 3. Points validés ensemble

Ce que l'appel a fermement acté. Listés en bullets •. Maximum 5.

S'il n'y a aucun point vraiment verrouillé, sauter ce bloc.

### 4. Points à affiner

Ce qui reste ouvert, ce sur quoi le client a hésité, ce que l'agent doit creuser avant
de construire la proposition. Listés en bullets •.

Exemples :
- "• Le départ de Skye en milieu ou en fin de séjour reste à définir."
- "• Budget terrestre non précisé : je travaillerai sur une gamme intermédiaire en
  attendant votre retour."
- "• Allergie aux chats à confirmer de votre côté avant la sélection des hébergements."

### 5. Prochaines étapes

Une ou deux phrases, concrètes. Date de livraison de la proposition si connue, fourchette
honnête sinon.

CTA unique : la proposition à venir, ou un second call si nécessaire.

### 6. Signature

Signature standard de l'agent et de la plateforme (cf. `agents/<prenom>.md`).

---

## Règles spécifiques à cette étape

### Fidélité aux notes, pas au mot à mot

Le message reformule, il ne retranscrit pas. Les notes sont souvent lacunaires, abrégées,
dans le désordre. Claude les réorganise et les traduit en langage fluide.

### Ton : sobre et fonctionnel

Ce message n'est pas commercial. Pas de pitch agence, pas de relance, pas de valorisation
du voyage. C'est un compte rendu.

Ton direct, professionnel, respectueux du temps du client.

### Longueur cible

3 à 5 paragraphes. Un message trop long signe le manque de synthèse. Trop court, il donne
l'impression que l'agent n'a rien retenu.

### Règles permanentes applicables

Toutes les règles transverses s'appliquent :

- Aucun em-dash —
- Aucun balisage Markdown gras
- Aucun nom d'hôtel (aucun booking confirmé à ce stade)
- Séparation absolue des marques entre plateformes
- Voix de l'agent qui signe
- Un seul CTA

---

## Exemple de transformation notes → message

### Notes brutes (exemple)
