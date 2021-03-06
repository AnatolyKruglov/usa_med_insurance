# usa_med_insurance
Предсказание медицинских расходов американцев с помощью линейной регрессии

## Постановка задачи бизнесом
Необходимо предсказать индивидуальные медицинские расходы граждан США, оплачиваемые медицинской страховкой. 

## Декомпозиция задачи
Я действовал по стандартному алгортму решения ML-задач:
1. Исследование данных
2. Подготовка данных
3. Моделирование
4. Оценка модели

В сумме провел 4 итерации:
1. Бэйслайн, простая линейная модель, обученная на сырых данных
2. Перевод целевого признака из логнормального в нормальное распределение, определение выбросов в распределении других признаков
3. Нормализация признаков, добавление полиномиальной модели (признаки стпепени 2)
4. Регуляризация (сравнение эффективности L1 и L2 регуляризаторов)

## Итог
Модель позволила уменьшить величину средней абсолютной процентной ошибки (MAPE) более чем вдвое: почти на 60%. Средняя абсолютная ошибка уменьшилась на полторы тысячи долларов. R^2 улучшился примерно на 10 пунктов.
