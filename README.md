# Prédiction de Carrière pour Étudiants en Informatique

Projet personnel — Licence 3 Informatique, Aix-Marseille Université.

En tant qu'étudiante en informatique moi-même, ce dataset m'a tout de suite intéressée : peut-on prédire l'orientation professionnelle d'un étudiant à partir de son profil (GPA, compétences, domaine d'intérêt) ?

Ce projet est différent de mes deux précédents (NLP) — ici les données sont **tabulaires et structurées**.



## Ce que fait ce projet

À partir de 180 profils d'étudiants en informatique :
- analyse exploratoire : GPA par domaine, compétences par genre, carrières visées
- regroupement des 33 métiers en 6 familles cohérentes
- encodage des variables catégorielles (compétences, domaine, genre)
- comparaison de 3 modèles : Régression Logistique, Random Forest, Gradient Boosting
- analyse de l'importance des features
- fonction de prédiction sur un profil personnalisé

## Résultats

| Modèle | Accuracy test | CV moyen (5-fold) |
|--------|--------------|-------------------|
| Régression Logistique | 61.1% | 55.6% |
| Random Forest | 83.3% | 72.9% |
| Gradient Boosting | 86.1% | 91.0% |

Le Gradient Boosting est le meilleur modèle avec 86% d'accuracy et 91% en validation croisée.

**Observation clé :** le domaine d'intérêt est de loin la feature la plus prédictive, devant le GPA et les compétences techniques.



## Fichiers

- `student_career_barbara.ipynb` — notebook complet
- `cs_students.csv` — dataset (180 étudiants en informatique)



## Lancer le projet

```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
jupyter notebook student_career_barbara.ipynb
```

## Dataset

"Computer Science Students Performance Dataset" — disponible sur [Kaggle](https://www.kaggle.com/datasets/zahra-nusrat/cs-students).



## Ce que j'aimerais faire ensuite

- Explorer le clustering (K-Means) pour identifier des profils d'étudiants sans supervision
- Tester sur un dataset plus grand avec des notes par matière
- Comparer avec une approche deep learning sur plus de données



## Auteure

**Barbara KENGNE**
Licence 3 Informatique — Aix-Marseille Université
[LinkedIn](https://www.linkedin.com/in/barbara-nguimfack-kengne-343094303) | [GitHub](https://github.com/BarbaraKengne) | [Kaggle](https://kaggle.com/barbarakengne)
