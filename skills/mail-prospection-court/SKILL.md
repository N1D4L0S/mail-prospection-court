---
name: mail-prospection-court
description: Use when writing, rewriting or A/B testing a short French prospecting e-mail sent in volume from a mailing tool (cold mail, campagne, mailing, lot, démarchage), for a freelancer or small studio selling custom work to businesses. Covers register, structure, personalisation by attributes, subject line, pre-send checks and how to process replies and bounces.
---

# Mail de prospection court, envoyé en volume

Un mail de démarchage de 100 à 150 mots, envoyé par centaines depuis un
outil de mailing, personnalisé par des attributs, pour vendre un travail sur
mesure à des dirigeants d'entreprise. Ce n'est pas le mail nominatif avec
pièce jointe, écrit un par un : ici, le texte est écrit une fois, et c'est la
donnée qui le personnalise.

Tout ce qui suit a été validé sur une campagne réelle. Les règles viennent
des corrections de l'expéditeur, pas d'une méthode de vente.

## 1. Le registre : écrit comme on parle

Le premier jet « selon la méthode » a été rejeté en un mot : ça sent l'IA.
La version qui a marché a été réécrite par l'expéditeur, en français parlé.
Ce qui distingue son texte d'un texte de machine :

- **Des phrases courtes, une idée chacune.** « L'idée, c'est que l'appli
  est à vous. » Pas de subordonnées empilées. Pas de « ainsi », « par
  ailleurs », « en effet », « n'hésitez pas ».
- **Aucun équilibre rhétorique.** Pas de « non seulement… mais aussi », pas
  de triplettes, pas de phrase qui répond en miroir à la précédente. Une
  phrase dit une chose et s'arrête.
- **Le concret avant l'abstrait.** « Vos couleurs, vos produits, et pas
  d'abonnement mensuel par boutique. » plutôt que « une solution
  personnalisée et économique ».
- **Parler au pire des cas, jamais au meilleur.** « Vous ouvrez ailleurs, la
  facture ne bouge pas. » Pas de promesse de résultat, pas de « vous
  gagnerez », pas de pourcentage.
- **Jamais de délai de livraison.** Ni « en quelques semaines », ni « rapide à
  mettre en place ». Un délai écrit dans un mail devient un engagement.
- **Jamais de prix, jamais de fourchette.**
- **Ne jamais pointer ce que le prospect n'a pas.** « Vous n'avez pas
  d'application » devient « votre marque est dans le téléphone de vos
  clients ». Le prospect doit pouvoir refuser sans se sentir jugé, pour que
  la porte reste ouverte six mois plus tard.
- **Cinq à sept paragraphes d'une à deux phrases**, 110 mots pour la version
  courte. Au-delà de 150 mots, il y a une idée de trop.
- Pas de tiret cadratin, pas de séparateur, pas de citation, pas de gras, pas
  d'emoji. Vouvoiement de bout en bout.

Passe finale : relire à voix haute. Une phrase qu'on ne dirait pas au
téléphone se réécrit.

## 2. La trame

1. **Formule d'appel** : « Bonjour Madame Durand, » ou « Bonjour Monsieur
   Durand, ». Jamais le prénom seul. Sans civilité sûre : « Bonjour, » tout
   court (voir 5).
2. **Qui je suis, en une phrase**, avec la ville et le métier : « Je suis
   développeur à [ville], je fais des applis de commande et de fidélité pour
   des enseignes comme la vôtre. »
3. **La phrase à l'enseigne**, seulement si son nom est présentable : « Je
   pense qu'un tel produit pourrait être pertinent pour [Enseigne]. »
4. **L'idée**, en deux ou trois paragraphes courts (voir 3).
5. **L'appel à l'action** : une chose légère à accepter, et une porte de
   sortie. « Si ça vous intéresse, je peux vous faire une maquette rapide
   pour montrer à quoi ça ressemblerait chez vous. Sinon, vous pouvez jeter
   un œil à mon portfolio : [lien] ». Un seul lien dans tout le mail.
6. **La formule de fin**, toujours la même, chaleureuse et courte : « Merci
   beaucoup, et passez une belle journée. »
7. **Signature nue**, trois lignes : nom, structure et ville, téléphone.
   Pas de logo, pas de titre, pas de deuxième lien.

## 3. Les arguments : comment ils sont construits

Ce qui a été demandé, en une phrase : rassurer, économies, proximité,
facilité, sérieux et réactivité. Chaque argument est une phrase concrète,
jamais un adjectif :

