# Задача
Построение модели, котороя должна предсказать коэффициент восстановления золота из золотосодержащей руды. 
Для данной цели используется метрика sMAPE и метрика эффективности обогащения
Recovery = (C*(F-T))/(F*(C-T))*100%
C — доля золота в концентрате после флотации/очистки;
F — доля золота в сырье/концентрате до флотации/очистки;
T — доля золота в отвальных хвостах после флотации/очистки.

# Используемые библиотеки
В данном проекте использовались библиотеки pandas, numpy, sklearn, seaborn

и в частности sklearn.linear_model.LinearRegression, sklearn.ensemble.RandomForestRegressor, sklearn.model_selection.cross_val_score, sklearn.model_selection.GridSearchCV
# Данные
данные были в трех файлах: gold_industry_train.csv, gold_industry_test.csv, gold_industry_full.csv

|Технологический процесс||
| :--------------------: | :---------------------: |
|Rougher feed | исходное сырье|
|Rougher additions (или reagent additions) — флотационные реагенты: Xanthate, Sulphate, Depressant|
|Xanthate | ксантогенат (промотер, или активатор флотации)|
|Sulphate | сульфат (на данном производстве сульфид натрия)|
|Depressant | депрессант (силикат натрия)|
|Rougher process | флотация|
|Rougher tails | отвальные хвосты|
|Float banks | флотационная установка|
|Cleaner process | очистка|
|Rougher Au | черновой концентрат золота|
|Final Au | финальный концентрат золота|

|Параметры этапов||
| :--------------------: | :---------------------: |
|air amount | объём воздуха|
|fluid levels | уровень жидкости|
|feed size | размер гранул сырья|
|feed rate | скорость подачи|

