# musee-tutoriel

Projet pédagogique du musée des inventions absurdes. Ouvrir index.html dans un navigateur, sans installation ni serveur.

Les fichiers .git sont présents dans l'archive : l'historique et les branches font partie du projet de départ. Aucun dépôt distant n'est configuré.

HTML : contenu. CSS : présentation. JavaScript : compteur de votes local. Aucun service externe ni donnée personnelle.

## Mes explications (tutoriel S2)

- **Ma branche `feature/presentation`** : créée depuis `main`, elle m'a permis de réécrire la présentation de la collection sans toucher à la version commune pendant mon travail. Mon commit : `b2e5830`.
- **Sens des fusions** : les branches ont été fusionnées *vers* `main`. D'abord `feature/presentation` (avance rapide, sans commit de fusion), puis `feature/visite` (commit de fusion `2b66ac1`).
- **Le bug** : la fusion a réussi techniquement, mais le lien « Visiter » pointait vers `visites.html` alors que le fichier s'appelle `visite.html`. Git fusionne du texte ; il ne vérifie pas que le site fonctionne.
- **La correction** : branche `hotfix/lien-visite` créée depuis `main`, lien corrigé (`eb0e0cc`), puis fusionnée dans `main`.
- **Vérifications** : sur `main`, le bouton de vote incrémente le compteur, « Visiter » ouvre bien `visite.html` et « Accueil » ramène à la page d'accueil.
