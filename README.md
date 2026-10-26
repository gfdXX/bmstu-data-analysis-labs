# Анализ данных и машинное обучение — лабораторные работы

![Python](https://img.shields.io/badge/Python-3.10-3776AB?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-notebooks-F37626?logo=jupyter&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-F7931E?logo=scikitlearn&logoColor=white)
![BMSTU](https://img.shields.io/badge/МГТУ_им._Баумана-ИУ7-0a4a8f)

Три лабораторные на одном датасете — пассажиры «Титаника» (цель: `survived`). Магистратура МГТУ им. Н.Э. Баумана, весна 2026.
Ноутбуки сохранены с результатами, поэтому графики и метрики видны прямо на GitHub.

| Работа | Ноутбук | Что сделано |
|---|---|---|
| ЛР1. Визуализация | [lab1_titanic.ipynb](lab1-visualization/lab1_titanic.ipynb) | пропуски, очистка, выбросы по IQR, кодирование и масштабирование, корреляции, снижение размерности PCA / t-SNE / MDS |
| ЛР2. Классификация | [lab2_titanic.ipynb](lab2-classification/lab2_titanic.ipynb) | случайный лес и XGBoost, стратифицированная кросс-валидация, матрицы ошибок, accuracy / F1 / ROC-AUC, подбор гиперпараметров `GridSearchCV` |
| ЛР3. Кластеризация | [lab3_titanic.ipynb](lab3-clustering/lab3_titanic.ipynb) | t-SNE, KMeans и DBSCAN с подбором параметров, оценка качества кластеризации |

В [extra-wine-quality-visualization](extra-wine-quality-visualization) — первый вариант ЛР1 на датасете [Wine Quality (UCI)](https://archive.ics.uci.edu/dataset/186/wine+quality): EDA, PCA, t-SNE, UMAP, MDS.

## Как запустить

```bash
python -m venv .venv
.venv\Scripts\activate          # Linux/macOS: source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook
```

Датасет Titanic загружается через `seaborn.load_dataset("titanic")`, отдельный файл не нужен.

## Автор

Салженикин Даниил, МГТУ им. Н.Э. Баумана.
