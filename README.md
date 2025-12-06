# Cogni Robot - Hardware Repository

![Status](https://img.shields.io/badge/Status-Alpha-red) ![License](https://img.shields.io/badge/License-CC_BY--SA_4.0-lightgrey) ![Cost](https://img.shields.io/badge/Target_Cost-~300€-green)

**Cogni** est un projet de robotique open-source visant à démocratiser l'accès aux robots humanoïdes avancés. L'objectif est de recréer une plateforme basée sur la morphologie du [Poppy Humanoid](https://www.poppy-project.org/), mais repensée pour être ultra-accessible (low-cost), autonome et capable d'apprentissage continu en local.

## Avertissement (Version Alpha)

> **ATTENTION : Ce projet est actuellement en phase de développement actif (Alpha).**

* La modélisation est en cours.
* Je suis en phase d'apprentissage sur Fusion 360, les fichiers peuvent subir des refontes majeures sans préavis.
* **Il est fortement déconseillé d'imprimer ou d'assembler ce robot pour l'instant**, sauf si vous souhaitez contribuer activement au développement et au débogage.

## Objectifs du Projet

* **Coût drastiquement réduit :** Passer d'un budget de ~5000€ (Poppy Torso original) à environ **300€** (potentiellement moins avec des pièces d'occasion).
* **Autonomie énergétique :** Optimisation pour une consommation faible.
* **Intelligence Locale :** Conçu pour héberger des modèles/architectures innovantes capable d'apprendre en permanence (sans backpropagation classique) et en locale.
* **100% Open Source :** Hardware et Software entièrement libres.

## Modifications Hardware & Spécifications

Ce dépôt contient les fichiers 3D (STL et sources) modifiés pour adapter le design original à des composants plus abordables.

### Moteurs
J'ai remplacé les moteurs coûteux Dynamixel MX-28 par des moteurs **Feetech STS3215**.
* **Voltage :** 12V
* **Couple :** 30Kg/cm
* **Avantage :** Rapport qualité/prix imbattable pour des performances similaires.

### Adaptations 3D
Pour rendre ces moteurs compatibles avec la structure humanoïde :
* Création d'une **"couronne" adaptatrice** spécifique : Cette pièce permet au moteur STS3215 d'avoir des dimensions externes et des points de fixation similaires au Dynamixel MX28-T.
* Modification des pièces (en cours) et des autres membres pour intégrer ces nouveaux actuateurs.

## Structure du Dépôt

* `/STL` : Fichiers prêts à imprimer (Mesh).
* `/STEP` : Fichiers sources (STEP) pour modification.
* `/docs` : Instructions d'assemblage (à venir).

## Licence et Crédits

Ce projet hardware est un **fork** (œuvre dérivée) du projet [Poppy Humanoid](https://github.com/poppy-project/poppy-humanoid).

### Fichiers 3D (Hardware)
Conformément à la licence originale du projet Poppy, tous les modèles 3D, les fichiers CAO et les adaptations présents dans ce dépôt sont distribués sous la licence **Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)**.

Cela signifie que vous êtes libre de partager et d'adapter ce matériel, à condition de :
1.  **Créditer les auteurs** (voir ci-dessous).
2.  **Distribuer vos contributions sous la même licence** (CC BY-SA 4.0).

### Attribution / Crédits Originaux
Le design original du robot humanoïde, dont ce projet est inspiré et adapté, est l'œuvre de :
* **Matthieu Lapeyre** (Créateur original)
* **L'équipe du Poppy Project**
* **Inria** (Institut national de recherche en sciences et technologies du numérique)

Source des fichiers originaux : [https://github.com/poppy-project/poppy-humanoid](https://github.com/poppy-project/poppy-humanoid)

*Note : Le code source et les futurs modèles d'IA de Cogni (situés dans des dépôts séparés) sont des créations originales ("from scratch") et seront soumis à des licences différentes.*

---
*Projet Cogni maintenu par [NotPunchnox](https://github.com/notpunchnox). Des mises à jour régulières sont prévues.*