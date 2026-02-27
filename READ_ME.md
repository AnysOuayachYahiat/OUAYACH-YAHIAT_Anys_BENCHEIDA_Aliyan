#  Mini-Projet TI404 – Partie 1  
## Conception d'une Base de Données – Clash Royale

###  Membres du binôme
- Nom Prénom
- Nom Prénom

---

#  Présentation du projet

Ce projet consiste à concevoir une base de données en suivant la méthode MERISE.

Le thème choisi est : **Clash Royale**.

L’objectif est de modéliser une base permettant de gérer :
- Les joueurs
- Les cartes
- Les decks
- Les combats
- Les clans
- Les arènes
- Les récompenses

---

#  Étape 1 – Analyse des besoins

Nous avons identifié les règles métier principales :

- Un joueur possède un pseudo unique.
- Un joueur peut appartenir à un seul clan.
- Un joueur possède plusieurs cartes avec un niveau propre.
- Un joueur peut créer plusieurs decks.
- Un deck contient exactement 8 cartes.
- Un combat oppose exactement 2 joueurs.
- Un combat se déroule dans une arène.
- Un joueur peut obtenir des récompenses.

Les détails complets sont disponibles dans le fichier `Analyse_Besoins.md`.

---

#  Étape 2 – MCD

Le Modèle Conceptuel de Données comprend les entités suivantes :

- JOUEUR
- CARTE
- DECK
- CLAN
- COMBAT
- ARENE
- RECOMPENSE

Le modèle inclut :

- Des associations N–N
- Des attributs d’association
- Des contraintes d’unicité
- Une cardinalité fixe (Deck = 8 cartes)

Le schéma MCD est fourni dans le fichier `MCD_ClashRoyale.pdf`.

---

#  Éléments avancés utilisés

- Association N–N avec attributs (Posséder)
- Contraintes d’intégrité métier
- Cardinalité fixe (8,8)
- Attributs uniques

---

#  Organisation du dépôt

- README.md
- Analyse_Besoins.md
- MCD_ClashRoyale.pdf
- Prompts/

---

Projet réalisé dans le cadre du module **TI404 – Bases de données 1**
