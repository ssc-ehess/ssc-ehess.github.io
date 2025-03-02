---
layout: page
permalink: /datasets/
title: Datasets
description: Présentation des datasets sur lesquels s'appuie le cours.
nav: true
nav_order: 3
toc:
  sidebar: left
---

## 1. Science

Nous proposons deux datasets issus de données extraites de <a href="https://openalex.org/">OpenAlex</a>. 
Chacun des datasets recense les articles (titre, abstract, références), auteurs, affiliations d'un corpus de littérature scientifique.

### 1.1 Climat (2015-2025)

Ce jeu de données couvre la littérature scientifique sur le climat de 2015 à 2025. Il comprend environ 200.000 articles.

#### Téléchargement manuel

 - Téléchargement rapide [ici](https://scc-ehess-science.s3.eu-west-1.amazonaws.com/MD5E-s766794240--862572f2ed4d98c4ba32f4993f19419e.tar).
 - Téléchargement lent (backup) [ici](https://gin.g-node.org/lucasgautheron/science/raw/master/climate.tar).

#### Téléchargement automatique

Pour télécharger le corpus automatiquement installez les notebooks (comme expliqué [ici](preparations/#4-télécharger-les-notebooks-et-données-du-cours)), puis exécutez la commande suivante:

```bash
datalad get science/climate -s s3
```

### 1.2 Sciences économiques (2019-2025)

> ##### Attention
>
> Ce jeu de données est relativement lourd. 
> Prévoir 2 Go d'espace disque, et 8 Go de mémoire vive au minimum.
> Dans le cas contraire, privilégiez les autres datasets.
{: .block-warning }

Ce jeu de données couvre la littérature scientifique en économie de 2019 à 2025. Il comprend environ 600.000 articles.

Pour télécharger le corpus automatiquement, installez les notebooks (comme expliqué [ici](preparations/#4-télécharger-les-notebooks-et-données-du-cours)), puis exécutez la commande suivante:

```bash
datalad get science/econ
```

---

### 2. Impact investing (twitter)


#### Téléchargement manuel

 - Téléchargement des graphes (RT) [ici](https://gin.g-node.org/lucasgautheron/twitter/raw/master/retweet-graphs.zip)

#### Téléchargement automatique

Pour télécharger le corpus automatiquement, installez les notebooks (comme expliqué [ici](preparations/#4-télécharger-les-notebooks-et-données-du-cours)), puis exécutez la commande suivante:

```bash
datalad get science/climate -s s3
```