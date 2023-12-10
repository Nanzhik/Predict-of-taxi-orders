# Прогнозирование заказов такси

[ipynb](https://github.com/Nanzhik/Predict-of-taxi-orders/blob/main/Predict-of-taxi-orders.ipynb)
[HTML](https://github.com/Nanzhik/Predict-of-taxi-orders/blob/main/Predict-of-taxi-orders.html)

## Описание проекта

Компании «Чётенькое такси» необходимо спрогнозировать количество заказов такси на следующий час, чтобы привлекать больше водителей в период пиковой нагрузки и построить модель для такого предсказания. В распоряжении исторические данные о заказах такси в аэропортах.

## Навыки и инструменты

* **python**
* **pandas**
* **seaborn**
* **numpy**
* matplotlib.**pyplot**
* sklearn.model_selection.**TimeSeriesSplit**
* sklearn.linear_model.**Ridge**
* sklearn.ensemble.**RandomForestRegressor**
* lightgbm.**LGBMRegressor**
* catboost.**CatBoostRegressor**
* xgboost.**XGBRegressor**
* statsmodels.tsa.seasonal.**seasonal_decompose**
* statsmodels.tsa.stattools.**adfuller**

## Вывод

- Исследованы исходные данные и подготовлены к анализу (проведено ресемплирование данных по 1 часу);
- Построены графики временных рядов
- Выявлен возврастающий тренд заказов такси от начала весны к концу лета
- Определена сезонность заказов такси, равная одному дню, также отдельно выведена сезонность за в течение недели
- Проведено обучение 5 моделей: *RandomForestRegressor*, *Ridge*, *LGBMRegressor*, *XGBRegressor* и *CatBoostRegressor*
- Определена наилучшая модель по сумме показателей (время обучения, время предсказания и лучшее RMSE модели) - *CatBoostRegressor*, и проведено ее тестирование
