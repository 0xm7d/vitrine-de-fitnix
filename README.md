# FITNIX — Site vitrine d'une salle de sport

## Présentation

FITNIX est un projet pédagogique d'intégration web réalisé dans le cadre de la formation en développement web. L'objectif est de transformer une maquette Figma en un site vitrine de salle de sport, en utilisant principalement HTML5 et CSS3.

Le site présente les activités sportives, les entraîneurs, les formules d'abonnement, les témoignages et les coordonnées de contact. Il utilise une identité visuelle sombre avec des accents jaunes, une mise en page orientée fitness et des adaptations pour plusieurs tailles d'écran.

**Type de projet :** site vitrine statique, multipage  
**Période :** octobre 2026  
**Dépôt GitHub :** https://github.com/0xm7d/vitrine-de-fitnix  
**Maquette source :** `fitnix.fig` (fournie dans le brief pédagogique)

## Objectifs

- Intégrer la maquette Figma dans une interface web.
- Structurer le contenu avec HTML5 et CSS3.
- Construire des mises en page à l'aide de Flexbox et Grid.
- Adapter le site aux différentes largeurs d'écran avec des media queries.
- Permettre la navigation entre les sections du site.
- Travailler en équipe avec Git et GitHub.

## Pages du site

| Fichier | Contenu |
|---|---|
| `index.html` | Accueil, présentation de la salle, vidéo et section « About us ». |
| `programs.html` | Programmes d'entraînement, bénéfices et informations complémentaires. |
| `galleryH.html` | Présentation des entraîneurs et transformations avant/après, avec navigation par ancres. |
| `pricing.html` | Présentation de trois formules : Starter, Pro et Elite. |
| `testimonial.html` | Témoignages de membres et questions fréquentes (FAQ). |
| `contact-us.html` | Coordonnées, formulaire de prise de contact et invitation à une séance d'essai. |

Le brief initial prévoit cinq rubriques principales. L'implémentation contient six fichiers HTML distincts, dont des pages dédiées aux tarifs et témoignages, et une section « About us » sur l'accueil.

## Technologies et ressources

- **HTML5 :** structure des pages, contenus, navigation et formulaires.
- **CSS3 :** typographie, couleurs, espacements, animations, transitions et responsive design.
- **Flexbox et CSS Grid :** organisation des éléments et des sections.
- **Media queries :** adaptations aux différentes tailles d'écran.
- **Git et GitHub :** versionnement et collaboration.
- **Google Fonts et Font Awesome :** ressources typographiques et icônes utilisées dans certaines pages.
- **Images et vidéo locales :** illustrations sportives, portraits et séquence vidéo.

Aucun framework JavaScript ni processus de compilation n'est nécessaire pour consulter le site.

## Organisation des fichiers

```text
vitrine-de-fitnix/
├── index.html
├── programs.html
├── galleryH.html
├── pricing.html
├── testimonial.html
├── contact-us.html
├── style.css
├── image/
│   ├── logo.png
│   ├── pic1.avif ... pic4.avif
│   ├── autres images (JPG, AVIF, PNG, JFIF)
│   └── vidéo MP4
└── .vscode/
```

La feuille `style.css` centralise les styles des différentes pages. Les ressources multimédias se trouvent dans le dossier `image/`.

## Responsive design

La feuille CSS comprend plusieurs media queries, notamment pour les largeurs **1024 px, 900 px, 800 px, 768 px, 700 px, 600 px, 500 px, 480 px et 400 px**. Les règles adaptent les dimensions, l'organisation de plusieurs sections et certains éléments de navigation.

Un système de menu mobile reposant sur une case à cocher HTML et des règles CSS est présent dans le projet. Son comportement doit être vérifié sur toutes les pages et tailles d'écran avant la livraison finale.

## Fonctionnalités intégrées

- Navigation entre les principales pages via les menus de navigation.
- Présentation visuelle des programmes de musculation, HIIT/cardio, recomposition corporelle et fitness fonctionnel.
- Présentation des entraîneurs et de deux exemples de transformation avant/après.
- Affichage de trois formules d'abonnement.
- Section de témoignages et FAQ.
- Formulaire de contact avec plusieurs champs.
- Effets visuels et animations CSS.

**Limites fonctionnelles :** il s'agit d'un site statique. Aucun envoi d'e-mail côté serveur n'est configuré. Certains contrôles affichés (notamment les boutons de bascule tarifaire ou les flèches de témoignages) ne disposent pas de comportement interactif JavaScript confirmé.

## Travail collaboratif

Le projet a été développé en groupe, avec Git et GitHub pour centraliser les contributions, organiser les branches et intégrer les modifications.

- **Dépôt :** https://github.com/0xm7d/vitrine-de-fitnix
- **Historique des contributions :** https://github.com/0xm7d/vitrine-de-fitnix/commits/main
- **Pull requests :** https://github.com/0xm7d/vitrine-de-fitnix/pulls
- **Planification GitHub Projects :** https://github.com/users/0xm7d/projects/3

La répartition nominative précise des tâches peut être ajoutée après confirmation par les membres de l'équipe.

## Points à améliorer identifiés dans `main`

Lors de la revue du dépôt du **16 octobre 2026**, les éléments suivants restaient à vérifier ou à corriger :

1. Certains liens de footer référencent `trainers.html` ou `testimonials.html`, alors que les fichiers présents s'appellent `galleryH.html` et `testimonial.html`.
2. Certaines références d'images utilisent un dossier `Images/` alors que les ressources du dépôt sont stockées dans `image/` ; vérifier les chemins et leur casse.
3. Le formulaire de contact ne dispose pas encore des attributs `required` et de vrais éléments `label` pour les champs principaux ; corriger aussi `type="submet"` en `type="submit"`.
4. Aucune carte de localisation intégrée n'a été confirmée dans le HTML de contact.
5. Certains liens ou contrôles utilisent des ancres vides et ne mènent pas à une action réelle.
6. GitHub Pages n'était pas activé dans les métadonnées du dépôt au moment de cette revue.

## Présentation du projet

La soutenance est organisée en quatre parties selon le brief pédagogique :

| Durée | Activité |
|---|---|
| 5 min | Démonstration du site et du responsive design. |
| 10 min | Explication du HTML, du CSS, de Flexbox, de Grid et des media queries. |
| 5 min | Questions / réponses techniques. |
| 10 min | Retour sur les difficultés, solutions et pistes d'amélioration. |

## Perspectives d'amélioration

- Harmoniser les liens de navigation et de footer.
- Renforcer l'accessibilité et les contrôles de formulaire.
- Corriger les chemins des ressources.
- Intégrer une carte de localisation si demandée par la maquette.
- Finaliser les vérifications multi-écrans et les tests W3C.
- Publier une version stable sur GitHub Pages.

---

*Projet réalisé à des fins pédagogiques dans le cadre de l'intégration web HTML & CSS, à partir d'une maquette Figma fournie.*
