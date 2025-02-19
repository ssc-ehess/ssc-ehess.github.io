---
layout: page
permalink: /preparations/
title: Préparations
description: Préparer son environnement de programmation
nav: true
nav_order: 2
toc:
  sidebar: left
---


### 1. Installer anaconda

Conda permet de créer des environnements comparables à travers différents systèmes d’exploitation.
Pour l'installer, suivez les instructions ci-dessous, en fonction de votre système d'exploitation (windows, mac, linux):

[https://docs.anaconda.com/anaconda/install/](https://docs.anaconda.com/anaconda/install/)

---

### 2. Créer un environnement conda avec python 3.10

Ouvrez un terminal (sous windows, via anaconda <footnote>Pour lancer le terminal Anaconda, appuyez sur les touches (Win + S), et tapez "Anaconda Prompt" (d'après ChatGPT...).</footnote>) et exécutez la commande suivante :

```bash
conda install -n py python=3.10
```

Par la suite, l'environnement devra être activé à chaque session, en tapant:

```bash
conda activate py
```

Enfin, installez `datalad', qui permet de téléchargement facilement les données du cours:

```bash
conda install datalad
```

---

### 3. Préinstaller des paquets python avec pip

Une fois l'environnement conda activé, vous pouvez installer des "paquets" python qui étendent les fonctionnalités de base du langage. Pour cela, nous utilisons le gestionnaire de paquets python "pip".

Vous pouvez d'ores-et-déjà installer les paquets, qui seront nécessaires pour reproduire les exemples du cours:

```bash
pip install numpy pandas fastparquet scipy networkx bertopic notebook matplotlib datalad
```

---

### 4. Télécharger les notebooks et données du cours

Enfin, vous pouvez installer les notebooks (exemples) et datasets du cours en une commande:

```bash
datalad install -r https://github.com/ssc-ehess/notebooks.git
```

Cela ne télécharge pas automatiquement toutes les données, qui prennent un peu de place. Si vous souhaitez utiliser le dataset climat, par exemple, faites:

```bash
cd notebooks
datalad get science/climate
```



