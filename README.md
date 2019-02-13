# Parkinson-Speech-Dataset-with-Multiple-Types-of-Sound-Recordings
Python for data-science  
Devoir à la maison  
Date de rendu : 15 février 2019

## 1) Rappel des consignes 

### L’objet du devoir est de mettre en pratique les différentes compétences nécessaires au métier de data-scientist, vues en cours cette année :
*Data-visualisation  
*Modélisation  
*Usage de Git

### Une base de donnée distincte est affectée à chaque étudiant du cours selon le fichier excel joint. Chacun doit :
*Créer un script python qui automatise toute la procédure de modélisation de la base de données :  
`*Téléchargement du fichier de données à la main.`  
`*Data-visualisation des données (via matplotlib, seaborn ou bokeh …)`  
`*Data-préparation (pandas)`  
`*Modélisation (scikit learn)`  
`*Optimisation des hyperparamètres (grid search)`  
`*Visualisation des performance (courbe roc …)`  

### Le résultat attendu est en plusieurs points :
*Un repository github pour la partie modélisation  
`*Doit avoir :`  
`*Du code propre, commenté et fonctionnel`  
`*Un fichier readme expliquant le contexte, et les objectifs`  
*Un ppt :  
`*Présenter l’analyse descriptive des données dans un powerpoint qui explique le contexte de la base de donnée, la cible à prédire, les différentes features disponibles, les étapes de récupération de données, de features engeneering, les tests des différentes hyper paramètres, et les gains de performance des différents modèles.`  
`*Le nom du ou des élèves`  
`*Ce fichier ppt doit être dans le github`  

## 2) Informations sur le jeu de données : [Dataset et description](https://archive.ics.uci.edu/ml/datasets/Parkinson+Speech+Dataset+with++Multiple+Types+of+Sound+Recordings)

### i) Introduction
La maladie de Parkinson est une maladie neurodégénérative d'étiologie inconnue. Au cours de son parcours, elle provoque une déficience vocale chez environ 90% des patients. Les patients atteints de la maladie souffrent de dysarthrie hypokinétique, qui se manifeste dans tous les aspects de la production de la parole: respiration, phonation, articulation, nasalité et prosodie. Pour les évaluer, les cliniciens ont adopté des méthodes perceptuelles, basées sur des signaux acoustiques, permettant de distinguer différents états pathologiques. Afin d'améliorer ces évaluations, dans ce jeu de données, ils ont utilisé une variété d'échantillons de voix comprenant les nombres de 1 à 10, quatre phrases rimées, neuf mots turcs plus les voyelles maintenues «a», «o» et «u». Des échantillons ont été prélevés chez 40 personnes, dont 20 atteintes de la maladie.  

*La cible à prédire est l’échelle UPDRS (Unified Parkinson Disease Rating Scale)  
*L’UPDRS (échelle d’évaluation unifiée pour la maladie de Parkinson), est une méthode efficace d’évaluation, très employée à travers le monde.  
*Elle est simple, globale, et n’utilise pas d’appareillages de mesure pour évaluer le handicap et ne fait appel qu’à l’expérience du neurologue.

### ii) Database

La base de données PD comprend des fichiers de formation et de test. Les données de formation concernent 20 PWP (6 femmes et 14 hommes) et 20 personnes en bonne santé (10 femmes et 10 hommes) qui ont interjeté appel au département de neurologie de la faculté de médecine de Cerrahpasa de l’Université d’Istanbul. De tous les sujets, plusieurs types d’enregistrements sonores (26 échantillons de voix, y compris des voyelles, des nombres, des mots et des phrases courtes) sont effectués. Un groupe de 26 entités linéaires et temporelles est extrait de chaque échantillon vocal. Le score UPDRS ((Unified Park Disease Rating Scale) de chaque patient déterminé par un médecin expert est également disponible dans cet ensemble de données. Cet ensemble de données peut donc également être utilisé pour la régression.  

Après avoir collecté le jeu de données de formation qui comprend plusieurs types d’enregistrements sonores et effectué nos expériences, conformément aux résultats obtenus, nous avons continué à collecter un jeu de tests indépendant à partir de PWP via le même processus d’examen du médecin dans les mêmes conditions. Lors de la collecte de cet ensemble de données, il est demandé à 28 patients PD de ne déclarer que les voyelles maintenues «a» et «o» trois fois, soit un total de 168 enregistrements. Les mêmes 26 caractéristiques sont extraites d'échantillons vocaux de cet ensemble de données. Cet ensemble de données peut être utilisé comme un ensemble de test indépendant pour valider les résultats obtenus sur un ensemble de formation.  

> Further details are contained in the following reference -- if you use this dataset, please cite: Erdogdu Sakar, B., Isenkul, M., Sakar, C.O., Sertbas, A., Gurgen, F., Delil, S., Apaydin, H., Kursun, O., 'Collection and Analysis of a Parkinson Speech Dataset with Multiple Types of Sound  Recordings', IEEE Journal of Biomedical and Health Informatics, vol. 17(4), pp. 828-834, 2013 

### 3) L'application

Pour répondre à la problématique, nous avons crée un script python qui automatise toute la procédure de modélisation de la base de données :  

1. Lancer [Jupiter](https://jupyter.org/install)  
2. Ouvrir un nouveau fichier script  
3. Copier la commande `git clone https://github.com/cjacques4/Parkinson-Speech-Dataset-with-Multiple-Types-of-Sound-Recordings` et lancer l'execution  
4. Retournez dans l'arborescence et allez dans le dossier `Parkinson Speech Dataset with Multiple Types of Sound Recordings Data Set`.  
5. Ouvrez le script `Projet_Python_DataAnalysis.ipynb`
