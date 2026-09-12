# TABOUKA — Axiom Mali

Dashboard statique de prospection minière et pétrolière au Mali. L'application est disponible directement dans `index.html` et ne nécessite ni serveur applicatif ni étape de compilation.

## Utilisation locale

Depuis la racine du dépôt, lancez un serveur HTTP statique, par exemple :

```powershell
python -m http.server 8000
```

Puis ouvrez <http://localhost:8000>. Un serveur HTTP est recommandé plutôt qu'une ouverture `file://`, car les cartes Leaflet et les ressources CDN sont chargées à distance.

## Fonctionnalités

- Carte interactive des ressources, avec affichage initial des gisements aurifères.
- Modules thématiques et graphiques scientifiques.
- Fenêtres déplaçables, fermeture par `Échap` et navigation mobile avec menu latéral.
- Thèmes visuels par ressource et marqueurs filtrés sur la carte.

## Déploiement

Le workflow `.github/workflows/pages.yml` publie automatiquement la racine du dépôt sur GitHub Pages après chaque push sur `main`. Dans les paramètres du dépôt, la source Pages doit être configurée sur **GitHub Actions**.