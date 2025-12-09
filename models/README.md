# Fichiers du modèle

Le fichier `random_forest_optimized.joblib` n'est **pas inclus dans ce dépôt** car sa taille dépasse la limite d’upload autorisée par GitHub.

Il est généré automatiquement à partir du script `rf_search.py` :

```bash
python rf_search.py
import os
os.makedirs("models", exist_ok=True)
joblib.dump(best_rf, "models/random_forest_optimized.joblib")

## 📊 Performances du modèle optimisé

Après optimisation avec RandomizedSearchCV, les meilleurs hyperparamètres trouvés sont :

```python
{'n_estimators': 100,
 'min_samples_split': 5,
 'min_samples_leaf': 1,
 'max_features': 0.5,
 'max_depth': None,
 'bootstrap': False}
