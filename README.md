# heart-attack
À propos de l'ensemble de données
Cet ensemble de données sur « Soins de santé : Ensemble de données sur la possibilité d'une crise cardiaque » Publié à l'origine à Kaggle : Heart Disease UCI
Cette base de données contient 76 attributs, mais toutes les expériences publiées se réfèrent à l'utilisation d'un sous-ensemble de 14 d'entre eux. En particulier, la base de données de Cleveland est la seule qui a été utilisée par les chercheurs en ML à
ce jour.
Le champ « objectif » fait référence à la présence d'une maladie cardiaque chez le patient. Il s'agit d'un entier dont la valeur va de 0 (aucune présence) à 4. 
Leq noms et numéros de sécurité sociale des patients ont été récemment supprimés de la base de données, remplacés par des valeurs fictives.


#Attribut d'intérêt 
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



Documentation complète de l'attribut :

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

#Quelques questions

Quelles sont la plupart des raisons pour la possibilité d'une crise cardiaque?
Quels sont les groupes d'âge les plus nombreux pour la crise cardiaque?
Quelles sont les principales causes des crises cardiaques?

L'ensemble de données est pris à des fins d'apprentissage. 

#Source des données : 
https://archive.ics.uci.edu/ml/datasets/Heart+Disease



Créateurs :

1. Institut hongrois de cardiologie. Budapest : Andras Janosi, MD
2. Hôpital universitaire, Zurich, Suisse : William Steinbrunn, MD
3. Hôpital universitaire, Bâle, Suisse : Matthias Pfisterer, MD
4. VA Medical Center, Long Beach et Cleveland Clinic Foundation : Robert Detrano, MD, doctorat

Donateur :

David W. Aha ( aha '@' ics.uci.edu ) (714) 856-8779





Articles citant cet ensemble de données 1 :


Remco R. Bouckaert et Eibe Frank. Évaluation de la réplicabilité des tests de signification pour la comparaison des algorithmes d'apprentissage . PAKDD. 2004. [ Voir le contexte ].

Xiaoyong Chai et Li Deng et Qiang Yang et Charles X. Ling. Classification naïve de Bayes sensible aux coûts . ICDM. 2004. [ Voir le contexte ].

Gavin Brown. Diversité dans les ensembles de réseaux de neurones . L'Université de Birmingham. 2004. [ Voir le contexte ].

Kaizhu Huang et Haiqin Yang et Irwin King et Michael R. Lyu et Laiwan Chan. Machine de probabilité Minimax biaisée pour le diagnostic médical . AMAI. 2004. [ Voir le contexte ].

Jeroen Eggermont et Joost N. Kok et Walter A. Kosters. Programmation génétique pour la classification des données : partitionnement de l'espace de recherche . SAC. 2004. [ Voir le contexte ].

Zhi-Hua Zhou et Yuan Jiang. NeC4.5 : basé sur un ensemble de neurones C4.5 . IEEE Trans. Savoir. Data Eng, 16. 2004. [ Voir le contexte ].

David Page et Soumya Ray. Inclinaison : une alternative efficace à l'anticipation pour l'induction de l'arbre de décision . IJCAI. 2003. [ Voir le contexte ].

Jinyan Li et Limsoon Wong. Utilisation de règles pour analyser les données biomédicales : une comparaison entre C4.5 et PCL . WAIM. 2003. [ Voir le contexte ].

Yuan Jiang Zhi et Hua Zhou et Zhaoqian Chen. Apprentissage de règles basé sur un ensemble de réseaux de neurones . Actes de la Conférence internationale conjointe sur les réseaux de neurones. 2002. [ Voir le contexte ].

Baback Moghaddam et Gregory Shakhnarovich. Discriminants du noyau dyadique renforcés . NIPS. 2002. [ Voir le contexte ].