- **La propriété.** Ce que le prospect achète lui appartient. « L'appli est
  à vous. Vos couleurs, vos produits, et pas d'abonnement mensuel par
  boutique. Vous ouvrez ailleurs, la facture ne bouge pas. »
- **L'actif contre la charge.** « Et comme elle vous appartient, elle est à
  votre actif. Un abonnement, c'est une charge, il n'en reste rien. »
- **La proximité.** « Vous m'avez moi au bout du fil, pas un support. »
- **Une maquette, pas une démonstration.** On ne montre pas un produit sur
  étagère, on propose une esquisse de ce que serait le leur. C'est ce qui
  distingue le sur-mesure de l'abonnement.

Ce qui a été écarté : les chiffres d'économie, les comparaisons avec un
concurrent nommé, le mot « innovation », les délais, tout ce qui commence par
ce que le prospect n'a pas.

## 4. Deux versions, pour un test A contre B

- **A, le mail court** : la trame ci-dessus, trois paragraphes d'idée en
  prose.
- **B, les avantages** : même ouverture, une phrase de principe (« Je les
  fais sur mesure, parce qu'une appli louée au mois ne vous appartient
  jamais. »), puis cinq puces d'une ligne, chacune un bénéfice concret, puis
  le même appel à l'action.

Deux lots de 100 tirés au sort dans la même cible, une version par lot. Ce
qu'on mesure : **les réponses humaines**, pas les ouvertures ni les clics.
Les lots suivants reçoivent la version gagnante. Sur la campagne d'origine,
la version courte a obtenu la première réponse chaude le jour même, la
version à puces aucune.

## 5. La personnalisation par attributs

| Attribut | Comment on l'obtient | Dans le mail |
|---|---|---|
| civilité et nom | Le prénom est tranché avec un fichier public de prénoms par sexe (en France, celui de l'INSEE) : civilité posée seulement si le prénom est porté à 90 % au moins par un seul sexe. Les prénoms étrangers que le fichier ignore se tranchent à la main dans une liste tenue dans le script. Les ambigus (Camille, Sasha, Dominique, prénoms chinois) restent sans civilité. Repérer les fiches où prénom et nom sont inversés. | `Bonjour{{ si civilité }} {{ civilité }} {{ nom }}{{ fin }},` |
| nom d'enseigne présentable | À partir de la raison sociale : nom commercial entre parenthèses s'il existe, mots de structure retirés (SAS, SARL, GROUPE, DEVELOPPEMENT, HOLDING, EXPLOITATION…), sigles courts gardés, noms trop génériques ou en majuscules illisibles rendus vides. | La phrase entière sous condition : nom vide, phrase absente. On ne cite jamais une raison sociale brute. |
| référence de campagne | un identifiant par entreprise | paramètre du lien de suivi |

Règle de décision : une civilité fausse coûte plus qu'une formule neutre,
un nom d'entreprise moche coûte plus qu'une phrase en moins. Dans le doute,
on omet.

## 6. L'objet

Minuscules, deux à cinq mots, factuel, il annonce le contenu : `appli de
commande et fidélité`, `ce qu'apporte une appli`. Pas de prénom, pas
d'enseigne, pas de faux « Re : », pas d'emoji, pas de question.

## 7. Le lien et la preuve

Pas de pièce jointe dans un mail de masse. Un seul lien, vers un portfolio,
avec un paramètre de campagne pour compter les visites. Le lien nu du
portfolio ne change jamais s'il est imprimé quelque part (cartes de visite,
QR code) : on ajoute un paramètre, on ne redirige pas. On compte les
visites, on ne piste pas les personnes.

## 8. L'outil de mailing, ce qui casse si on l'oublie

- Envoyer en HTML avec un gabarit qui porte le lien de désinscription. Une
  campagne partie en texte brut sans gabarit est tombée en indésirables avec
  un lien de désinscription cassé.
- Vérifier le rendu personnalisé par un vrai mail de test à soi-même, avec
  un abonné de démonstration qui porte tous les attributs. L'aperçu de
  l'outil n'applique pas toujours les attributs de l'abonné.
- Cadence lente, de l'ordre d'un mail toutes les 30 secondes : c'est bon
  pour la délivrabilité et pour la limite horaire du compte d'envoi.
- SPF, DKIM et DMARC en place sur le domaine avant le premier lot.
- Ne jamais renvoyer tels quels des réglages lus par l'API de l'outil s'ils
  contiennent des mots de passe masqués : l'outil peut les enregistrer comme
  nouveaux mots de passe.

