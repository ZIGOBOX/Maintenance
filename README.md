# Suivi de maintenance — Tickets

Application web autonome en français pour créer, modifier, filtrer, imprimer et exporter des tickets de maintenance.

## Utilisation immédiate

Ouvrir `index.html` dans un navigateur moderne, puis cliquer sur **Nouveau ticket**.

## Publication sur GitHub Pages

1. Créer un dépôt GitHub, par exemple `tickets-maintenance`.
2. Ajouter les fichiers `index.html` et `README.md` à la racine du dépôt.
3. Dans le dépôt, ouvrir **Settings > Pages**.
4. Sous **Build and deployment**, sélectionner **Deploy from a branch**, branche **main**, dossier **/(root)**, puis enregistrer.
5. Ouvrir l'URL GitHub Pages affichée dans les paramètres après publication.

## Fonctions

- Références automatiques des tickets (`MAINT-AAAA-0001`).
- Bâtiments/secteurs, salles, descriptions, catégories, priorités et statuts.
- Signalant, intervenant, échéance, date de clôture, actions et observations.
- Tableau de bord et recherche/filtrage.
- Modification et suppression avec confirmation.
- Impression de la fiche depuis son formulaire.
- Export CSV (compatible Excel), sauvegarde et import JSON.
- Interface responsive, sans dépendance externe, sans compte nécessaire.

## Important : stockage et confidentialité

Les données sont conservées uniquement dans le stockage local du navigateur (**localStorage**), pas sur GitHub. Elles ne sont donc **pas partagées entre différents ordinateurs**. Un nettoyage des données du navigateur peut les supprimer : effectuez des sauvegardes JSON régulières. L'import JSON fusionne les tickets avec ceux déjà présents, par référence ; un ticket de même référence sera remplacé. N'enregistrez pas d'informations confidentielles dans un dépôt public. Pour un suivi multi-utilisateur en temps réel avec authentification, il faudra ajouter un serveur et une base de données.
