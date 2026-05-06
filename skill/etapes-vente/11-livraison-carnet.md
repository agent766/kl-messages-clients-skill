# Étape 11 — Livraison du carnet de voyage

## Quand

Entre J-30 et J-15 du départ, généralement avant le mail de pré-départ (étape 10).

## Objectif

1. Livrer le carnet de voyage (HTML hébergé Ezus + PDF si demandé)
2. Présenter sa structure et son utilisation
3. Inviter à signaler les éventuelles erreurs / omissions
4. Préparer le terrain pour le mail de pré-départ

## Structure

1. Salutation + accroche courte
2. Présentation du carnet (lien Ezus + format)
3. Structure du carnet :
   - Sommaire jour par jour
   - Hébergements avec coordonnées et plan d'accès
   - Activités et points d'intérêt
   - Conseils pratiques (météo, étiquette, urgences)
   - Contacts agence
4. Invitation à relire et à signaler les erreurs ou ajouts souhaités
5. Sign-off + annonce du mail de pré-départ à venir

Longueur cible : 12 à 18 lignes.

## Variations plateforme

### Kilt & Licorne

- Carnet hébergé sur Ezus (pages.ezus.io/thecampbox/)
- Lien direct, pas de PDF par défaut (sur demande)

### Evaneos

- Suivre les conventions de carnet propres au mandat Evaneos
- Pas de template officiel dédié

### Destination-Écosse

- Carnet souvent envoyé en PDF + version Ezus
- Marie peut joindre une lettre de suivi personnalisée

## Pièges

- Carnet livré sans mail d'accompagnement → le client ne sait pas quoi en faire
- Ne pas vérifier que le lien Ezus est valide avant envoi (cf. `workflow-ezus.md` §pièges)
- Mentionner un hôtel non confirmé dans le carnet (= problème pour plus tard si changement)
- Ne pas inviter le client à relire le carnet → erreurs découvertes sur place

## Référence Evaneos

- Pas de template officiel dédié
- Convention agence : carnet livré J-21 minimum

## Sous-skill transports

Si le voyage inclut des transports en commun (train, ferries, autocar), s'appuyer sur les contenus prêts à coller du sous-skill transports : `ressources/SKILL.md` et notamment `ressources/10-contenu-voyageur.md`.

## Template transverse (validé Nicolas 2026-05-06)

Applicable à toutes plateformes et tous agents. Adaptable selon les variations agent ci-dessous.

```
Bonjour [Prénom],

Votre carnet de voyage est prêt : [lien Ezus]

Avec lui, votre aventure écossaise devient un peu plus réelle.

Vous y retrouverez chaque journée détaillée, la route du jour sur la
carte, les étapes à ne pas manquer, vos hébergements avec leurs
horaires d'arrivée, et toutes les petites adresses que nous avons
sélectionnées pour vous.

Pas besoin d'imprimer quoi que ce soit, ce lien remplace les vouchers
papier d'autrefois. Vous gardez juste votre téléphone à portée de
main : tout y est, des numéros utiles aux références de réservation,
jusqu'aux instructions pour se garer ou récupérer les clés, même hors
connexion une fois la page chargée.

Chaque journée s'ouvre sur sa carte, ses points d'intérêt et les
détails pratiques qui vous éviteront de chercher quoi que ce soit sur
place.

Un récapitulatif des hébergements reste accessible en permanence
depuis le bouton dédié en bas de l'écran, pratique le soir au moment
du check-in.

Je vous propose un point téléphonique pour parcourir le carnet
ensemble. Nous pourrons affiner le programme, apporter les dernières
personnalisations selon vos envies, et répondre à toutes vos questions
avant le départ. Voici mon Calendly pour réserver un créneau qui vous
convient : [Calendly Agent]

Le mail de pré-départ vous parviendra ensuite d'ici une dizaine de
jours avec les derniers détails pratiques.

Bonne route,

[Agent]
[Plateforme si applicable]
```

## Variations agent

### Marie / Destination-Écosse

- Récap final formel autorisé : possibilité d'ajouter un bloc "Récap" structuré en gras (manuel dans l'éditeur cible) avec les 4-5 points clés du voyage juste avant le bloc Calendly
- Séparateur `---` autorisé avant l'invitation Calendly pour démarquer le CTA
- Calendly : https://calendly.com/desti-ecosse-marie/30min

### Nicolas / Kilt & Licorne

- Pas de variation forte sur le ton, garder direct
- Possibilité d'ajouter un tell de présence terrain juste avant la phrase carte/hébergements ("J'ai mis à jour deux adresses dîner sur Skye la semaine dernière, vous les retrouverez dans la fiche jour 4")
- Calendly : https://calendly.com/nico-caisso/30min

### Alison / Evaneos

- **Couper** la phrase "Avec lui, votre aventure écossaise devient un peu plus réelle" (trop chaude pour la voix sobre Alison)
- Garder le reste du template tel quel
- Sign-off : "Bien à vous, Alison" (sign-off Evaneos officiel possible : "Au plaisir de vous parler prochainement,")

### Angélina / Evaneos

- Possibilité d'insérer **un coup de cœur terrain concret** entre la description du carnet et le bloc Calendly, si pertinent au dossier client (ex : "Le petit déjeuner du B&B de Plockton est à ne pas rater, j'ai prévenu Catriona de votre passage")
- Sign-off : "Au plaisir de vous parler prochainement, Angélina" (Evaneos officiel)
- Calendly : https://calendly.com/angelina-etre/30min

### Squelettes (Johanna, Emily, Carole, Anastassia)

- Suivre le template transverse sans variation tant que la voix n'est pas affinée
- Sign-off selon plateforme

## Checklist vérification avant livraison

- [ ] Lien Ezus valide (cf. `workflow-ezus.md` §pièges)
- [ ] Pas d'hôtel non confirmé nommé dans le carnet
- [ ] Calendly de l'agent qui signe (cf. `agents/<prenom>.md` §Calendly)
- [ ] [Prénom] remplacé
- [ ] Aucun emoji Unicode (le bouton hébergements se référence en texte simple "bouton dédié" ou "bouton Hébergements" si l'agent veut le préciser)
- [ ] "Nous" pour l'équipe, pas "on" (cf. S11)
- [ ] Si plateforme = Evaneos : aucune mention KL/DE/ByNativ/Mister Fly
- [ ] Si plateforme = KL : Option Way nommé si pertinent au contexte
- [ ] Si plateforme = DE : Mister Fly nommé si pertinent au contexte

## À enrichir

- Template-type de retour client après relecture (réponse aux ajustements demandés en call)
- Variante "carnet réémis" si la proposition Ezus est mise à jour entre v1 et v2
- Liens utiles dernière minute spécifiques selon saison ou région
