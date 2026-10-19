# Projet L2 — Traitement géométrique des images et compression JPEG

## Démarche

Pour ce projet informatique sur le _traitement géométrique des images et la compression jpeg_, vous êtes guidé par 8 notebooks jupyter.

Chaque notebook, un par semaine, introduit de façon succincte quelques notions importantes, des exercices simples pour les assimiler puis définit du travail personnel d'approfondissement -- travail qui correspond à environ 2 heures hebdomadaire supplémentaires.  
La démarche attendue est une recherche (par exemple via wikipedia) des compléments nécessaires à une compréhension suffisante pour réaliser le travail personnel d'approfondissement.

Les notions abordées chaque semaine constituent une "étape" du projet global. 
Un "livrable" d'étape est défini dans chaque notebook.
Deux sujets de projets sont proposés en fin du dernier notebook.
Vous disposez de deux semaines pour réaliser ce projet.

## Contrôle de connaissance

En fin de semestre, votre travail est évalué lors d'un oral individuel (semaine des examens fin décembre ou début janvier) dont les modalités seront précisées en fin de séquence (fin novembre).

## Progression pédagogique

1. Représentation et inspection d’images
2. Transformations affines et composition
3. Interpolation et transformation inverse
4. Convolution et filtres
5. DCT par blocs
6. Quantification, MSE et PSNR
7. Comparaison avec JPEG via Pillow
8. Finalisation et restitution

Durée : 8 séances de 3 h, avec environ 2 h de travail personnel hebdomadaire.

## Supports

- `seance_01.ipynb` : images numériques et tableaux
- `seance_02.ipynb` : transformations affines
- `seance_03.ipynb` : rééchantillonnage et interpolation
- `seance_04.ipynb` : convolution et filtrage
- `seance_05.ipynb` : DCT
- `seance_06.ipynb` : quantification et distorsion
- `seance_07.ipynb` : JPEG réel et évaluation
- `seance_08.ipynb` : validation et sujets de projet

## Installation et lancement de jupyter

### A utiliser : moodle et anaconda

- Les notebooks hebdomadaires (seance_0x.ipynb) ainsi que les ressources nécessaires sont sur l'espace moodle de cette UE. 
- Sur les machines de l'UPVD, python et jupyter (lab) sont accesibles par le navigateur anaconda.

### Optionnel : github et uv

- cloner le dépôt github dans un répertoire de votre choix :
```bash
git clone https://github.com/phillanglois/L2-ProjetInfo.git
```
- vérifier que le fichier `pyproject.toml` est présent dans ce répertoire (de travail). Ce fichier  définit la configuration pour le gestionnaire d'environnement `uv`
- le premier lancement de `uv run` créera automatiquement l'environnement python avec les ressources nécessaires au projet. Un fichier `uv.lock` et des répertoires `.venv` et `src` seront ajoutés à votre répertoire de travail. Ne vous en occupez pas.
- il est utile de travailler avec `jupyter`, ce qui s'obtient en exécutant :
```bash
uv run --with jupyter jupyter lab
``` 
Ainsi votre session jupyter a accès à l'ensemble des ressources de l'environnement.

Bon travail.
