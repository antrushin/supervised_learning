# ОБУЧЕНИЕ С УЧИТЕЛЕМ

В данном проекте рассматривается решение задачи классификации, где целевой признак не сбалансирован.

## Краткое описание проекта и расшифровка столбцов

Из банка стали уходить клиенты. Немного, но заметно. Из расчетов известно, что сохранять текущих клиентов дешевле, чем привлекать новых.

Нужно спрогнозировать, уйдет клиент из банка в ближайшее время или нет. Представлены исторические данные о поведении клиентов и расторжении договоров с банком.

Расшифровка названий столбцов:

**Признаки**


* RowNumber — индекс строки в данных
* CustomerId — уникальный идентификатор клиента
* Surname — фамилия
* CreditScore — кредитный рейтинг
* Geography — страна проживания
* Gender — пол
* Age — возраст
* Tenure — сколько лет человек является клиентом банка
* Balance — баланс на счёте
* NumOfProducts — количество продуктов банка, используемых клиентом
* HasCrCard — наличие кредитной карты
* IsActiveMember — активность клиента
* EstimatedSalary — предполагаемая зарплата

**Целевой признак**

* Exited — факт ухода клиента

  

## Используемые алгоритмы машинного обучения

1. Логистическая регрессия;
2. Дерево решений;
3. Случайный лес.

Для поиска оптимальных гиперпараметров была использована байесовская оптимизация из библиотеки **hyperopt** как в примере по этой ссылке https://habr.com/ru/post/542624/

## Методы борьбы с дисбалансом

1. Автобалансировка;
2. Увеличение выборки (Upsampling);
3. Уменьшение выборки (Downsampling).

