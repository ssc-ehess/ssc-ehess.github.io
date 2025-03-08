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

Ouvrez un terminal (sous windows, via anaconda [^1]) et exécutez la commande suivante :

```bash
conda create --name py python=3.10
```

Par la suite, l'environnement devra être activé à chaque session, en tapant:

```bash
conda activate py
```

---

### 3. Préinstaller des paquets python avec pip

Une fois l'environnement conda activé, vous pouvez installer des "paquets" python qui étendent les fonctionnalités de base du langage. Pour cela, nous utilisons le gestionnaire de paquets python "pip".

Vous pouvez d'ores-et-déjà installer les paquets, qui seront nécessaires pour reproduire les exemples du cours:

```bash
pip install numpy pandas fastparquet scipy networkx bertopic notebook matplotlib datalad
```

---

### 4. Installer Gephi

Téléchargez et installer [gephi](https://gephi.org/), une interface graphique pour la visualisation de réseaux.

### 5. Télécharger les notebooks et données du cours

Vous pouvez installer les notebooks ainsi:

```bash
git clone https://github.com/ssc-ehess/notebooks.git
```

Pour les données, il y a deux approches:

a. Le téléchargement manuel
b. Le téléchargement automatique

#### a. Téléchargement manuel

1. Téléchargez la ou les archives souhaitées depuis la page des datasets: [ssc-ehess.github.io/datasets/](https://ssc-ehess.github.io/datasets/).
2. Placez les dans le dossier "notebooks".
3. Extrayez l'archive dans le dossier notebooks. 

#### b. Téléchargement automatique

Installez `datalad', qui permet de téléchargement facilement les données du cours:

```bash
conda install -c conda-forge datalad
```

Depuis le dossier contenant les notebooks, tapez:

```bash
datalad install science
```

Cela ne télécharge pas automatiquement toutes les données, qui prennent un peu de place. Si vous souhaitez utiliser le dataset climat, par exemple, faites:

```bash
datalad get science/climate -s s3
```


---

### 5. Ouvrir les notebooks

Pour lancer un notebook:

1. Ouvrir le terminal
2. Placez vous dans le répertoire notebooks (e.g. `cd notebooks`). [Pour connaître votre position dans l'arborescence: `pwd`]
3. Exécutez la commande:
```bash
jupyter notebook
```
4. Un onglet va s'ouvrir dans votre navigateur. Vous pourrez alors ouvrir le notebook de votre choix.

> ##### TIP
>
> N'oubliez pas de mettre régulièrement vos notebooks à jour en tapant
> `git pull` dans le terminal.
{: .block-tip }

---

[^1]: Pour lancer le terminal Anaconda sous windows, appuyez sur les touches (Win + S), et tapez "Anaconda Prompt" (d'après ChatGPT...).