# Planning Personnel

Outil pour extraire et imprimer un planning individuel à partir d'un fichier Excel.

## Fonctionnement

- Le fichier Excel est traité localement dans le navigateur. Aucune donnée n'est envoyée.
- Extraction par nom et plage de dates.
- Impression optimisée A4 portrait (8 semaines par page avec notes, 12 sans).
- Les préférences sont sauvegardées en local.

## Fonctionnalités

- Sélection du nom et de la période
- Mode sombre
- Options d'affichage : titre, période, date source, binôme, ligne de notes
- Surlignage des entêtes, week-ends travaillés, jours fériés travaillés

## Dépendance

SheetJS pour lire les fichiers `.xlsx` :
```html
<script src="https://cdnjs.cloudflare.com/ajax/libs/xlsx/0.18.5/xlsx.full.min.js"></script>
```

## Utilisation

1. Charger un fichier Excel (.xlsx)
2. Sélectionner votre nom
3. Définir la période (date de début et nombre de semaines)
4. Configurer les options d'affichage
5. Générer et imprimer

## Structure du fichier Excel

- Un onglet par mois (janvier, février, etc.)
- Colonne A : noms des employés
- Une ligne d'en-tête avec les jours et numéros
- Cellules : amplitudes (J6, J7, M4, S1, .RH, etc.)

## Installation

1. Placer `index.html` à la racine du repo
2. Activer GitHub Pages dans Settings
