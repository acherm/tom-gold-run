# 🐱 Tom Gold Run

Un *endless runner* en 3D (Three.js) : cours sur la route à 3 voies avec **Tom le chat**, ramasse les lingots d'or pour bâtir de nouveaux villages, esquive les voitures (ou saute dessus !) et marque des buts avec les ballons.

▶️ **Jouer en ligne :** https://acherm.github.io/tom-gold-run/

## Contrôles

| Action | Clavier | Tactile (téléphone) |
|---|---|---|
| Changer de voie | ← → (ou A / D) | glisser gauche / droite |
| Sauter (et monter sur les voitures/caisses) | ↑ / Espace | glisser haut / **taper** |
| Glisser (passer sous les barrières) | ↓ | glisser bas |
| Pause | P | bouton ⏸️ |

## Le jeu

- 🪙 **Lingots d'or** comptés vers un objectif → atteint, tu **construis une maison** et ton village grandit.
- 🎵 **Sifflet** = temps (jauge en haut à gauche, +5 s).
- ⚽ **Ballon** = **+20 lingots** et **but automatique** dans la cage.
- 🛹 **Skateboard** (power-up) : boost de vitesse, aimant à lingots, on traverse les voitures.
- 🚗 **Voitures / caisses / barrières / ponts** : à esquiver, sauter ou glisser dessous.
- 🦝 Un **rival raton** te double parfois.
- 🐱 **Changement de personnage** à la fin de chaque niveau (Tom, Angela, Ginger, Ben, Hank, le Raton).
- 💥 Écrasé ou temps écoulé = **Game Over**, on recommence.

## Technique

100 % statique, **un seul fichier `index.html`**, aucun asset externe (toute la 3D est générée par primitives). Three.js est chargé depuis un CDN. Rien à compiler.

Pour jouer en local :

```bash
python3 -m http.server 8123
# puis ouvrir http://localhost:8123/index.html
```

(Les modules ES nécessitent un serveur `http://` — ouvrir le fichier en `file://` ne fonctionne pas.)
