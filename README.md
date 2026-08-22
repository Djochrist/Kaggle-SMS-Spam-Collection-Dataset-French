# Dataset français de détection des spams

<p align="center">
  <img src="https://img.shields.io/badge/🚀_VERSION-1.0-7c3aed?style=for-the-badge&labelColor=111827" alt="Version 1.0">
  <img src="https://img.shields.io/badge/📦_MESSAGES-10_000-0ea5e9?style=for-the-badge&labelColor=111827" alt="10 000 messages">
  <img src="https://img.shields.io/badge/🇫🇷_LANGUE-Français-f97316?style=for-the-badge&labelColor=111827" alt="Français">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/🧪_NATURE-Synthétique-e11d48?style=for-the-badge&labelColor=111827" alt="Dataset synthétique">
  <img src="https://img.shields.io/badge/🤖_USAGE-Entraînement_et_prototypage-16a34a?style=for-the-badge&labelColor=111827" alt="Entraînement et prototypage">
  <img src="https://img.shields.io/badge/⚖️_LICENCE-CC_BY_4.0-f59e0b?style=for-the-badge&labelColor=111827" alt="Licence CC BY 4.0">
</p>

> Dataset synthétique de messages français destiné à l’entraînement et au prototypage de modèles d’intelligence artificielle capables de détecter les spams.

## Présentation

Il existe encore peu de datasets francophones dédiés à la détection des messages indésirables. Ce projet a été créé pour fournir une première base accessible à la communauté, aux chercheurs, aux étudiants et aux développeurs qui souhaitent travailler sur la classification automatique des spams en français.

Cette version contient des SMS et des emails classés en deux catégories :

- `spam` : message indésirable ;
- `legitimate` : message légitime.

Les messages sont synthétiques, diversifiés et conçus pour servir de base à l’apprentissage, aux tests et au prototypage.

## Version précédente

Une première version du projet était basée sur la traduction en français de messages provenant d’un corpus anglophone. Cette approche reste utile pour constituer une base initiale, mais elle ne reflète pas toujours les formulations naturelles, les habitudes d’écriture et les contextes propres aux messages francophones.

Cette version propose donc un corpus généré directement en français :

[Consulter la version basée sur les traductions](https://github.com/Djochrist/Kaggle-SMS-Spam-Collection-Dataset-French)

## Chiffres clés

| Propriété | Valeur |
|---|---:|
| Nombre total de messages | 10 000 |
| Messages spam | 5 000 |
| Messages légitimes | 5 000 |
| SMS | 5 000 |
| Emails | 5 000 |
| Textes uniques | 10 000 |
| Langue | Français |
| Version | 1.0 |

## Structure du dataset

Le fichier principal contient les colonnes suivantes :

| Colonne | Description |
|---|---|
| `id` | Identifiant unique du message |
| `text` | Contenu du SMS ou de l’email |
| `label` | Catégorie du message |
| `domain` | Type de contenu : SMS ou email |
| `spam_category` | Catégorie du spam |
| `split` | Ensemble d’entraînement, de validation ou de test |
| `template_group` | Groupe de structure utilisé pour contrôler la séparation des données |

## Utilisations

Ce dataset peut être utilisé pour :

- entraîner un premier modèle de détection des spams ;
- tester des méthodes de classification de textes ;
- comparer des modèles de traitement automatique du langage ;
- créer des démonstrations et des prototypes ;
- tester des pipelines de préparation et d’évaluation des données ;
- contribuer à la recherche sur la détection des spams en français.

## Limites

Les messages de cette version sont synthétiques. Ils ne proviennent pas de conversations réelles et ne représentent pas nécessairement la diversité des messages reçus dans un environnement réel.

Le dataset doit donc être considéré comme une base de départ pour l’apprentissage et le prototypage. Il a vocation à évoluer progressivement vers un corpus plus réaliste, comprenant des messages réels anonymisés, légalement obtenus et annotés par des personnes compétentes.

Avant toute utilisation en production, il est recommandé d’évaluer le modèle sur un corpus réel indépendant.

## Séparation des données

Les messages sont répartis entre les ensembles :

- `train` : entraînement ;
- `validation` : réglage et comparaison des modèles ;
- `test` : évaluation finale.

Les familles de structures similaires sont séparées afin de limiter la présence de variantes proches dans plusieurs ensembles.

## Licence

Ce dataset est distribué sous licence **Creative Commons Attribution 4.0 International — CC BY 4.0**.

Vous pouvez l’utiliser, le modifier et le redistribuer, y compris dans un projet commercial, à condition de mentionner la source.

Attribution recommandée :

> Dataset français de détection des spams, version 1.0, corpus synthétique, 2026.

## Contribution

Les contributions sont les bienvenues, notamment pour :

- proposer des formulations françaises plus naturelles ;
- améliorer la diversité des messages ;
- signaler des erreurs ou des incohérences ;
- contribuer à l’anonymisation et à l’annotation de futurs messages réels ;
- suggérer de nouvelles catégories de spams.

## Évolution du projet

Cette version constitue une première étape. Le projet a vocation à évoluer vers un dataset plus représentatif des messages réels en français, avec davantage de diversité linguistique, de contextes et de catégories de spams.

Les retours de la communauté permettront d’améliorer progressivement la qualité et l’utilité du dataset.
