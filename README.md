# heart-attack
À propos de l'ensemble de données
Cet ensemble de données sur « Soins de santé : Ensemble de données sur la possibilité d'une crise cardiaque » Publié à l'origine à Kaggle : Heart Disease UCI
Cette base de données contient 76 attributs, mais toutes les expériences publiées se réfèrent à l'utilisation d'un sous-ensemble de 14 d'entre eux. En particulier, la base de données de Cleveland est la seule qui a été utilisée par les chercheurs en ML à
ce jour.
Le champ « objectif » fait référence à la présence d'une maladie cardiaque chez le patient. Il s'agit d'un entier dont la valeur va de 0 (aucune présence) à 4. 
Leq noms et numéros de sécurité sociale des patients ont été récemment supprimés de la base de données, remplacés par des valeurs fictives.


# Attribut d'intérêt
1) âge
2) sexe
3) type de douleur thoracique (4 valeurs)
4) tension artérielle au repos
5) cholestérol sérique en mg/dl
6) glycémie à jeun > 120 mg/dl
7) résultats électrocardiographiques au repos (valeurs 0,1 ,2)
8) fréquence cardiaque maximale atteinte
9) angor
induit par l'exercice 10) oldpeak = dépression du segment ST induite par l'exercice par rapport au repos
11) la pente du segment ST d'exercice maximal
12) nombre de vaisseaux principaux (0-3) colorés par fluoroscopie
13) thal : 0 = normal ; 1 = défaut corrigé ; 2 = défaut réversible
14) cible : 0= moins de chance de crise cardiaque 1= plus de chance de crise cardiaque



# Documentation complète de l'attribut :

id : numéro d'identification du patient

