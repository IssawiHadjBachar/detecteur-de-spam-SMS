# SMS Spam Detection

Un système complet de détection de SMS spam comparant des modèles classiques de machine learning (Naive Bayes, SVM, Logistic Regression) avec un modèle deep learning (BERT).

## 🎯 Fonctionnalités

- **Plusieurs modèles** : Comparaison de 4 approches différentes
  - Naive Bayes
  - Support Vector Machine (SVM)
  - Logistic Regression
  - BERT (Transformer-based)
- **Dataset UCI** : Utilisation du dataset standard SMS Spam Collection (5 574 messages)
- **Pipeline complet** : Chargement des données, prétraitement, entraînement, évaluation et visualisation
- **Prédiction interactive** : Tester les modèles sur de nouveaux messages

## 📊 Performances

| Modèle | Accuracy | AUC-ROC |
|--------|---------|---------|
| BERT | ~0.99 | ~0.99 |
| SVM | ~0.98 | ~0.98 |
| Logistic Regression | ~0.97 | ~0.97 |
| Naive Bayes | ~0.97 | ~0.97 |

## 📁 Structure du projet
`````
.
│   .gitignore                  # Fichiers et dossiers ignorés par Git
│   requirements.txt            # Dépendances Python du projet
│
├───Notebooks                   # Notebooks pour l'expérimentation et l'analyse
│       bert_model.ipynb        # Fine-tuning et évaluation du modèle BERT
│       classical_models.ipynb  # Entraînement et évaluation des modèles classiques (Naive Bayes, SVM, LR)
│       comparison.ipynb        # Comparaison des performances de tous les modèles
│       data_loading.ipynb      # Chargement et préparation des données
│       testing.ipynb           # Test de prédictions sur de nouveaux messages
│
├───outputs                     # Visualisations et résultats générés
│       sms_confusion_matrix.png    # Matrice de confusion pour le meilleur modèle
│       sms_eda.png                 # Analyse exploratoire des données
│       sms_model_comparison.png    # Comparaison graphique des performances
`````
### Notes

- Les dossiers `data/` et `bert_sms_spam/` sont **ignorés par Git** car ils contiennent des fichiers volumineux (datasets, modèles entraînés).  
- Les notebooks permettent de reproduire **l’ensemble du workflow**, depuis le chargement des données jusqu’aux prédictions finales.  
- Les visualisations dans `outputs/` facilitent la comparaison des modèles et l’analyse des résultats.
