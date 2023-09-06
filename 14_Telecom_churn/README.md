﻿## Прогнозирование оттока клиентов оператора связи
---

### Цель
Построить модель, которая сможет пресказать факт разрыва договора с оператором связи

### Описание
В нашем распоряжении персональные данные о некоторых клиентах, информация об их тарифах и договорах с датами начала и прекращения дествия договора. Необходимо выявить клиентов, которые наиболее вероятно разорвут договор для планирования промоакций с целью удержания этих клиентов.


### Используемые библиотеки
- **`LightGBM`**
- **`Scikit-learn`**
- **`NumPy`**
- **`Pandas`**
- **`Matplotlib`**
- **`Seaborn`**

### Результаты
- Был проведён разведочный анализ данных, показано распределение значений признаков относительно таргета, исследована корреляция признаков между собой
- Построили несколько моделей машинного обучения и выбрали наиболее подходящую модель. На выбранной модели были получены следующие значения метрик: **ROC_AUC = 0.896, Accuracy = 0.91**
         