ccf : numéro de sécurité sociale (je l'ai remplacé par une valeur fictive de 0)

age : âge en années

sexe : sexe (1 = masculin ; 0 = féminin)

painloc : localisation de la douleur thoracique (1 = sous-sternal ; 0 = autrement)

painexer (1 = provoqué par l'effort ; 0 = autrement)

relrest (1 = soulagé après le repos ; 0 = sinon)

8 pncaden (somme de 5, 6 et 7)
9 cp : type de douleur thoracique
-- Valeur 1 : angine typique
-- Valeur 2 : angine atypique
-- Valeur 3 : douleur non angineuse
-- Valeur 4 : asymptomatique
10 trestbps : tension artérielle au repos (en mm Hg à l'admission à l'hôpital)
11 htn
12 chol : cholestérol sérique en mg/dl
13 fumée : je crois que c'est 1 = oui ; 0 = non (est ou n'est pas fumeur)
14 cigs (cigarettes par jour)
15 ans (nombre d'années en tant que fumeur)
16 fbs : (glycémie à jeun > 120 mg/dl) (1 = vrai ; 0 = faux)
17 dm (1 = antécédent de diabète ; 0 = pas d'antécédents)
18 famhist : antécédents familiaux de maladie coronarienne (1 = oui ; 0 = non)
19 restecg : résultats électrocardiographiques au repos
-- Valeur 0 : normal
-- Valeur 1 : présentant une anomalie de l'onde ST-T (inversions de l'onde T et /ou Élévation ou dépression du segment ST > 0,05 mV)
-- Valeur 2 : montrant une hypertrophie ventriculaire gauche probable ou certaine selon les critères d'Estes
20 ekgmo (mois de lecture ECG d'effort)
21 ekgday (jour de lecture ECG d'effort)
22 ekgyr (année de lecture de l'ECG d'effort)
23 dig (digital utilisé sur l'ECG d'exercice furing : 1 = oui ; 0 = non)
24 prop (Bêta-bloquant utilisé pendant l'ECG d'effort : 1 = oui ; 0 = non)
25 nitr (nitrates utilisés pendant ECG d'effort : 1 = oui ; 0 = non)
26 pro (inhibiteur calcique utilisé pendant l'ECG d'effort : 1 = oui ; 0 = non)
27 diurétique (diurétique utilisé pendant l'ECG d'effort : 1 = oui ; 0 = non)
28 proto : protocole d'exercice
1 = Bruce
2 = Kottus
3 = McHenry
4 = rapide Balke
5 = Balke
6 = Noughton
7 = vélo 150 kpa min/min (Je ne sais pas si "kpa min/min" est ce qui était écrit !)
8 = vélo 125 kpa min/min
9 = vélo 100 kpa min/min
10 = vélo 75 kpa min/min
11 = vélo 50 kpa min/min
12 = ergomètre bras
29 thaldur : durée de l'épreuve d'effort en minutes
30 thaltime : heure à laquelle Une dépression de la mesure ST a été notée
31 atteinte : mets atteints
32 thalach : fréquence cardiaque maximale atteinte
33 thalrest : fréquence cardiaque au repos
34 tpeakbps : pic de la pression artérielle à l'effort (première des 2 parties)
35 tpeakbpd : pic de la pression artérielle à l'effort (deuxième des 2 parties)
36 mannequin
37 trestbpd : tension artérielle au repos
38 exang : angine d'effort (1 = oui ; 0 = non)
39 xhypo : (1 = oui ; 0 = non)
40 oldpeak = dépression du segment ST induite par l'exercice par rapport au repos
41 pente : la pente du segment ST à l'exercice de pointe
-- Valeur 1 : montante
-- Valeur 2 : plat
-- Valeur 3 : descente
42 rldv5 : hauteur au repos
43 rldv5e : hauteur à l'exercice de pointe
44 ca : nombre de vaisseaux principaux (0-3) colorés par la fluoroscopie
45 restckm : non pertinent
46 exerckm : non pertinent
47 restef : repos raidonuclid (sp?) fraction d'éjection
48 restwm : anomalie du mouvement de la paroi du repos (sp?)
0 = aucune
1 = légère ou modérée
2 = modérée ou sévère
3 = akinésie ou dyskmem (sp?)
49 exeref: exercice radinalid (sp?) fraction d'éjection
50 exerwm: exercice mur (sp?) mouvement
51 thal: 3 = normal; 6 = défaut corrigé ; 7 = défaut réversible
52 thalsev : non utilisé
53 thalpul : non utilisé
54 lobe de l'oreille : non utilisé
55 cmo : mois du cathéter cardiaque (sp?) (peut-être "appel")
56 cday : jour du cathéter cardiaque (sp?)
57 cyr : année de cathétérisme cardiaque (sp?)
58 num : diagnostic de maladie cardiaque (statut de la maladie angiographique)
-- Valeur 0 : rétrécissement de diamètre < 50 %
-- Valeur 1 : rétrécissement de diamètre > 50 %
(dans tout vaisseau majeur : attributs 59 à 68 sont des navires)
59 lmt
60 ladprox
61 laddist
62 diag
63 cxmain
64 ramus
65 om1
66 om2
67 rcaprox
68 rcadist
69 lvx1 : non utilisé
70 lvx2 : non utilisé
71 lvx3 : non utilisé
72 lvx4 : non utilisé
73 lvf : non utilisé
74 cathef : non utilisé
75 junk : non utilisé
76 nom : nom de famille du patient (je l'ai remplacé par la chaîne factice "nom")

# Quelques questions

Quelles sont la plupart des raisons pour la possibilité d'une crise cardiaque?
Quels sont les groupes d'âge les plus nombreux pour la crise cardiaque?
Quelles sont les principales causes des crises cardiaques?

L'ensemble de données est pris à des fins d'apprentissage. 

# Source des données : 
https://archive.ics.uci.edu/ml/datasets/Heart+Disease

# Créateurs :

1. Institut hongrois de cardiologie. Budapest : Andras Janosi, MD
2. Hôpital universitaire, Zurich, Suisse : William Steinbrunn, MD
3. Hôpital universitaire, Bâle, Suisse : Matthias Pfisterer, MD
4. VA Medical Center, Long Beach et Cleveland Clinic Foundation : Robert Detrano, MD, doctorat

# Donateur :

David W. Aha ( aha '@' ics.uci.edu ) (714) 856-8779




# Quelques articles citant cet ensemble de données 1 :


Remco R. Bouckaert et Eibe Frank. Évaluation de la réplicabilité des tests de signification pour la comparaison des algorithmes d'apprentissage . PAKDD. 2004. 

Xiaoyong Chai et Li Deng et Qiang Yang et Charles X. Ling. Classification naïve de Bayes sensible aux coûts . ICDM. 2004. 

Gavin Brown. Diversité dans les ensembles de réseaux de neurones . L'Université de Birmingham. 2004. 

Kaizhu Huang et Haiqin Yang et Irwin King et Michael R. Lyu et Laiwan Chan. Machine de probabilité Minimax biaisée pour le diagnostic médical . AMAI. 2004. 

Jeroen Eggermont et Joost N. Kok et Walter A. Kosters. Programmation génétique pour la classification des données : partitionnement de l'espace de recherche . SAC. 2004.

Zhi-Hua Zhou et Yuan Jiang. NeC4.5 : basé sur un ensemble de neurones C4.5 . IEEE Trans. Savoir. Data Eng, 16. 2004.


# Demande de citation :

Les auteurs des bases de données ont demandé que toutes les publications résultant de l'utilisation des données incluent les noms du chercheur principal responsable de la collecte des données dans chaque établissement. Ils seraient :
1. Institut hongrois de cardiologie. Budapest : Andras Janosi, MD
2. Hôpital universitaire, Zurich, Suisse : William Steinbrunn, MD
3. Hôpital universitaire, Bâle, Suisse : Matthias Pfisterer, MD
4. VA Medical Center, Long Beach et Cleveland Clinic Foundation : Robert Detrano, MD, doctorat
