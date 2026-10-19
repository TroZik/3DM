# 3DM

Visionneuse 3D interactive d'un moteur et de sa visserie, pensée pour le téléphone.

Premier modèle : **EA888 Gen 1 – code moteur CCTA** (2.0 TFSI), monté sur une **Audi A3 Sportback 8PA S line 2012**, boîte **DSG6 DQ250 (02E)**, transmission **Quattro**.

> Statut : **v0.2.0** – pièces internes (prototype : v0.1.0)

## Fonctionnalités

- Vue 3D du bloc moteur et de tout ce qui y est vissé : bloc, culasse, carter d'arbres à cames, carters d'huile, carters de distribution, flasque, volant bimasse, pompe à eau, support d'accessoires, capteurs, support moteur.
- Visserie détaillée : environ 200 vis réparties en 55 groupes.
- Fiche au toucher : couple, angle, vis à remplacer ou non, filetage, procédure, lien vers la source.
- **Ordre de serrage animé** (15 groupes), avec l'ordre de desserrage pour la culasse.
- Accessoires (alternateur, clim, turbo, admission, démarreur, DSG) affichés en silhouette avec leurs vis de fixation sur le moteur.
- **Pièces internes (v0.2)** : vilebrequin, bielles, pistons, arbres à cames, déphaseur, soupapes, ressorts, linguets et poussoirs, chaînes et tendeurs, arbres d'équilibrage, pompe à huile, gicleurs. Cotes et jeux du manuel dans les fiches.
- **Vue en coupe** et **rotation du moteur** : pistons, bielles, cames, soupapes et chaînes s'animent (ordre d'allumage 1-3-4-2).
- Vue éclatée, transparence du bloc, calques, recherche (par exemple « 9 Nm »).
- Code couleur des têtes de vis : rouge = à remplacer, gris = réutilisable, jaune = couple à compléter ou à vérifier.

## Utilisation

Aucune installation nécessaire. Ouvrir `index.html` dans un navigateur récent (Chrome, Safari, Firefox), sur téléphone ou sur ordinateur.

- 1 doigt : rotation
- 2 doigts : zoom et déplacement
- Toucher une pièce ou une vis : ouvre sa fiche

La bibliothèque 3D (three.js 0.147.0) est chargée depuis le CDN jsDelivr : une connexion internet est nécessaire.

## Structure

```
index.html          Application complète (HTML, CSS, JS et données)
docs/SOURCES.md     Origine des données techniques
docs/ROADMAP.md     Évolutions prévues
CHANGELOG.md        Historique des versions
LICENSE             Licence (tous droits réservés)
```

## Données et limites

- Couples, angles, vis à remplacer et ordres de serrage : manuel atelier VW « 4-cyl. injection engine (1.8 and 2.0 l engine, chain drive) », édition 08.2018 (voir `docs/SOURCES.md`).
- Formes et positions des pièces : **schématiques**, ce n'est pas un modèle CAO.
- Références pièces : à compléter (catalogue ETKA).
- Valeurs absentes du manuel moteur, marquées « à compléter » : vis boîte DSG ↔ moteur, démarreur, refroidisseur d'huile.

**Avertissement :** cet outil est une aide visuelle. Avant toute intervention, vérifier les valeurs dans la documentation constructeur à jour.

## Licence

© 2026 TroZik. Tous droits réservés. Voir [LICENSE](LICENSE).