## 9. Avant d'envoyer, dans cet ordre

1. **Relire la liste à l'œil**, nom de l'entreprise, domaine de l'adresse et
   titre de son site côte à côte. Un filtre par mots-clés ne suffit pas : sur
   la campagne d'origine, il laissait passer une plateforme d'emploi, une
   fondation, un maroquinier et des bowlings dans une cible de restauration.
   Un mail hors cible coûte de la crédibilité, pas seulement un envoi.
2. **Sortir de la liste les prospects suivis à part** (ceux à qui on prépare
   un mail nominatif ou une vidéo). Le mail de masse ne doit pas arriver
   avant.
3. **Vérifier la santé des entreprises** (procédures collectives, radiations)
   si un registre le permet.
4. **Mail de test** reçu et relu : formule d'appel, enseigne, lien,
   désinscription.
5. **L'accord explicite de l'expéditeur sur ce lot et ce texte.** Un accord
   sur un lot ne vaut pas pour le suivant.

## 10. Après l'envoi : lire tous les retours, pas seulement les réponses

| Type de retour | Action |
|---|---|
| rebond dur (adresse inconnue, domaine mort) | liste noire |
| réponse automatique « j'ai quitté l'entreprise » | liste noire, créer les remplaçants cités dans une liste à part |
| réponse automatique « absent » | marquer absent, créer les remplaçants cités, relancer plus tard |
| réponse qui révèle une entreprise hors cible | liste noire, noter le faux rapprochement pour que le prochain import ne le réintègre pas |
| réponse humaine | sortir la personne des listes de masse, ouvrir un dossier de suivi, rédiger la réponse pour l'expéditeur, ne jamais l'envoyer à sa place |

## Gabarits

### A, objet `appli de commande et fidélité`

```
Bonjour Monsieur Durand,

Je suis développeur à [ville], je fais des applis de commande et de fidélité pour des enseignes comme la vôtre. Je pense qu'un tel produit pourrait être pertinent pour [Enseigne].

L'idée, c'est que l'appli est à vous. Vos couleurs, vos produits, et pas d'abonnement mensuel par boutique. Vous ouvrez ailleurs, la facture ne bouge pas.

Et comme elle vous appartient, elle est à votre actif. Un abonnement, c'est une charge, il n'en reste rien.

Vous m'avez moi au bout du fil, pas un support.

Si ça vous intéresse, je peux vous faire une maquette rapide pour montrer à quoi ça ressemblerait chez vous. Sinon, vous pouvez jeter un œil à mon portfolio : [lien]

Merci beaucoup, et passez une belle journée.

[Prénom Nom]
[Structure], [ville]
[téléphone]
```

### B, objet `ce qu'apporte une appli`

```
Bonjour Madame Durand,

Je suis développeur à [ville]. Je fais des applis de commande et de fidélité pour des restaurateurs et des enseignes. Je pense qu'un tel produit pourrait être pertinent pour [Enseigne].

Je les fais sur mesure, parce qu'une appli louée au mois ne vous appartient jamais.

Ce que ça change, concrètement :

- plus d'abonnement par boutique, vous payez une fois
- vous joignez vos clients directement, par notification, sans passer par les réseaux sociaux
- vous récompensez vos meilleurs clients comme vous voulez, pas comme un prestataire l'a prévu
- votre marque est dans le téléphone de vos clients, pas dans l'appli de quelqu'un d'autre
- et c'est un actif : un produit numérique qui compte dans la valeur de votre entreprise, et qui se valorise avec le temps

Si vous voulez voir ce que ça donnerait chez vous, je peux faire une maquette rapide. Sinon, mon portfolio : [lien]

Merci beaucoup, et passez une belle journée.

[Prénom Nom]
[Structure], [ville]
[téléphone]
```

Le produit vendu ici est une application sur mesure ; la même trame vaut
pour tout travail sur mesure vendu à des dirigeants, en remplaçant les trois
arguments par ceux du métier, construits de la même façon : une phrase
concrète, au pire des cas, sans chiffre.

## Red flags

- « Bonjour Prénom », ou une civilité devinée sans règle.
- Une raison sociale brute dans le mail.
- Un délai, un prix, un pourcentage, une démonstration.
- Deux liens, une pièce jointe, un logo en signature.
- Une phrase qu'on ne dirait pas à voix haute.
- Une campagne en texte brut, ou sans lien de désinscription.
- Un lot lancé sans relecture de la liste à l'œil, ou sans accord explicite.
