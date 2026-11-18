# Prévision de séries temporelles avec Facebook Prophet

**Projet Master IA & Data — Jacques Callewaert**

## Présentation

Ce projet consiste à analyser et prévoir l'évolution de l'intérêt pour le terme « data science » aux États-Unis à partir d'un jeu de données Google Trends couvrant janvier 2004 à août 2020.

## Technologies

- Python
- Pandas et NumPy
- Matplotlib
- Facebook Prophet
- Scikit-learn
- Jupyter Notebook / VS Code

## Méthodologie

1. Importation et exploration des données.
2. Nettoyage et préparation de la série temporelle.
3. Analyse de la tendance historique.
4. Découpage chronologique entraînement/test.
5. Entraînement d'un modèle Prophet.
6. Évaluation des prédictions sur 24 mois.
7. Prévision sur deux années supplémentaires.
8. Analyse de la tendance et de la saisonnalité.
9. Validation croisée temporelle.

## Résultats

**Évaluation sur 24 mois de test :**

| Métrique | Résultat |
|---|---:|
| MAE | 8,29 |
| RMSE | 10,71 |
| MAPE | 10,78 % |

**Validation croisée temporelle :**

| Métrique | Résultat |
|---|---:|
| MAE | 4,54 |
| RMSE | 6,09 |
| MAPE | 15,85 % |
| Coverage | 46,59 % |

## Principales observations

L'intérêt pour la data science présente une forte croissance à partir de 2013. Prophet capture globalement cette évolution, mais rencontre des difficultés à anticiper les variations brusques.

La validation croisée révèle notamment une couverture insuffisante des intervalles d'incertitude. La saisonnalité annuelle présente également un risque de surajustement.

Les prévisions historiques sur 2020–2022 doivent être interprétées avec prudence, notamment parce que certaines dépassent l'échelle normalisée de Google Trends.

## Conclusion

Ce projet illustre la capacité de Prophet à modéliser une tendance temporelle et à produire des prévisions interprétables, ainsi que l'importance de mesurer leurs limites par une évaluation chronologique rigoureuse.