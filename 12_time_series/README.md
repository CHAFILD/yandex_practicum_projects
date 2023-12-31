# Прогнозирование количество заказов такси

Компания «Чётенькое такси» собрала исторические данные о заказах такси в аэропортах. Чтобы привлекать больше водителей в период пиковой нагрузки, нужно спрогнозировать количество заказов такси на следующий час. 

## Цель исследования:

Постройте модель для предсказания количества заказов.

Значение метрики `RMSE` на тестовой выборке должно быть не больше `48`.

## Итог исследования:
Наилучший результат показала модель `Random Forest`, которая имеет `RMSE` на тестовой выборке равный `45.97`. Она позволяет предсказать количество заказов такси с точностью, достаточной для решения бизнес-задачи.

## Используемые библиотеки:

`Pandas` `Matplotlib` `Seaborn` `Numpy` `Scikit-learn` `Statsmodels` `CatBoost`
