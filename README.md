# Scanner I2C LCD

Mini-projet de conception PCB – BTS CIEL 2 (Électronique et Réseaux)

Scanner d'adresses I2C autonome, basé sur un microcontrôleur **ATtiny84** et un écran LCD **HD44780**. Il suffit de brancher un composant I2C sur le scanner : la première adresse détectée s'affiche sur l'écran, sans avoir besoin d'un ordinateur ni de la documentation du composant.

## Objectif

Proposer un circuit imprimé prêt à être fabriqué :

- une seule face de pistes (et éventuellement quelques ponts)
- format Eurocard sans connecteur de rack
- sérigraphie complète (nom du concepteur, du fichier, date)
- routage à la main, en brouillant les pistes (approche « cyber »)
- composants brasés sur le PCB, selon la nomenclature imposée
- points de test placés judicieusement

## Nomenclature de base

| Désignation | Valeur | Quantité |
|---|---|---|
| Microcontrôleur | ATtiny84 P-PU | 1 |
| Écran LCD | Hitachi HD44780 | 1 |
| Bornes de connexion | PinHeader | [à définir] |
| Bornier à vis | 5,08 mm | 1 |
| Résistances | 4,7 kΩ | 2 |
| Potentiomètre | 10 kΩ horizontal | 1 |

## Organisation du dépôt

```
Scanner_I2C_LCD/
├── README.md
├── docs/                 Sujet du projet et datasheets
├── kicad/                Projet KiCad (schéma + PCB)
├── simulation/           Projet SimulIDE et captures
├── code/                 Code C (IDE Arduino)
└── dossier_technique/    Nomenclature, SysML, gamme de montage, tests
```

## Outils utilisés

- **KiCad** : schéma et routage du PCB
- **SimulIDE** : simulation préalable
- **Arduino IDE** : programmation de l'ATtiny84 en C

## Ouvrir le projet KiCad

Ouvrir le fichier `kicad/Scanner LCD.kicad_pro` avec KiCad. Le schéma (`.kicad_sch`) et le PCB (`.kicad_pcb`) se trouvent dans le même dossier.

## Auteur

Enzo – BTS CIEL 2, [établissement] – [année scolaire]
