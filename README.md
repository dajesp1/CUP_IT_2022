# CUP_IT_2022
Data Science Case Championship

Cup IT – онлайн кейс-чемпионат от Changellenge в области Data Science. 
Даты проведения: с 2 по 9 марта (первый тур), а также c 16 по 23 марта (финал).
Ссылка на соревнование:  https://changellenge.com/championships/changellenge-cup-it-2022

# Задача:
### Первый тур:
Построить look-alike-модель на основе классификации данных, которая производит скоринг участников программы лояльности и предсказывает, кто из них максимально похож на людей, недавно присоединившихся к «Клубу полезных привычек». Необходимо предсказать, кто из держателей карт лояльности потенциально смог бы присоединиться к клубу.
### Второй тур:
Проанализировать ошибки и выдвинуть гипотезы о том, как их справить. Доработать модель первого тура, улучшить показатели качества модели на 3-5% (основываясь на метрике f1). Проверить работу модели на более сложном датасете с новыми признаками.

# Предобработка и итоговая модель
- Заполнение пропусков 0, вследствие критического процента пропусков в датасете. Исправление недочетов датасета: отрицательные суммы покупок, отрицательное std суммы покупок. Обработка выбросов.
- Учет внешних факторов: продуктовая инфляция, рост заработной платы
- Анализ признаков и построение новых признаков

### Не вошло в решение:
- Oversampling, undersampling
- TableNet как часть модели

Итоговая модель : CatBoost + LightGBM с подбором гиперпараметров на кросс-валидации. 

# Установка библиотек
```python
! pip install catboost
! pip install optuna
! pip install shap
```
# Контакты для связи в Telegram
@Umaaaaaaaa – Ума Абдуллаева
@sonya_serebryakova – Соня Серебрякова

