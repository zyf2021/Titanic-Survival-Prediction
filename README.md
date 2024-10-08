# Titanic-Survival-Prediction
Проект направлен на предсказание выживаемости пассажиров с использованием данных о рейсе Титаника. На основе таких характеристик, как возраст, пол, класс билета и другие факторы, мы будем строить модель машинного обучения, чтобы предсказать, кто выжил, а кто нет.

Отлично! Проект по анализу выживаемости пассажиров **Titanic Survival Prediction** является классической задачей в области машинного обучения, особенно в контексте бинарной классификации. Давайте начнем с пошагового плана для этого проекта.

### Шаги выполнения проекта:

#### 1. Описание задачи:
Проект направлен на предсказание выживаемости пассажиров с использованием данных о рейсе Титаника. На основе таких характеристик, как возраст, пол, класс билета и другие факторы, мы будем строить модель машинного обучения, чтобы предсказать, кто выжил, а кто нет.

#### 2. Получение данных:
Для этого проекта мы будем использовать знаменитый набор данных **Titanic**, который можно скачать с различных источников (например, с Kaggle).
  
- **Ссылка на данные Titanic на Kaggle**: [Titanic Dataset](https://www.kaggle.com/c/titanic/data)

В датасете есть следующие основные столбцы:
- `PassengerId`: Идентификатор пассажира.
- `Survived`: Целевая переменная (1 – пассажир выжил, 0 – не выжил).
- `Pclass`: Класс билета пассажира (1-й, 2-й, или 3-й класс).
- `Name`: Имя пассажира.
- `Sex`: Пол.
- `Age`: Возраст.
- `SibSp`: Количество родственников на борту (братья, сестры, супруги).
- `Parch`: Количество родителей/детей на борту.
- `Ticket`: Номер билета.
- `Fare`: Цена билета.
- `Cabin`: Номер каюты (многие значения отсутствуют).
- `Embarked`: Порт посадки (C = Cherbourg, Q = Queenstown, S = Southampton).

#### 3. Предобработка данных:
Цель на данном этапе — очистить и подготовить данные для модели.

- Обработка **пропущенных данных** (например, у возрастов или кают могут быть пропуски).
- Преобразование категориальных признаков в числовые (например, `Sex`, `Embarked`).
- Нормализация и масштабирование данных (если необходимо).

#### 4. Первичный анализ данных (Exploratory Data Analysis, EDA):
На этом этапе мы:
- Изучим распределение выживаемости (сколько людей выжило).
- Проведем анализ зависимостей между различными признаками и выживаемостью (например, влияние пола, возраста, класса на выживаемость).
- Построим визуализации (гистограммы, boxplots, тепловые карты и т.д.) для лучшего понимания данных.

#### 5. Построение модели машинного обучения:
Используем различные алгоритмы классификации для предсказания выживаемости:
- **Логистическая регрессия**
- **Дерево решений**
- **Методы ансамблей (Random Forest, Gradient Boosting)**
- **K-ближайших соседей (KNN)**

Сначала обучаем модели и затем оцениваем их точность.

#### 6. Оценка модели:
Оцениваем модель с использованием метрик классификации:
- **Accuracy** (точность)
- **Precision**, **Recall**, **F1-score**
- **ROC-AUC** кривая

#### 7. Улучшение модели:
Проводим гиперпараметрическую настройку с помощью GridSearch или RandomizedSearch и анализируем, какие модели лучше справляются с задачей.

