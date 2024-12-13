# Студент группы М8О-407Б-21 Дегтярев Денис Андреевич

1) data - в данной папке содержатся файлы для задач:
    - gym_members_exercise_tracking.csv - задача классификации
    - insurance.csv - задача регрессии

2) implementation - в данной папке содержатся реализации моделей для задач классификации и регрессии:
    - [KNN](implementation/KNN.py) - реализация к ближайших соседей
    - [Regressor](implementation/Regressor.py) - реализация линейной и логистической регрессий
    - [DecTree](implementation/DecTree.py) - реализация решающего дерева
    - [RandForest](implementation/RandForest.py) - реализация случайного леса
    - [Boost](implementation/Boost.py) - реализация градиентного бустинга

3) lab1, lab2, lab3, lab4, lab5 - проведение EDA и тест моделей KNearestNeighbors, Linear(Logistic)Regression, DecisionTree, RandomForest, GradientBoosting

# Подведение итогов

Метрика оценки качества регрессии: **F1-score**;  
Метрика оценки качества классификации: **MAE**;

*Метрики качества на тестовом наборе данных*
<table>
    <tr>
        <th rowspan="1">Алгоритм</th>
        <th>Задача</th>
        <th>Бейзлайн</th>
        <th>Улучшенный бейзлайн</th>
        <th>Самостоятельная имплементация алгоритма</th>
    </tr>
    <tr>
        <td rowspan="2">KNN</td>
        <td>классификация</td>
        <td>0.76</td>
        <td>0.96</td>
        <td>0.94</td>
    </tr>
    <tr>
        <td>регрессия</td>
        <td>7708</td>
        <td>3494</td>
        <td>3494</td>
    </tr>
    <tr>
        <td rowspan="2">Линейные модели</td>
        <td>классификация</td>
        <td>0.86</td>
        <td>0.92</td>
        <td>0.93</td>
    </tr>
    <tr>
        <td>регрессия</td>
        <td>4181</td>
        <td>4254</td>
        <td>4181</td>
    </tr>
    <tr>
        <td rowspan="2">Решающее дерево</td>
        <td>классификация</td>
        <td>0.97</td>
        <td>0.98</td>
        <td>0.98</td>
    </tr>
    <tr>
        <td>регрессия</td>
        <td>3107</td>
        <td>3225</td>
        <td>3170</td>
    </tr>
    <tr>
        <td rowspan="2">Случайный лес</td>
        <td>классификация</td>
        <td>0.99</td>
        <td>0.99</td>
        <td>0.96</td>
    </tr>
    <tr>
        <td>регрессия</td>
        <td>2554</td>
        <td>2531</td>
        <td>2500</td>
    </tr>
    <tr>
        <td rowspan="2">Градиентный бустинг</td>
        <td>классификация</td>
        <td>0.99</td>
        <td>0.98</td>
        <td>0.99</td>
    </tr>
    <tr>
        <td>регрессия</td>
        <td>2398</td>
        <td>2410</td>
        <td>3989</td>
    </tr>
</table>


<br><br>
Укажу лучшие модели для каждого отдельного кейса:
<br>

```
Регрессия: градиентный бустинг  
Классификация: случайный лес
