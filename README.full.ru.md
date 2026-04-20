🇬🇧 **[English Version / На английском](README.full.md)**

# 📚 Полный каталог проектов

🔙 **[Ключевые проекты](README.ru.md#-ключевые-проекты)**

## 🚀 Все проекты

| Категория | Проект | Ключевые технологии | Суть и ключевые задачи |
| :--- | :--- | :--- | :--- |
| **Production Backend** | [💰 Wallet REST API](#-wallet-rest-api-fastapi-postgresql) | FastAPI, PostgreSQL, Docker, async | Асинхронное API для финансовых операций с гарантией консистентности данных при конкурентных запросах (транзакции, блокировки). |
| **AI & Интеллектуальные системы** | [🤖 Video Analytics Bot](#-video-analytics-bot-ai-llm-postgresql) | Aiogram, Ollama (LLM), PostgreSQL, asyncpg | Бот с NLP-интерфейсом: преобразует запросы на естественном языке в SQL-аналитику с использованием локальной LLM (Mistral 7B). |
| **Машинное обучение & NLP** | [🎬 Movie Recommendation System](#-movie-recommendation-system-nlp-tf-idf) | scikit-learn, pandas, TF-IDF, Aiogram | End-to-end система рекомендаций на основе текстовых данных (жанры, актёры) с двумя интерфейсами: Telegram-бот и консольное приложение с визуализацией. |
| **Машинное обучение & NLP** | [🔬 Embedding Visualizer](#-embedding-visualizer-ml-nlp-visualization) | Gensim, scikit-learn, Matplotlib | Интерактивный инструмент для глубокого семантического анализа эмбеддингов (векторных представлений) слов с визуализацией аналогий через векторные стрелки, визуализацией семантических кластеров (PCA/t-SNE) и оценкой качества моделей на тесте аналогий через интуитивную командную оболочку. Разработан с использованием модульной архитектуры. |
| **Исследование & Анализ данных** | [🔬 CountVectorizer Comparison](#-countvectorizer-comparison-project-nlp) | scikit-learn, NLTK, Matplotlib, Seaborn | Комплексный сравнительный анализ 5 методов предобработки текста (базовый, удаление стоп-слов, лемматизация, стемминг, простая токенизация) для задачи классификации новостей с использованием CountVectorizer. Включает оценку по точности, скорости и размеру словаря. Разработан с применением модульной архитектуры для обеспечения удобства сопровождения и читаемости кода. |
| **Исследование & Анализ данных** | [🔑 Text Keyword Extractor](#-text-keyword-extractor-tf-idf-nlp) | scikit-learn, pandas, NLTK | Сравнительный анализ TF-IDF: реализация алгоритма с нуля и детальное сравнение (формулы, веса, ранжирование) с библиотечной версией scikit-learn для извлечения ключевых слов из текстов. |
| **Исследование & Анализ данных** | [🔮 Pumpkin Price & Color Forecast](#-pumpkin-price--color-forecast-scikit-learn-pandas) | scikit-learn, pandas, matplotlib, EDA | Две прогнозные модели для сельскохозяйственной экономики: регрессия для прогноза цены и классификация для определения цвета с интерпретируемыми результатами и структурой, готовой к использованию. |
| **Веб-сервисы & API** | [🔗 URL Shortener Service](#-url-shortener-service-flask-rest-api) | Flask, SQLAlchemy, REST API, Alembic | Веб-сервис с REST API для генерации коротких ссылок. Реализована валидация, поддержка кастомных идентификаторов и хранение истории в БД. |
| **Веб-сервисы & API** | [🍳 Recipe Network](#-recipe-network-django-rest-framework) | Django, Django REST Framework, Djoser, PostgreSQL, Docker | Веб-приложение для публикации кулинарных рецептов с подписками, избранным и списком покупок. Реализован бэкенд (API) и контейнеризация. |
| **Backend & API** | [🎗️ Funds Allocation API](#-funds-allocation-api-fastapi) | FastAPI, SQLAlchemy, JWT, Alembic, Pydantic | API для управления благотворительными проектами с автоматическим распределением пожертвований (FIFO), JWT-аутентификацией и полной документацией. |
| **Backend & API** | [👥 Social Network API](#-social-network-api-django-rest-framework) | Django, Django REST Framework, JWT, SQLite | REST API для социальной сети с постами, комментариями, подписками и группами. Полная аутентификация через JWT. |

### 💰 Wallet REST API [FastAPI, PostgreSQL]

**Высоконагруженное асинхронное REST API для управления финансовыми балансами.** Сервис гарантирует консистентность данных при параллельных операциях пополнения и списания, реализуя паттерн электронного кошелька.

**✨ Ключевые особенности:**
*   **Конкурентная безопасность:** Гарантия целостности данных через транзакции `READ COMMITTED` и строковые блокировки `SELECT ... FOR UPDATE`.
*   **Производственный стек:** Полный цикл от асинхронного бэкенда до контейнеризации.
*   **Готовый к деплою:** Проект полностью настроен для запуска в Docker с оркестрацией (`docker-compose`).
*   **Полная документация:** Автоматическая генерация интерактивной документации OpenAPI (Swagger) по адресу `/docs`.

**🛠 Стек технологий:**
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=for-the-badge&logo=python&logoColor=white)
![Alembic](https://img.shields.io/badge/Alembic-000000?style=for-the-badge&logo=alembic&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Pytest](https://img.shields.io/badge/Pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white)

[**📂 Репозиторий проекта**](https://github.com/IlyaShaposhnikov/wallet-api)


### 🤖 Video Analytics Bot [AI, LLM, PostgreSQL]

**Интеллектуальный Telegram-бот, преобразующий запросы на естественном языке в аналитические SQL-запросы** к базе данных статистики видео. Использует локальную LLM (Ollama + Mistral 7B) для промпт-инжиниринга и генерации кода.

**✨ Ключевые особенности:**
*   **NLP-интерфейс:** Пользователь задаёт вопросы на естественном языке ("Сколько видео набрало >100K просмотров?"), бот возвращает точный числовой ответ.
*   **Локальная LLM:** Использование модели **Mistral 7B через Ollama** обеспечивает полную конфиденциальность данных, работу оффлайн и отсутствие лимитов/платежей.
*   **Промпт-инжиниринг:** Детальный системный промпт с описанием схемы БД, строгими правилами и примерами для стабильной генерации SQL-запросов.
*   **Production-архитектура:** Асинхронный бот на **Aiogram 3.7+**, оптимизированная **PostgreSQL** с индексами, пул соединений **asyncpg**.

**🛠 Стек технологий:**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Aiogram](https://img.shields.io/badge/Aiogram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-3BB143?style=for-the-badge&logo=ollama&logoColor=white)
![asyncpg](https://img.shields.io/badge/asyncpg-000000?style=for-the-badge&logo=postgresql&logoColor=white)

[**📂 Репозиторий проекта**](https://github.com/IlyaShaposhnikov/video_analytics_bot)


### 🎬 Movie Recommendation System [NLP, TF-IDF]

**Проект для рекомендации фильмов с двумя интерфейсами: Telegram-бот и консольное приложение.** Система анализирует описания и актерский состав, используя методы обработки естественного языка и машинного обучения.

**✨ Ключевые особенности:**
*   **Два алгоритма:** Рекомендации на основе **жанров/ключевых слов** и **взвешенного актерского состава**.
*   **Два интерфейса:** Удобный **Telegram-бот** и наглядный **консольный интерфейс** с графиками.
*   **Полный цикл:** От предобработки данных (TF-IDF) до интерактивного веб-приложения.

**🛠 Стек технологий:**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)
![Telegram Bot API](https://img.shields.io/badge/Telegram_Bot-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)

[**📂 Репозиторий проекта**](https://github.com/IlyaShaposhnikov/film-recommendation-tfidf)


### 🔬 Embedding Visualizer [ML, NLP, Visualization]

**Интерактивный исследовательский инструмент для глубокого семантического анализа эмбеддингов (векторных представлений) слов с визуализацией семантических отношений через векторные стрелки.** Разработан с использованием модульной архитектуры для повышения стабильности и удобства сопровождения. Позволяет интуитивно исследовать семантическую структуру моделей Word2Vec и GloVe через визуализацию аналогий с направленными стрелками, визуализацию семантических кластеров и оценку качества моделей.

**✨ Ключевые особенности:**
*   **Визуализация семантических кластеров:** Автоматическое 2D-отображение опорных слов и их ближайших соседей с цветовой кодировкой кластеров с использованием PCA (глобальная структура) и t-SNE (локальные окрестности).
*   **Визуализация аналогий через векторные стрелки:** Уникальные 2D-графики, отображающие семантические отношения как направленные стрелки (`man → king` и `result → woman`), наглядно демонстрирующие параллелизм в векторной арифметике (`king - man + woman = queen`).
*   **Оптимизированное управление моделями:** Автоматическая загрузка с проверкой целостности, использованием резервных зеркал и бинарным кэшированием для мгновенной загрузки при повторных запусках.
*   **Ленивая загрузка моделей**: Модели загружаются по требованию через менеджер моделей, что улучшает скорость запуска и эффективность использования памяти.
*   **Модульная архитектура**: Разделение ответственностей по слоям `services`, `presentation`, `visualization`, `data` для чистого и тестируемого кода. Централизованная конфигурация и улучшенное логгирование.
*   **Оценка качества моделей:** Тестирование на наборе Google Analogy Test Set (19 544 задачи) с разбивкой по семантическим/синтаксическим категориям и анализом покрытия словаря.
*   **Исследование без программирования:** Интуитивная командная оболочка с контекстной справкой и демо-режимом — для глубокого семантического анализа не требуется писать код.

**🛠 Стек технологий:**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Gensim](https://img.shields.io/badge/Gensim-3BB143?style=for-the-badge&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)

[**📂 Репозиторий проекта**](https://github.com/IlyaShaposhnikov/embedding-visualizer)


### 🔬 CountVectorizer Comparison Project [NLP]

**Проект для сравнения эффективности 5 методов предобработки текста** (базовый, удаление стоп-слов, лемматизация, стемминг, простая токенизация) при векторизации через `CountVectorizer` на датасете BBC News. **Разработан с использованием модульной архитектуры** для обеспечения лучшей читаемости и сопровождаемости кода.

**✨ Ключевые особенности:**
*   **Сравнительный анализ:** Прямое сравнение 5 подходов к обработке текста по точности, размеру словаря, времени работы и плотности матрицы.
*   **Глубокий фокус на NLP:** Реализация и оценка лингвистических методов (лемматизация, стемминг).
*   **Четкие выводы:** Выявление оптимального метода, обеспечившего баланс точности и скорости.
*   **Полная визуализация и отчетность:** Автоматическая генерация сравнительных графиков, таблиц и подробных CSV-отчетов.
*   **Модульная структура**: Код структурирован по отдельным модулям (`methods`, `utils`) с соблюдением принципа DRY.

**🛠 Стек технологий:**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![NLTK](https://img.shields.io/badge/NLTK-3BB143?style=for-the-badge&logo=python&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)

[**📂 Репозиторий проекта**](https://github.com/IlyaShaposhnikov/count-vectorizer)


### 🔑 Text Keyword Extractor [TF-IDF, NLP]

**Исследовательский проект по глубокому анализу алгоритма TF-IDF: собственная реализация с нуля и детальное сравнение с библиотечной реализацией scikit-learn** для задачи извлечения ключевых слов из текстовых документов (датасет BBC News).

**✨ Ключевые особенности:**
*   **TF-IDF с нуля:** Чистая, документированная реализация алгоритма TF-IDF на Python без использования сторонних библиотек для векторного представления.
*   **Сравнительный анализ алгоритмов:** Прямое, пошаговое сравнение результатов и формул собственной реализации (`idf = log(N / df)`) и оптимизированной версии scikit-learn (`idf = log((1 + N) / (1 + df)) + 1` с L2-нормализацией).
*   **Аналитический CLI:** Интерактивный консольный интерфейс для полноценного исследования: поиск документов по словам, извлечение топ-N ключевых слов с весами, сравнение реализаций TF-IDF и анализ случайных документов.
*   **Промышленные практики:** Использование `NLTK` для обработки стоп-слов, пагинация результатов, модульная архитектура и работа с реальным датасетом.

**🛠 Стек технологий:**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NLTK](https://img.shields.io/badge/NLTK-3BB143?style=for-the-badge&logo=python&logoColor=white)

[**📂 Репозиторий проекта**](https://github.com/IlyaShaposhnikov/text-keyword-extractor)


### 🔮 Pumpkin Price & Color Forecast [scikit-learn, pandas, EDA]

**Проект двойного прогнозного моделирования данных рынка тыкв в США: регрессия для прогноза цены и классификация для определения цвета, с акцентом на интерпретируемость и структуру кода, готовую к использованию.**

**✨ Ключевые особенности:**
*   **Интерпретируемые регрессионные модели:** От простой линейной (`y = kx + b`) до многомерных полиномиальных моделей с **R² = 0.969**, с понятными формулами и метриками качества (MSE, RMSE).
*   **Высокоточная классификация:** Классификатор на логистической регрессии для прогнозирования цвета тыквы с **F1 = 0.94** и **AUC = 0.975**, включая оптимизацию порога и анализ матрицы ошибок.
*   **Комплексный EDA-пайплайн:** Автоматизированный разведочный анализ с визуализацией сезонности, корреляций и распределений признаков, сохраняемый в структурированные директории.
*   **Архитектура, готовая к использованию:** Модульная структура кода (`src/`, `scripts/`, `utils/`), переиспользуемые компоненты и демо-скрипт для запуска полного пайплайна.
*   **Практическая фокусировка на сельскохозяйственной экономике:** Реальный датасет (рынок тыкв США) с практическими выводами о факторах цены (сорт, локация, упаковка) и предикторах цвета.

**🛠 Стек технологий:**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge&logo=python&logoColor=white)

[**📂 Репозиторий проекта**](https://github.com/IlyaShaposhnikov/pumpkin-price-color-forecast)


### 🔗 URL Shortener Service [Flask, REST API]

**Веб-сервис для генерации коротких ссылок с полноценным REST API и веб-интерфейсом.** Позволяет создавать как автоматически сгенерированные короткие ссылки, так и кастомные идентификаторы, с валидацией и сохранением в БД.

**✨ Ключевые особенности:**
*   **Двойной интерфейс:** Удобный **веб-интерфейс** для ручного создания ссылок и **REST API** для автоматической интеграции с другими сервисами.
*   **Гибкость создания:** Поддержка как автоматической генерации коротких ID (6 символов), так и задания **пользовательских коротких идентификаторов**.
*   **Полный цикл работы с данными:** Использование **Flask-Migrate (Alembic)** для управления версиями схемы базы данных, обеспечивая надежное хранение истории ссылок.
*   **Надежная валидация:** Встроенная проверка корректности исходных URL и кастомных идентификаторов через **Flask-WTF** и **WTForms**.

**🛠 Стек технологий:**
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=for-the-badge&logo=python&logoColor=white)
![Alembic](https://img.shields.io/badge/Alembic-000000?style=for-the-badge&logo=alembic&logoColor=white)
![REST API](https://img.shields.io/badge/REST_API-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![Jinja2](https://img.shields.io/badge/Jinja2-B41717?style=for-the-badge&logo=jinja&logoColor=white)

[**📂 Репозиторий проекта**](https://github.com/IlyaShaposhnikov/shortlink_generator)


### 🍳 Recipe Network [Django, Django REST Framework]

**Веб-приложение для публикации кулинарных рецептов с подписками, избранным и списком покупок.** В рамках проекта была реализована бэкенд-часть (API), настроена контейнеризация (Docker) и CI/CD.

**✨ Ключевые особенности:**
*   **Полнофункциональный API:** Реализованы все необходимые эндпоинты для регистрации, аутентификации, работы с рецептами, подписками, избранным и списком покупок.
*   **Аутентификация и авторизация:** Использование Djoser для управления пользователями, JWT-токены.
*   **Работа с данными:** Возможность загрузки ингредиентов из JSON-файла, фильтрация по тегам, пагинация.
*   **Готовность к деплою:** Настроена контейнеризация с помощью Docker и Docker Compose, подготовлен CI/CD пайплайн (GitHub Actions) для автоматического развертывания.

**🛠 Стек технологий (Backend):**
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
![Django REST Framework](https://img.shields.io/badge/DRF-092E20?style=for-the-badge&logo=django&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)

[**📂 Репозиторий проекта**](https://github.com/IlyaShaposhnikov/recipe_network)


### 🎗️ Funds Allocation API [FastAPI, SQLAlchemy]

**API-приложение для управления благотворительными проектами и автоматического распределения пожертвований.** Реализована система с алгоритмом FIFO (First In, First Out) для справедливого распределения средств между проектами.

**✨ Ключевые особенности:**
*   **Автоматическое распределение пожертвований:** Реализован алгоритм FIFO для распределения входящих пожертвований между открытыми проектами, гарантирующий прозрачность и предсказуемость.
*   **Полноценная система аутентификации:** Использование JWT-токенов для защиты API-эндпоинтов, с поддержкой суперпользователей и ролевой моделью.
*   **Профессиональная структура проекта:** Четкое разделение на модули (API, CRUD, модели, схемы, сервисы) с использованием асинхронного SQLAlchemy 2.0.
*   **Полная документация:** Автоматическая генерация интерактивной документации OpenAPI (Swagger UI и ReDoc) по адресам `/docs` и `/redoc`.
*   **Готовность к разработке:** Настроена система миграций через Alembic, конфигурация через переменные окружения, валидация данных через Pydantic.

**🛠 Стек технологий:**
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=for-the-badge&logo=python&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)
![Alembic](https://img.shields.io/badge/Alembic-000000?style=for-the-badge&logo=alembic&logoColor=white)
![Pydantic](https://img.shields.io/badge/Pydantic-92000?style=for-the-badge&logo=pydantic&logoColor=white)

[**📂 Репозиторий проекта**](https://github.com/IlyaShaposhnikov/funds_allocation_system)


### 👥 Social Network API [Django, Django REST Framework]

**REST API для социальной сети с функционалом публикации постов, комментариев, подписок и управления группами.** Предоставляет полный набор эндпоинтов для взаимодействия с платформой, используя современную аутентификацию по JWT-токенам.

**✨ Ключевые особенности:**
*   **Полнофункциональный API для социальной сети:** Реализованы все необходимые CRUD-операции для работы с постами, комментариями, группами и подписками.
*   **Современная аутентификация:** Использование JWT-токенов (Simple JWT) с разделением на access и refresh токены для безопасной работы с API.
*   **Четкая структура эндпоинтов:** RESTful архитектура с логичной иерархией URL (например, `/api/v1/posts/{id}/comments/` для комментариев к конкретному посту).
*   **Полная документация:** Все доступные методы API описаны в README проекта с примерами запросов и ответов, что упрощает интеграцию для сторонних разработчиков.

**🛠 Стек технологий:**
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
![Django REST Framework](https://img.shields.io/badge/DRF-092E20?style=for-the-badge&logo=django&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)

[**📂 Репозиторий проекта**](https://github.com/IlyaShaposhnikov/social_network_api)


🔙 **[Ключевые проекты](README.ru.md#-ключевые-проекты)**

🇬🇧 **[English Version / На английском](README.full.md)**
