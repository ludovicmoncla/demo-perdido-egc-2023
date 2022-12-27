
<img src="https://egc2023.sciencesconf.org/data/pages/logo_2.jpg" alt="EGC 2023" width="200px"/>

# Démonstration - Perdido Geoparser - EGC 2023 


Cette démonstration s'appuie sur le tutoriel présenté lors de l'atelier [Librairies Python et Services Web pour la reconnaissance d’entités nommées et la résolution de toponymes](https://anf-tdm-2022.sciencesconf.org/resource/page/id/11) de la formation CNRS [ANF TDM 2022](https://anf-tdm-2022.sciencesconf.org).
Elle présente la librairie Python [Perdido](https://github.com/ludovicmoncla/perdido) pour le geoparsing et le geocoding de textes en français. Nous montrons en particulier comment utiliser `Perdido` pour la reconnaissance des entités nommées (*Named Entity Recognition*) et la résolution de toponymes (*Geocoding*). 

Nous expérimenterons le geoparsing et le geocoding au travers deux études de cas : le traitement d'articles encyclopédiques (corpus issu du projet [GEODE](https://geode-project.github.io)) et le traitement de descriptions de randonnées (corpus issu du projet [ANR CHOUCAS](http://choucas.ign.fr)).

**Auteurs** : [Ludovic Moncla](https://ludovicmoncla.github.io) (Univ Lyon, INSA Lyon, CNRS, UCBL, LIRIS, UMR 5205, F-69621)
[Mauro Gaio](https://lma-umr5142.univ-pau.fr/fr/organisation/membres/cv_-mgaio-fr.html) (Université de Pau et des Pays de l'Adour, CNRS, LMAP, UMR 5142)


### Tâches et problématiques abordées

 1. Reconnaissance et classification des entités nommées en français
 2. Créer et afficher une carte à partir d'un texte
 3. Résolution de toponymes (problématique de désambiguïsation)


Vous pouvez exécuter le notebook à distance en utilisant [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ludovicmoncla/demo-perdido-egc-2023/main?labpath=notebook-demo-perdido-egc.ipynb) ou [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](http://colab.research.google.com/github/ludovicmoncla/demo-perdido-egc-2023/blob/main/notebook-demo-perdido-egc.ipynb).
Sinon, pour exécuter ce tutoriel depuis un environnement local sur votre ordinateur, vous pouvez suivre les instructions ci-dessous. 


## Configurer un environnement Python

### Cloner ce dépôt git

```bash
git clone https://github.com/ludovicmoncla/demo-perdido-egc-2023.git
```

### Configurer l'environnement avec toutes les dépendances nécessaires


* Créer un nouvel environnement nommé `demo-perdido-egc-py39`

```bash
conda create -n demo-perdido-egc-py39 python=3.9
```

* Activer l'environnement

```bash
conda activate demo-perdido-egc-py39
```

* Installer le paquet `fiona` avec conda (évite une erreur lors de l'installation de cette dépendence avec `pip`)

```bash
conda install fiona==1.8.21
```

* Installer les dépendances avec `pip`

```bash
pip install -r requirements.txt
```


### Lancer le serveur Jupyter

```bash
jupyter notebook
```





