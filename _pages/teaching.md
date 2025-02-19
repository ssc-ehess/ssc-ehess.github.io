---
layout: page
permalink: /preparations/
title: Préparations
nav: true
nav_order: 2
toc:
  sidebar: left
---

## Préparer son environnement de programmation

### 1. Installer anaconda

Conda permet de créer des environnements comparables à travers différents systèmes d’exploitation.
Pour l'installer, suivez les instructions ci-dessous, en fonction de votre système d'exploitation (windows, mac, linux):

[https://docs.anaconda.com/anaconda/install/](https://docs.anaconda.com/anaconda/install/)


### 2. Créer un environnement conda avec python 3.10

Ouvrez un terminal (sous windows, via anaconda) et exécutez la commande suivante :

```bash
conda install -n py python=3.10
```

Par la suite, l'environnement devra être activé à chaque session, en tapant:

```bash
conda activate py
```

### 3. Préinstaller des paquets python avec pip

Une fois l'environnement conda activé, vous pouvez installer des "paquets" python qui étendent les fonctionnalités de base du langage. Pour cela, nous utilisons le gestionnaire de paquets python "pip".

Vous pouvez d'ores-et-déjà installer les paquets, qui seront nécessaires pour reproduire les exemples du cours:

```bash
pip install numpy pandas fastparquet scipy networkx bertopic notebook matplotlib
```

### 4. Télécharger les données du cours





