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

#### Appelez votre tuteur pour validation.


### 1.3 - Ajouter des fichiers à votre projets
Depuis votre ide, créez les trois fichiers (vide pour le moment) suivants :
- calculator.py
- main.py
- test_calculator.py


Votre projet doit avoir la structure suivante : 
```bash
├── .gitignore
├── README.md
├── calculator.py
├── main.py
└── test_calculator.py
```


Vous devez maintenant "pusher" ces trois nouveaux fichiers vers le répertoire git distant.
Pour rappel, vous devez réaliser trois commandes pour obtenir le résultat escompter : 
