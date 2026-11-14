# Projet L2 — Traitement géométrique des images et compression JPEG

## Démarche

Pour ce projet informatique sur le _traitement géométrique des images et la compression jpeg_, vous êtes guidé par 8 notebooks jupyter.

Chaque notebook, un par semaine, introduit de façon succincte quelques notions importantes, des exercices simples pour les assimiler puis définit du travail personnel d'approfondissement -- travail qui correspond à environ 2 heures hebdomadaire supplémentaires.  
La démarche attendue est une recherche (par exemple via [wikipedia](fr.wikipedia.org)) des compléments nécessaires à une compréhension suffisante pour réaliser le travail personnel d'approfondissement.

Les notions abordées chaque semaine constituent une "étape" du projet global. 
Un "livrable" d'étape est défini dans chaque notebook.
Deux sujets de projets sont proposés en fin du dernier notebook.
Vous disposez de deux semaines en autonomie pour réaliser ce projet.

## Votre notebook projet

Votre travail de projet est _un_ notebook. 

**Ce notebook doit pouvoir être excuté entièrement sans erreur, ni intervention de l'utilisateur ("Redemmarage du noyau et exécution de la totalité des cellules").**
Le résultat de cette exécution sera la première démonstration possible de oral.

Votre notebook commencera par :

- une présentation synthétique de son organisation ;
- la démarche que doit suivre un _utilisateur_ (pas vous) pour être exécuté sur d'autres exemples que celui de la démonstration ;
- les éventuelles faiblesses ou problèmes non résolus du travail rendu.

Il se terminera par un "rapport" organisé en quatre sections -- comme pour les rapports intermédiaires : 

- en _quelques phrases_, qu'avez-vous appris ?
- quelles difficultés avez-vous éventuellement rencontrées ?
- qu'avez vous aimé ou moins aimé dans cette série de séances ?
- et des notes et commentaires libres.


## Contrôle de connaissance 

En fin de semestre, votre travail est évaluée en deux temps :
- lors d'un oral _individuel_ (semaine des examens fin décembre ou début janvier) dont les modalités pratiques seront précisées en fin de séquence (fin novembre) ; 
- par relecture du code de votre projet.


### Oral individuel : objectifs

Pendant cet oral, vous ferez brièvement la démonstration de vos résultats.
Vous mentionnerez les faiblesses ou problèmes non résolus de votre code. 
Puis vous serez interrogés sur le code rendu.
Cet échange permettra _d'évaluer_ : 

* à quel point vous avez compris le sujet ;
* jusqu'où vous avez abordé le sujet ;
* si vous êtes capables de commenter vos choix et de les analyser ;
* si vous êtes bien approprié le code rendu ;
* si les contributions dans le binôme sont équilibrées.

### Le code du projet : relecture 

Le code de votre projet (votre notebook) sera ensuite relu (sans vous). 
Le correcteur évaluera les points suivants.

Votre notebook :

* s'exécute sans erreur sur la démonstration proposée,
* s'exécute sans erreur sur un autre cas choisi par le correcteur,
* intègre des tests pour l'intégralité des étapes du traitement,
* permet de charger une situation initiale différente de celle de la démontration,
* permet de trouver une solution.

Le code est clair, bien structuré et documenté :

* nommage clair des fonctions et variables,
* bon découpage des fonctions pour éviter la duplication de code,
* pas de fonctions trop longues,
* pas de lignes de code trop longues,
* des spécifications claires explicitées dans le 'docstring', 
* des commentaires utiles et courts tout au long du code.


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

- Les notebooks hebdomadaires (seance_0x.ipynb) ainsi que les ressources nécessaires sont disponibles ici et sur l'espace moodle de cette UE. 
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
