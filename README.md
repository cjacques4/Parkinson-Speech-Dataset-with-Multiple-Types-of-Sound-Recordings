# Parkinson-Speech-Dataset-with-Multiple-Types-of-Sound-Recordings
Python for data-science  
Devoir à la maison  
Date de rendu : 15 février 2019

## 1) Rappel des consignes 

#### L’objet du devoir est de mettre en pratique les différentes compétences nécessaires au métier de data-scientist, vues en cours cette année :
*Data-visualisation  
*Modélisation  
*Usage de Git

## Une base de donnée distincte est affectée à chaque étudiant du cours selon le fichier excel joint. Chacun doit :
*Créer un script python qui automatise toute la procédure de modélisation de la base de données :  
`*Téléchargement du fichier de données à la main.`  
`*Data-visualisation des données (via matplotlib, seaborn ou bokeh …)`  
`*Data-préparation (pandas)`  
`*Modélisation (scikit learn)`  
`*Optimisation des hyperparamètres (grid search)`  
`*Visualisation des performance (courbe roc …)`  

## Le résultat attendu est en plusieurs points :
*Un repository github pour la partie modélisation  
`*Doit avoir :`  
`*Du code propre, commenté et fonctionnel`  
`*Un fichier readme expliquant le contexte, et les objectifs`  
*Un ppt :  
`*Présenter l’analyse descriptive des données dans un powerpoint qui explique le contexte de la b ase de donnée, la cible à prédire, les différentes features disponibles, les étapes de récupération de données, de features engeneering, les tests des différentes hyper paramètres, et les gains de performance des différents modèles.`  
`*Le nom du ou des élèves`  
`*Ce fichier ppt doit être dans le github`  

## Informations sur le jeu de données:

##### La base de données PD comprend des fichiers de formation et de test. Les données de formation concernent 20 PWP (6 femmes et 14 hommes) et 20 personnes en bonne santé (10 femmes et 10 hommes) qui ont interjeté appel au département de neurologie de la faculté de médecine de Cerrahpasa de l’Université d’Istanbul. De tous les sujets, plusieurs types d’enregistrements sonores (26 échantillons de voix, y compris des voyelles, des nombres, des mots et des phrases courtes) sont effectués. Un groupe de 26 entités linéaires et temporelles est extrait de chaque échantillon vocal. Le score UPDRS ((Unified Park Disease Rating Scale) de chaque patient déterminé par un médecin expert est également disponible dans cet ensemble de données. Cet ensemble de données peut donc également être utilisé pour la régression. 

##### Après avoir collecté le jeu de données de formation qui comprend plusieurs types d’enregistrements sonores et effectué nos expériences, conformément aux résultats obtenus, nous avons continué à collecter un jeu de tests indépendant à partir de PWP via le même processus d’examen du médecin dans les mêmes conditions. Lors de la collecte de cet ensemble de données, il est demandé à 28 patients PD de ne déclarer que les voyelles prolongées «a» et «o» trois fois, soit un total de 168 enregistrements. Les mêmes 26 caractéristiques sont extraites d'échantillons vocaux de cet ensemble de données. Cet ensemble de données peut être utilisé comme un ensemble de test indépendant pour valider les résultats obtenus sur un ensemble de formation. 

##### échantillons - échantillons de voix correspondants 
##### 1: voyelle soutenue (aaa) 
##### 2: voyelle soutenue (ooo ...) 
##### 3: voyelle soutenue ( uuu ... ... 
##### 4-13: nombres de 1 à 10 
##### 14-17: phrases courtes 
##### 18-26: mots 

##### Fichier de données de test: 
##### Il est demandé à 28 patients PD de ne déclarer que les voyelles prolongées 'a' et 'o' trois fois, soit un total de 168 enregistrements (chaque sujet dispose de 6 échantillons vocaux). Les échantillons vocaux du fichier de données de test sont fournis. dans l'ordre suivant: 

##### sample # - échantillons de voix correspondants 
1-3: voyelle soutenue (aaa) 
4-6: voyelle soutenue (ooo) 


## Informations d'attribut:

##### Fichier de données de formation: 
##### colonne 1: identificateur de sujet 

##### colum 2-27: caractéristiques 
##### caractéristiques 1-5: gigue (locale), gigue (locale, absolue), gigue (rap), gigue (ppq5), gigue (ddp),  
##### caractéristiques 6- 11: Shimmer (local), Shimmer (local, dB), Shimmer (apq3), Shimmer (apq5), Shimmer (apq11), Shimmer (dda),  ##### caractéristiques 12-14: AC, NTH, HTN, 
##### caractéristiques 15-19: Pas moyen, Pas moyen, Écart-type, Pas minimum, Pas maximum, 
##### Caractéristiques 20-23: Nombre d'impulsions, Nombre de périodes, Période moyenne, Écart-type de période, 
##### Caractéristiques 24-26: Fraction de trames non localisées localement, Nombre de voix pauses, degré de pauses voix 

##### colonne 28: UPDRS 
##### colonne 29: informations sur la classe 

##### Fichier de données de test: 
##### colonne 1: identificateur de sujet 

##### colum 2-27: fonctionnalités 
##### caractéristiques 1-5: gigue (locale), gigue (locale, absolue), gigue (rap), gigue (ppq5), gigue (ddp), 
##### caractéristiques 6-11: Shimmer (locale), Shimmer (locale, dB), Shimmer (apq3), Shimmer (apq5), Shimmer (apq11), Shimmer (dda), 
##### caractéristiques 12-14: AC, NTH, HTN, 
##### caractéristiques 15-19: pitch médian, pitch moyen, écart-type, pitch minimum, pitch maximum, 
##### caractéristiques 20-23: nombre d'impulsions, nombre de périodes, période moyenne, déviation standard de la période, 
##### caractéristiques 24-26: fraction de trames non exprimées localement, nombre de coupures de voix, degré de rupture de voix, 

##### colonne 28: informations sur la classe 
