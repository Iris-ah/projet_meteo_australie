Récapitulatif des modèles de l'équipe

Ce document présente les modèles testés dans le cadre du projet météo ainsi que leurs performances principales.

1. Modèles exploratoires initiaux

Les premiers essais ont inclus plusieurs modèles de base :

régression logistique,

arbres de décision,

modèles simples servant de baseline.

Ils ont permis d’obtenir une première mesure de performance sur la variable RainTomorrow et de fixer un point de comparaison.

2. Modèle de Gradient Boosting (XGBoost)

Un modèle XGBoost a été testé pour :

évaluer une approche de gradient boosting plus avancée,

comparer son score F1 avec les autres modèles,

analyser son potentiel pour détecter les jours pluvieux.

Bien que performant, il n’a pas permis d’obtenir une amélioration significative du F1-score pluie.

3. Modèle RandomForest – base et version optimisée
Modèle RandomForest de base

F1 pluie : 0.600

Rappel pluie : 0.487

Précision pluie : 0.782

Version optimisée (RandomizedSearchCV)

F1 pluie : 0.611

Rappel pluie : 0.520

Précision pluie : 0.741

L’optimisation a amélioré :

la capacité à détecter les jours de pluie (rappel en hausse),

l’équilibre global entre les métriques.

4. Modèle final retenu

Le modèle HistGradientBoosting a été retenu comme modèle final car il présente les meilleurs résultats globaux :

F1 pluie : 0.69

Précision pluie : 0.71

Rappel pluie : 0.67

Accuracy : 0.86

Ce modèle :

offre les meilleures performances sur la classe pluie,

est robuste sur l’ensemble des données,

surpasse les autres modèles de l'équipe,

constitue la meilleure base pour l’application Streamlit et la présentation finale.
