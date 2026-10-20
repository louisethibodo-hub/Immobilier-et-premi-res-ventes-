Standard · Plan de build

# Du site en ligne à la première vente, en deux semaines.

Chaque étape produit quelque chose que tu peux voir tourner. Chaque session de travail se termine sur un site qui fonctionne, jamais sur du code à moitié fini.

## Un arbitrage à connaître avant de commencer

Tu m’as donné deux consignes qui se heurtent : « première vente cette semaine, une page, un bouton payer » d’un côté, un tunnel complet de six écrans avec paywall détaillé de l’autre. Avec moins de 5 h par semaine, on ne fait pas les deux en même temps. Je tranche ainsi :

- **Semaine 1 : le strict minimum qui encaisse.** Une page d’accueil, un bouton payer, un accès ouvert après paiement. Tu vends à la main à tes premiers clients, en créant leur base avec eux.
- **Semaine 2 : le produit et le tunnel complet.** Réponse en un clic, détection des nouvelles questions, statistiques, trois questions, résultat personnalisé, avant-goût et paywall.

## Semaine 1 — Encaisser

Étape 0 · environ 45 min

### Ouvrir les quatre comptes gratuits

GitHub · Vercel · Supabase · Stripe (mode test)

- Je te guide un compte à la fois, avec les captures d’écran décrites en mots.
- Aucun service payant à ce stade. Le seul coût possible plus tard : un nom de domaine, environ 10 € par an.

**Test en 30 secondes :** tu te connectes aux quatre tableaux de bord sans erreur.

Étape 1 · environ 1 h 30

### Site en ligne : page d’accueil, pages légales, page 404

Premier déploiement sur Vercel, dès aujourd’hui

- Une page d’accueil pensée pour le téléphone : promesse en une phrase, douleur chiffrée, trois bénéfices, un seul bouton « Commencer ».
- Aperçu de lien propre (Open Graph) pour TikTok, Instagram et WhatsApp.
- Mentions légales, CGV et politique de confidentialité rédigées, avec les champs à compléter clairement marqués (raison sociale, SIRET, adresse).
- Page 404 et page d’erreur qui ramènent à l’accueil.

**Test en 30 secondes :** tu ouvres l’adresse Vercel sur ton téléphone et tu colles le lien dans WhatsApp : l’aperçu s’affiche.

Étape 2 · environ 1 h 30

### Le bouton payer, en mode test puis en réel

Stripe Checkout + webhook vérifié côté serveur

- Bouton d’abonnement à 35 €/mois, page de paiement Stripe, page de remerciement, message clair si le paiement échoue.
- Le webhook confirme chaque paiement côté serveur. L’accès n’est jamais accordé sur la seule redirection.
- Paiement de test de bout en bout avec une carte fictive, puis bascule en production.

**Test en 30 secondes :** tu paies avec la carte de test 4242 4242 4242 4242 et le paiement apparaît dans Stripe et dans la base.

Étape 3 · environ 1 h 30

### Accès après paiement et vente à la main

Supabase : connexion par lien magique, abonnement relié au client

- Le client reçoit un lien de connexion par e-mail, sans mot de passe à retenir.
- Une page « Ma base » minimale s’ouvre juste après le paiement, avec un état vide qui explique quoi faire.
- Un moyen pour toi de créer un compte et de pré-remplir sa base à la main.

**Test en 30 secondes :** tu paies en test, tu cliques le lien reçu et tu arrives sur ta base vide, connectée.

**Si le temps manque :** les étapes 0 à 2 suffisent pour encaisser. L’étape 3 peut glisser de quelques jours, et tu livres alors le premier client à la main.

## Semaine 2 — Le produit et le tunnel

Étape 4 · environ 1 h 30

### La base de questions fréquentes, remplie en dix minutes

- Ajout rapide : une question, une réponse, des mots-clés.
- Une base de départ prête à importer, avec les questions typiques du métier, pour que personne ne parte d’une page blanche.

**Test :** tu remplis dix questions en moins de dix minutes depuis ton téléphone.

Étape 5 · environ 2 h

### Réponse proposée en un clic, modifiable avant envoi

