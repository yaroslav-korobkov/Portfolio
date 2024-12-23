# Множественная классификация обратной связи от пользователей службы доставки продуктов
Ссылка на Jupyter Notebook проекта: [ipynb](https://github.com/yaroslav-korobkov/Portfolio/blob/main/NLP_Samokat.tech/nlp_samokat.ipynb)

## Описание проекта

В этом проекте была поставлена задача множественной классификации отзывов пользователей службы доставки для определения всех классов, к которым можно отнести каждый экземпляр.

## Технологии

- pandas
- numpy
- matplotlib
- nltk
- re
- pymorphy2
- os
- pickle
- optuna
- hashlib
- sys
- requests
- tensorflow
- navec
- keras
- sklearn
- xgboost
- lightgbm
- catboost
- RandomForestClassifier
- SVC
- ClassifierChain
- Word2Vec

## Общий вывод

### Часть 1: Загрузка и анализ данных

Загрузил данные, провел их первичный анализ, предобработку, очистил от пропусков и дубликатов, а также преобразовал типы данных.

### Часть 2: Векторизация текстовых данных

Использовал различные методы векторизации, включая TfidfVectorizer, Word2Vec и Navec, чтобы определить оптимальный подход для машинного обучения.

### Часть 3: Обучение моделей

Для обучения применил методы кросс-валидации из-за ограниченного объема данных. Лучшие результаты показал LGBMClassifier с точностью 0.678 на данных, векторизированных с помощью TfidfVectorizer.

### Часть 4: Оптимизация и результаты

Попытки применения нейронной сети не привели к удовлетворительным результатам. Оптимизация LGBMClassifier с расширенной сеткой гиперпараметров улучшила метрику до 0.679.
