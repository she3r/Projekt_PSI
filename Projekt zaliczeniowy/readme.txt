## Projekt zaliczeniowy PSI

### Autor: Piotr Kubacki
### Zbior danych: https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset
(Predicting Stroke Dataset)
### Temat: Klasyfikacja: Przewidywanie zawału u pacjenta
### Jezyk: Python

## Po wstępnej kwalifikacji, wybrano modele do uczenia (accuracy):
- MLPClassifier
- SVC linear
- SVC rbf
- Logistic Regression
- AdaBoost
Każdy z nich wygenerował podobny, bardzo dobry wynik. 
### Najlepszy jednak uzyskał MLP Classifier: 0.95555 acc

## Po wstępnej kwalifikacji, wybrano modele do uczenia (recall):
- RandomTreeClassifier
- KNN
Jest problem z dobrym wyszkoleniem pod recall. Modele nie wychodzą poza barierę 12%. Podejrzewam, że może chodzić o nierealistyczne dane do uczenia. Dane były preprocesowane względem norm dla bmi i avg_glucose_level podlinkowanych w pracy, być może te normy nie były brane pod uwagę przy tworzeniu danych.

### Po gridowaniu najlepszy wynik uzyskał KNN