Thomas Melluish et Craig Saunders et Ilia Nouretdinov et Volodya Vovk et Carol S. Saunders et I. Nouretdinov V.. Le cadre de la typicité : une comparaison avec l'approche bayésienne . Département d'informatique. 2001. [ Voir le contexte ].

Robert Burbidge et Matthew Trotter et Bernard F. Buxton et Sean B. Holden.STAR-Sparsity grâce au rejet automatisé . IWANN (1). 2001. [ Voir le contexte ].

Peter L. Hammer et Alexander Kogan et Bruno Simeone et Sandor Szedm'ak. Rapport de recherche R utcor . Centre Rutgers pour la recherche opérationnelle Université Rutgers. 2001. [ Voir le contexte ].

Endre Boros et Peter Hammer et Toshihide Ibaraki et Alexander Kogan et Eddy Mayoraz et Ilya B. Muchnik. Une mise en œuvre de l'analyse logique des données . IEEE Trans. Savoir. Data Eng, 12. 2000. [ Afficher le contexte ].

Petri Kontkanen et Petri Myllym et Tomi Silander et Henry Tirri et Peter Gr. Sur les distributions prédictives et les réseaux bayésiens. Département d'informatique, Université de Stanford. 2000. [ Afficher le contexte ].

Rudy Setiono et Wee Kheng Leow. FERNN : un algorithme pour l'extraction rapide de règles à partir de réseaux de neurones . Appl. Intell, 12. 2000. [ Voir le contexte ].

Kristin P. Bennett et Ayhan Demiriz et John Shawe-Taylor. Un algorithme de génération de colonnes pour booster . ICML. 2000. [ Afficher le contexte ].

Thomas G. Dietterich. Une comparaison expérimentale de trois méthodes de construction d'ensembles d'arbres de décision : ensachage, renforcement et randomisation . Machine Learning, 40. 2000. [ Voir le contexte ].

Lorne Mason et Peter L. Bartlett et Jonathan Baxter.Généralisation améliorée grâce à l'optimisation explicite des marges . Machine Learning, 38. 2000. [ Afficher le contexte ].

Yoav Freund et Lorne Mason. L'algorithme d'apprentissage de l'arbre de décision en alternance . ICML. 1999. [ Voir le contexte ].

Jinyan Li et Xiuzhen Zhang et Guozhu Dong et Kotagiri Ramamohanarao et Qun Sun. Extraction efficace des règles d'association à haute confiance sans seuils de prise en charge . PKDD. 1999. [ Voir le contexte ].

Chun-Nan Hsu et Hilmar Schuschel et Ya-Ting Yang. L'approche ANNIGMA-Wrapper pour la sélection de fonctionnalités de réseaux neuronaux pour la découverte de connaissances et l'exploration de données . Institut des sciences de l'information. 1999. [ Voir le contexte].

