# [Natural Language Processing course (stream 7, autumn 2024)](https://ods.ai/tracks/nlp-course-autumn-2024)
## Финальное задание
Суть проекта - выявить разницу между качеством генерации заголовков новостных статей (задача суммаризации) между более "мощной" моделью ruGPT-3 Medium (350 млн параметров), дообученной на меньшем кол-ве данных (6900 статей), и более "слабой" моделью ruGPT-3 Small (125 млн параметров), дообученной на большем кол-ве данных (15000 статей).

Результат: более "слабые" модели ruGPT-3 Small, обученные на большем кол-ве данных, показывают значительно более высокий результат (согласно метрике ROUGE), чем более "мощные" модели ruGPT-3 Medium, обученные на меньшем количестве данных.

В таблице ниже представлены средние значения F-мер, полученные в результате оценки сгенерированных моделями заголовков метрикой ROUGE. Значения показывают, насколько в среднем процентов сгенерированные заголовки похожи на оригинальные. "Наука", "Спорт" и "Наука+Спорт" - названия моделей по датасетам новостей, на которых они были дообучены (всего 6 моделей). 

|  | RuGPT-3 Medium | RuGPT-3 Small |
|----------|----------|----------|
| Наука    | 17,4    | 23,8    |
| Спорт    | 19,6    | 32,8    |
| Наука+Спорт    | 22    | 27,5    |
