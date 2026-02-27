#  Analyse des Besoins – Clash Royale

## 1. Description du domaine

La base de données doit gérer un système de jeu similaire à Clash Royale.

Le système comprend :
- Des joueurs
- Des cartes
- Des decks
- Des combats
- Des clans
- Des arènes
- Des récompenses

---

## 2. Règles métier

### JOUEUR
- id_joueur (identifiant unique)
- pseudo (unique)
- niveau
- trophées
- or
- gemmes
- Un joueur appartient à 0 ou 1 clan.

### CLAN
- id_clan
- nom (unique)
- description
- nombre maximum de membres
- Un clan contient plusieurs joueurs.

### CARTE
- id_carte
- nom (unique)
- type (troupe, sort, bâtiment)
- rareté
- coût en élixir

### POSSEDER (association)
Un joueur possède plusieurs cartes.
Attributs :
- niveau_carte
- quantite

### DECK
- id_deck
- nom
- Un deck appartient à un joueur.
- Un deck contient exactement 8 cartes.

### COMBAT
- id_combat
- date
- résultat
- variation de trophées
- Oppose exactement 2 joueurs.

### ARENE
- id_arene
- nom
- trophées_minimum

### RECOMPENSE
- id_recompense
- or
- gemmes
- attribuée à un joueur

---

## 3. Contraintes métier importantes

- Pseudo joueur unique
- Nom carte unique
- Nom clan unique
- Deck = 8 cartes obligatoires
- Combat = exactement 2 joueurs

---

## 4. Hypothèses

- Un joueur ne peut appartenir qu’à un seul clan.
- Une récompense appartient à un seul joueur.
- Une carte peut être dans plusieurs decks.
