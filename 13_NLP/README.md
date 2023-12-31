# Проект для «Викишоп»

Интернет-магазин «Викишоп» запускает новый сервис. Теперь пользователи могут редактировать и дополнять описания товаров, как в вики-сообществах. То есть клиенты предлагают свои правки и комментируют изменения других. Магазину нужен инструмент, который будет искать токсичные комментарии и отправлять их на модерацию. 

## Цель исследования:

Обучите модель классифицировать комментарии на позитивные и негативные. В вашем распоряжении набор данных с разметкой о токсичности правок.

Постройте модель со значением метрики качества *F1* не меньше 0.75. 

## Итог исследования:

На кросс-валидации лучшую метрику `F1 0.761` показала модель `Logistic Regression`.

Был проведен процесс подбора гиперпараметров модели `Logistic Regression` с использованием `GridSearchCV`, что позволило получить значения параметров: `{'model__C': 8, 'tfidf__max_df': 0.25, 'tfidf__ngram_range': (1, 2)}`. После этого была проведена проверка модели на тестовой выборке, которая дала следующие метрики: 

* F1 - `0.758`
* Precision - `0.759`
* Recall - `0.756`
* Accuracy - `0.951`
* ROC-AUC: 0.965

## Используемые библиотеки:

`Pandas` `Matplotlib` `Numpy` `Scikit-learn` `Seaborn` `NLTK` `re` `CatBoost` `Imblearn`
