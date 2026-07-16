# Cafet Santé — V10.3

Correction iPhone : conservation du lien personnel après fermeture de l’application.

## Pourquoi

Le fichier `manifest.webmanifest` imposait une adresse de démarrage générale.
À la réouverture, iOS perdait donc le paramètre personnel `?app=...`.

Cette version ne relie plus le manifest à la page. L’iPhone conserve alors
l’adresse exacte ajoutée à l’écran d’accueil, tout en utilisant
`apple-touch-icon.png` pour le logo.

## Mise à jour GitHub

1. Importer tous les fichiers à la racine du dépôt `cafetsante/cafet-sante`.
2. Remplacer les fichiers existants.
3. Cliquer sur `Commit changes`.
4. Attendre une à deux minutes.

## Test obligatoire

1. Supprimer l’ancienne icône Cafet Santé de l’iPhone.
2. Ouvrir le lien d’installation personnalisé.
3. Attendre « Prêt à installer ».
4. Sans tester l’espace, faire Partager → Sur l’écran d’accueil.
5. Laisser « Ouvrir comme app web » activé.
6. Ajouter l’icône.
7. Ouvrir, fermer complètement, puis rouvrir l’icône.
