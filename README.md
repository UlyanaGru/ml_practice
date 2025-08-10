`Исследование факторов датасета на наличие влияния лояльности клиентов`

1. Проведена визуализация полученных данных

Зависимость возраста киента от готовности уйти от банка
![AgeLoyality](https://github.com/UlyanaGru/ml_practice/blob/master/pictures/Age%20Loyality.png)
Зависимость лояльности клиента от географического расположения
![GepgraphicalLoyality](https://github.com/UlyanaGru/ml_practice/blob/master/pictures/Geography_Loyality.png)
Зависимость кредитного рейтинга от готовности клиента уйти
![CreditScoreLoyality](https://github.com/UlyanaGru/ml_practice/blob/master/pictures/count_CresitScore_Loyal.png)
Матрица корреляций для признаков
![CorrMatrix](https://github.com/UlyanaGru/ml_practice/blob/master/pictures/corr%20matrix.png)

2. Построенные модели

Обучена линейная модель linear_model (LogisticRegression) с подбором оптимального порога вероятности
![LogisticRegression](https://github.com/UlyanaGru/ml_practice/blob/master/pictures/F1%20L1%20Regurazation.png)
Из модуля preprocessing созданы полиномиальные признаки (PolynomialFeatures)\
По ним обучена модель с минимизацией логистических потерь и подром оптимального порога вероятности
![PolynomialFeatures](https://github.com/UlyanaGru/ml_practice/blob/master/pictures/f1%20probability%20thresholds.png)
Произведено сравнение между DecisionTreeClassifier vs RandomForestClassifier из модуля sklearn.tree\
Выбрана наилучшая, рассчитана метрика на тестовых и тренировочных данных
![DecisionTreeClassifier](https://github.com/UlyanaGru/ml_practice/blob/master/pictures/f1%20probability%20thresholds%20tree.png)

`Заключение`

По итогам экспериментов получено значение метрики f1-score = 0.653. Модель успешно справляется с задачей, пример исследования приведен в [проекте](https://github.com/UlyanaGru/ml_practice/blob/master/ml_practice.ipynb)