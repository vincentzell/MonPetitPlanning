# Planning Personnel

Outil statique permettant d'extraire et d'imprimer un planning individuel à partir d'un fichier Excel multi-feuilles.

## Fonctionnement
- **Local uniquement** : Le fichier Excel est lu par le navigateur. Aucune donnée n'est envoyée vers un serveur.
- **Filtrage** : Extraction par nom d'employé et par plage de dates.
- **Impression** : Mise en page optimisée pour le format A4 portrait (8 semaines par page).
- **Persistance** : Les préférences (nom, thème, options d'affichage) sont stockées dans le `localStorage`.

## Dépendance
Le script utilise la bibliothèque **SheetJS** pour traiter les fichiers `.xlsx` :
- Lien distant (CDN) : `https://cdnjs.cloudflare.com/ajax/libs/xlsx/0.18.5/xlsx.full.min.js`

## Installation sur GitHub Pages
1. Déposer `index.html` à la racine du dépôt.
2. S'assurer que le script `xlsx.full.min.js` est présent localement ou pointer vers le lien distant ci-dessus dans le code.
3. Activer GitHub Pages dans **Settings > Pages** (Branche : `main`).

## Structure du fichier Excel attendue
- Un onglet par mois (ex: "Janvier", "Février", etc.).
- Les noms en colonne A.
- Une ligne d'en-tête contenant les jours de la semaine et les numéros de jour.