- Le client colle le message reçu, le produit propose la meilleure réponse de sa base, il la modifie, puis la copie.
- Chaque réponse utilisée est comptée, ce qui alimente les statistiques.

**Test :** tu colles une vraie question et la bonne réponse apparaît en un clic.

Étape 6 · environ 1 h 30

### Détection des questions nouvelles

- Quand aucune réponse ne correspond, la question est mise de côté et proposée à l’ajout dans la base.

**Test :** une question inconnue arrive dans la liste « À ajouter ».

Étape 7 · environ 1 h

### Statistiques : temps gagné, questions les plus fréquentes

- Temps gagné estimé en heures par mois, classement des dix questions les plus posées.

**Test :** après quelques réponses, les chiffres s’affichent sur l’accueil du compte.

Étape 8 · environ 3 h (sur deux sessions)

### Le tunnel complet et le paywall

- Trois questions, un écran chacune, barre de progression.
- Résultat personnalisé qui chiffre ce que la situation coûte aujourd’hui.
- Avant-goût gratuit utilisable, suite verrouillée mais visible.
- Paywall dans l’ordre voulu : rappel, gain chiffré, formules avec prix par jour, garantie en clair, « sans engagement » à côté du bouton, paiement sur le même écran, quatre questions fréquentes. Aucun faux avis, aucun faux compte à rebours.

**Test :** parcours complet sur téléphone, de l’accueil au paiement de test, en moins de deux minutes.

Étape 9 · environ 1 h

### Mesure d’audience et finitions

- Mesure d’audience respectueuse de la vie privée (sans bandeau de cookies), contrôle de vitesse sur 4G, relecture du français.

**Test :** tu vois le nombre de visiteurs du jour, et la page s’affiche en moins de 2 secondes.

Étape 10

### Plan de lancement sur 14 jours

- Jour par jour : quoi publier, où trouver tes dix premiers clients, quoi leur écrire, quand relancer. Sans vidéo de toi, sans appel.

## Ton prix : 35 €, est-ce le bon ?

| Prix | Clients pour 1 000 € | Clients pour 3 136 € |
| --- | --- | --- |
| 35 € | 29 | 90 |
| 49 € | 21 | 64 |
| 59 € | 17 | 54 |

Si un professionnel gagne seulement une demi-heure par jour, cela représente une dizaine d’heures par mois : 35 € est un prix très bas pour cette valeur. Il rassure pour les premières ventes, mais il t’oblige à trouver 90 clients, ce qui est lourd avec moins de 5 h par semaine, sans vidéo ni appel.

**Ce que je ferais :** garder 35 € pour tes dix premiers clients, afin d’apprendre vite, puis passer à 49 € pour les suivants. Pour le paywall, j’ajouterais une formule annuelle (deux mois offerts) qui t’apporte de la trésorerie dès la vente. À 49 €, 64 clients suffisent pour ton objectif.

## Trois décisions qui engagent le produit

**1. Stripe ou Whop :** Stripe. Standard est un logiciel avec un compte et des données, pas un accès à une communauté. Whop n’apporterait rien ici.

**2. Comment la bonne réponse est trouvée (étape 5) :** par recherche de mots-clés dans la base du client (gratuit, instantané, prévisible), ou par intelligence artificielle (plus souple mais payante à chaque réponse). Je recommande les mots-clés pour le MVP : zéro coût variable, et l’IA pourra s’ajouter ensuite.

**3. Qui est ta cible précise :** « Immobilier » est large (agents, syndics, gestionnaires locatifs, marchands de biens). La base de départ et le texte de la page d’accueil dépendent de ce choix. Plus il est précis, plus ta vidéo et ta page parlent à quelqu’un.

## Hors périmètre, volontairement

Connexion directe à WhatsApp, e-mail ou SMS, application mobile, équipes et plusieurs utilisateurs, réponses par intelligence artificielle, factures personnalisées. Si l’une de ces idées te paraît indispensable, tu me la signales et on décide ensemble.

Le client copie la réponse et l’envoie lui-même depuis son application habituelle : c’est ce qui garde le MVP faisable en deux semaines.