# Fichiers du modèle

Le fichier `random_forest_optimized.joblib` n'est **pas inclus dans ce dépôt** car sa taille dépasse la limite d’upload autorisée par GitHub.

Il est généré automatiquement à partir du script `rf_search.py` :

```bash
python rf_search.py
import os
os.makedirs("models", exist_ok=True)
joblib.dump(best_rf, "models/random_forest_optimized.joblib")

