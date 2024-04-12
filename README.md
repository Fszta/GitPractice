# Tp Git

## 1 - Initialisation du projet

### 1.1 - Création d'un projet 

Créer un nouveau projet github `tp-git` comme sur le screenshot ci-dessous :
- Cocher `Add a README.md`
- Sélectionner `.gitignore template : Python`

<img width="872" alt="Capture d’écran 2024-04-12 à 10 50 28" src="https://github.com/Fszta/GitPractice/assets/36471574/9742e047-c5c0-41e9-a211-90466e68fba7">

### 1.2 - Clôner le répertoire git localement
Une fois le projet github créé, récupérez l'url de votre projet pour le clôner localement : 


<img width="406" alt="Capture d’écran 2024-04-12 à 10 59 26" src="https://github.com/Fszta/GitPractice/assets/36471574/df285ed7-74ca-4ab4-ac96-d4c602c959f9">

- **Depuis un terminal** clôner votre projet: `git clone url_de_votre_projet.git` (Remplacez url_de_votre_projet.git par l'url précédemment copiée - cf screenshot)
- **Ouvrez le projet dans votre IDE (pycharm, vscode...)**

#### Appelez votre encadrant pour validation.


### 1.3 - Ajouter des fichiers à votre projets
Depuis votre ide, créez les trois fichiers (vide pour le moment) suivants :
- calculator.py
- main.py
- test_calculator.py


Votre projet local doit avoir la structure suivante : 
```bash
├── .gitignore
├── README.md
├── calculator.py
├── main.py
└── test_calculator.py
```


Vous devez maintenant "pusher" ces trois nouveaux fichiers vers le répertoire git distant.
Pour rappel, vous devez réaliser trois commandes pour obtenir le résultat escompter :
- `git add votre_fichier` - Ajoute le fichier à la zone de staging
- `git commit -m "Un message descriptif de votre commit"` 
- `git push origin main` - Pousse les modifications vers le répertoire distant 

> N'oubliez pas de remplacer `votre fichier` & `Un message descriptif de votre commit`..

Vous pouvez vérifier le bon fonctionnement en vous rendant sur votre projet github, qui doit maintenant contenir les commits, et donc les fichiers précédemment ajoutés.

#### Appelez votre encadrant pour validation.

## 2 - Les branches
L'objectif du tp n'est pas de tester votre capacité à coder, néanmoins il est nécessaire d'implémenter quelques fonctions pour la bonne réalisation du tp.

Vous allez créer une calculette (en python), supportant 3 opérations : 
- addition
- soustraction
- division

> Pour l'implémentation de chaque opération, vous devrez créer une branche dédiée.

### 2.1 - Fonctionnalité addition

**Rappel**
- Pour créer une branche et se "déplacer" dessus : `git checkout -b nom_de_la_branche`
- Pour simplement changer de branche : `git checkout nom_de_la_branche`
<hr>


- Depuis votre ide, créez une branche nommée `feat/addition`

- Dans le fichier `calculator.py` : implémentez la fonction addition prennant en paramètres deux nombres, et retournant un nombre

```python
def addition(a, b):
  ...
  return result

```


- Pousser les modifications vers le répertoire distant (add, commit, push ... cf partie 1.3. Attention, le nom de votre branche n'est plus `main` mais `feat/addition`)

- Sur github, créer une pull request pour intégrer les modifications dans votre branche principale (main)
<img width="927" alt="Capture d’écran 2024-04-12 à 11 47 59" src="https://github.com/Fszta/GitPractice/assets/36471574/e53f2f24-ab02-4303-b9a1-e35ec0bd0249">

- Valider la pull request pour intégrer les modifications dans votre branche principale (main)
<img width="933" alt="Capture d’écran 2024-04-12 à 11 53 15" src="https://github.com/Fszta/GitPractice/assets/36471574/ff5fa868-4881-435c-934b-dc32ca45c8a4">


#### Appelez votre encadrant pour validation.

### 2.2 - Fonctionnalité soustraction

Comme dans la partie précédente, implémentez la fonctionnalité de soustraction via une branche `feat/substraction`.

**Attention** avant de créer la branche, vous devez : 
- Vous déplacer sur la branche main : `git checkout main`
- Récupérer les modifications du répertoire distant (ce qui a été mergé précédemment) : `git pull origin main`

#### Appelez votre encadrant pour validation.

### 2.3 - Fonctionnalité division

Comme dans la partie précédente, implémentez la fonctionnalité de division via une branche `feat/division`

**Attention** avant de créer la branche, vous devez : 
- Vous déplacer sur la branche main : `git checkout main`
- Récupérer les modifications du répertoire distant (ce qui a été mergé précédemment) : `git pull origin main`

#### Appelez votre encadrant pour validation.


## 3 - Continuous integration pipeline
Dans cette partie, vous allez implémenter un pipeline de CI basique contenant deux étapes : 
- Execution automatique d'un linter (Utililaire visant à contrôler que les conventions de développement sont bien respectées - Style du code)
- Execution automatique de tests unitaires

### 3.1 Configuration du linter
Pour cette étape, vous allez utiliser `pylint`.

Github fournit un template pré-configuré permettant d'executé pylint dès qu'une modification est faite sur votre projet.



### 3.2 Execution automatique des tests unitaires