Kai Ming Ting et Ian H. Witten. Problèmes de généralisation empilée . J. Artif. Informer. Rés. (JAIR, 10. 1999. [ Voir le contexte ].

Iñaki Inza et Pedro Larrañaga et Basilio Sierra et Ramon Etxeberria et Jose Antonio Lozano et Jos Manuel Peña. Représenter le comportement des algorithmes d'apprentissage de classification supervisée par des réseaux bayésiens . Lettres de reconnaissance de motifs, 20. 1999. [ Voir le contexte ].

Jan C. Bioch et D. Meer et Rob Potharst. Arbres de décision bivariés . PKDD. 1997. [ Voir le contexte ].

D. Randall Wilson et Roel Martinez. Machine Learning : Actes de la quatorzième conférence internationale, Morgan. Dans Fisher. 1997. [ Voir le contexte ].

Pedro Domingos. Sélection de fonctionnalités sensibles au contrôle pour les apprenants paresseux . Artif. Informer. Rev, 11. 1997. [ Voir le contexte ].

Floriana Esposito et Donato Malerba et Giovanni Semeraro. Une analyse comparative des méthodes d'élagage des arbres de décision . IEEE Trans. Modèle Anal. Mach. Intell, 19. 1997. [ Voir le contexte ].

Rudy Setiono et Huan Liu. NeuroLinear : des réseaux de neurones aux règles de décision obliques . Neurocomputing, 17. 1997. [ Voir le contexte ].

. Sélection de prototypes pour les classificateurs composites du voisin le plus proche. Département d'informatique de l'Université du Massachusetts. 1997. [ Voir le contexte ].

Igor Kononenko et Edvard Simec et Marko Robnik-Sikonja. Surmonter la myopie des algorithmes d'apprentissage inductif avec RELIEFF . Appl. Intell, 7. 1997. [ Voir le contexte ].

Kamal Ali et Michael J. Pazzani. Réduction des erreurs grâce à l'apprentissage de descriptions multiples . Machine Learning, 24. 1996. [ Afficher le contexte ].

Ron Kohavi. Le pouvoir des tables de décision . CELV. 1995. [ Voir le contexte ].

Ron Kohavi et Dan Sommerfield. Sélection de sous-ensembles d'entités à l'aide de la méthode Wrapper : surapprentissage et topologie de l'espace de recherche dynamique. KDD. 1995. [ Voir le contexte ].

Peter D. Turney. Classification sensible aux coûts : évaluation empirique d'un algorithme d'induction d'arbre de décision génétique hybride . CRR, csAI/9503102. 1995. [ Voir le contexte ].

Gabor Melli. Une approche paresseuse basée sur un modèle pour la classification en ligne . Université de la Colombie-Britannique. 1989. [ Voir le contexte ].

Adil M. Bagirov et Alex Rubinov et AN Soukhojak et John Yearwood. Classification des données non supervisée et supervisée via une optimisation globale et non fluide . École des technologies de l'information et des sciences mathématiques, Université de Ballarat. [ Afficher le contexte ].

Bruce H. Edmonds.Utilisation de « Gossip » localisés pour structurer l'apprentissage distribué . Centre de modélisation des politiques. [ Afficher le contexte ].

Kristin P. Bennett et Erin J. Bredensteiner. La géométrie dans l'apprentissage . Département des sciences mathématiques Institut polytechnique Rensselaer. [ Afficher le contexte ].

Rafael S. Parpinelli et Heitor S. Lopes et Alex Alves Freitas. QUATRIÈME PARTIE : OPTIMISATION DES COLONIES DE FOURMIS ET SYSTÈMES IMMUNITAIRES Chapitre X Un algorithme de colonie de fourmis pour la découverte de règles de classification . CEFET-PR, Curitiba. [ Afficher le contexte ].

Wl/odzisl/aw Duch et Karol Grudzinski et Geerd H. F Diercksen. Méthodes neuronales à distance minimale. Département de méthodes informatiques, Université Nicholas Copernicus. [ Afficher le contexte ].

John G. Cleary et Leonard E. Trigg. Expériences avec OB1, un apprenant optimal de l'arbre de décision de Bayes . Département d'informatique Université de Waikato. [ Afficher le contexte ].

Glenn Fung et Sathyakama Sandilya et R. Bharat Rao. Extraction de règles à partir de machines à vecteurs de support linéaire . Diagnostic et thérapie assistés par ordinateur, Siemens Medical Solutions, Inc. [ Consulter la vue ].

Ayhan Demiriz et Kristin P. Bennett et John Shawe et I. Nouretdinov V.. Stimulation de la programmation linéaire via la génération de colonnes . Département des sciences de la décision et ing. Systèmes, Institut polytechnique Rensselaer. [Afficher le contexte ].

Zhi-Hua Zhou et Xu-Ying Liu. Formation de réseaux de neurones sensibles aux coûts avec des méthodes résolvant le problème du déséquilibre de classe . [ Afficher le contexte ].

Liping Wei et Russ B. Altman. Un système automatisé pour générer des profils comparatifs de maladies et établir des diagnostics . Section sur l'informatique médicale École de médecine de l'Université de Stanford, MSOB X215. [ Afficher le contexte ].

Federico Divina et Elena Marchiori. Gestion des attributs continus chez un apprenant inductif évolutif . Département d'informatique Vrije Universiteit. [ Afficher le contexte ].

Ron Kohavi et George H. John.Sélection automatique des paramètres en minimisant l'erreur estimée . Département d'informatique, Université de Stanford. [ Afficher le contexte ].

H. -T Lin et C. -J Lin. Une étude sur les noyaux sigmoïdes pour SVM et la formation de noyaux non PSD par des méthodes de type SMO . Département d'informatique et d'ingénierie de l'information Université nationale de Taiwan. [ Afficher le contexte ].

Alexandre K. Seewald. Dissertation Vers la compréhension des études d'empilement d'un schéma d'apprentissage d'ensemble général ausgefuhrt zum Zwecke der Erlangung des akademischen Grades eines Doktors der technischen Naturwissenschaften . [ Afficher le contexte ].

Wl odzisl et Rafal Adamczak et Krzysztof Grabczewski et Grzegorz Zal.Une méthode hybride pour l'extraction de règles logiques à partir de données . Département de méthodes informatiques, Université Nicholas Copernicus. [ Afficher le contexte ].

Wl odzisl/aw Duch et Karol Grudzinski. Recherche et minimisation globale dans les méthodes basées sur la similarité . Département de méthodes informatiques, Université Nicholas Copernicus. [ Afficher le contexte ].

Rudy Setiono et Wee Kheng Leow. Génération de règles à partir d'un réseau formé à l'aide d'un élagage rapide . École d'informatique Université nationale de Singapour. [ Afficher le contexte ].

Elena Smirnova et Ida G. Sprinkhuizen-Kuyper et I. Nalbantis et b. ERIM et Universiteit Rotterdam. Vote à l'unanimité à l'aide de machines à vecteurs de support. IKAT, Universiteit Maastricht. [ Afficher le contexte ].

Krista Lagus et Esa Alhoniemi et Jeremias Seppa et Antti Honkela et Arno Wagner. ANALYSE DE GROUPE VARIABLE INDÉPENDANTE DANS L'APPRENTISSAGE DE REPRÉSENTATIONS COMPACTES POUR LES DONNÉES . Centre de recherche sur les réseaux neuronaux, Université de technologie d'Helsinki. [ Afficher le contexte ].

Chiranjib Bhattacharyya et Pannagadatta K. S et Alexander J. Smola. Une formulation de programmation de cône de second ordre pour classer les données manquantes . Département d'informatique et d'automatisation Institut indien des sciences. [ Afficher le contexte ].

Ayhan Demiriz et Kristin P. Bennett. Chapitre 1 APPROCHE D'OPTIMISATION DE L'APPRENTISSAGE MI SUPERVISÉ. Département des sciences de la décision et des systèmes d'ingénierie et Département des sciences mathématiques, Institut polytechnique Rensselaer. [ Afficher le contexte ].

Adil M. Bagirov et John Yearwood. Un nouvel algorithme d'optimisation non fluide pour le clustering . Centre d'informatique et d'optimisation appliquée, École des technologies de l'information et des sciences mathématiques, Université de Ballarat. [ Afficher le contexte ].



Demande de citation :

Les auteurs des bases de données ont demandé que toutes les publications résultant de l'utilisation des données incluent les noms du chercheur principal responsable de la collecte des données dans chaque établissement. Ils seraient :
1. Institut hongrois de cardiologie. Budapest : Andras Janosi, MD
2. Hôpital universitaire, Zurich, Suisse : William Steinbrunn, MD
3. Hôpital universitaire, Bâle, Suisse : Matthias Pfisterer, MD
4. VA Medical Center, Long Beach et Cleveland Clinic Foundation : Robert Detrano, MD, doctorat
