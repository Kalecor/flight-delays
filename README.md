# Flight Delays Fall 2018

## Описание проекта

Данный проект выполнен в рамках практической работы по машинному обучению на основе соревнования Kaggle **Flight Delays Fall 2018**.

Цель проекта — построить модель машинного обучения для прогнозирования задержки авиарейса более чем на 15 минут.

Метрика качества модели — **ROC AUC**.

Лучшая модель: **XGBoost**

Полученный результат:

- Validation ROC AUC: **0.7524**
- Mean Cross Validation ROC AUC: **0.7481**

---

## Используемые технологии

- Python 3.11
- NumPy
- Pandas
- Matplotlib
- Seaborn
- SciPy
- Scikit-learn
- XGBoost
- PyArrow

---

## Структура проекта

```
.
├── notebook.ipynb
├── requirements.txt
├── README.md
└── submission.csv
```

---

## Как воспроизвести решение

### 1. Клонировать репозиторий

```bash
git clone <https://github.com/Kalecor/flight-delays>
cd <flight-delays>
```

---

### 2. Установить зависимости

```bash
pip install -r requirements.txt
```

---

### 3. Скачать данные

Можно загрузить данные соревнования **Flight Delays Fall 2018** с Kaggle и разместить их в каталоге (с заменой в коде) либо файлы будут сами использоваться и подгружаться в коде:

```
/kaggle/input/competitions/flight-delays-fall-2018/
```

Необходимые файлы:

- flight_delays_train.csv.zip
- flight_delays_test.csv.zip
- sample_submission.csv.zip

---

### 4. Запустить ноутбук

Открыть Jupyter Notebook или Kaggle Notebook и выполнить все ячейки последовательно сверху вниз.

После выполнения будет автоматически:

- выполнена предобработка данных;
- проведён разведочный анализ данных (EDA);
- обучены модели Logistic Regression и XGBoost;
- выполнена оценка качества по ROC AUC;
- сформирован файл `submission.csv`.

---

## Feature Engineering

В ходе работы были созданы дополнительные признаки:

- Route;
- PartOfDay;
- DepMinute;
- LongFlight.

Также были подобраны гиперпараметры модели XGBoost.

---

## Автор Пушков Дмитрий Юрьевич
