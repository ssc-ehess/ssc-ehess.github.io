---
layout: page
permalink: /preparations/
title: Préparations
description: Préparer un environnement de programmation pour les sciences sociales computationnelles.
nav: true
nav_order: 2
toc: true
---

## Instructions pour préparer son environnement de programmation

### 1. Installer anaconda en suivant les instructions ci-dessous:

[https://docs.anaconda.com/anaconda/install/](https://docs.anaconda.com/anaconda/install/)

Conda permet de créer des environnements comparables à travers différents systèmes d’exploitation.

### 2. Créer un environnement conda avec python 3.10

Ouvrir un terminal et exécuter la commande suivante :

```bash
conda install -n py python=3.10
```

Par la suite, l'environnement devra être activé à chaque session, en tapant:

```bash
conda activate py
```

### 3. Préinstaller des paquets python avec pip

Une fois l'environnement conda activé, nous pouvons installer des "paquets" python qui permettent d'étendre les fonctionnalités de base du langage. Pour cela, nous utilisons le gestionnaire de paquets python "pip".

Vous pouvez d'ores-et-déjà installer les paquets, qui seront nécessaires pour reproduire les exemples du cours:

```bash
pip install numpy pandas fastparquet scipy networkx bertopic notebook matplotlib
```

### 4. Télécharger les données du cours



