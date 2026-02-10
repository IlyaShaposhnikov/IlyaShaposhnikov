🇷🇺 [На русском / Russian Version](README.ru.md)

# 👋 Hi, my name is Ilya Shaposhnikov

**Python Developer** building backend services and integrating machine learning (**ML**) and **NLP** to solve real-world problems. I approach development as solving business problems: I value clean, maintainable architecture and measurable impact.

For **over 12 years**, I optimized complex processes at an international corporation, where I initiated and implemented IT solutions (from reporting automation to enterprise CAT system deployment). This experience shaped my **systems thinking, process analysis skills, and ability to drive projects to production** (tangible results: 90% reduction in manual effort, 70% increase in operational speed).

I apply the same mindset to Python development: I focus on building **robust, production-ready end-to-end solutions** — from designing architecture and business logic to containerization, CI/CD setup, and deployment. Below are projects I architected and implemented: from high-load APIs and modern AI/ML solutions to comprehensive web services.

## 🛠 Technology Stack

**Backend & Frameworks:**
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?logo=django&logoColor=white)
![Django REST Framework](https://img.shields.io/badge/DRF-092E20?logo=django&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?logo=flask&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?logo=python&logoColor=white)
![Alembic](https://img.shields.io/badge/Alembic-000000?logo=alembic&logoColor=white)

**Data Science & Machine Learning:**
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikit-learn&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?logo=python&logoColor=white)
![NLTK](https://img.shields.io/badge/NLTK-3BB143?logo=python&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-3BB143?logo=ollama&logoColor=white)

**Databases:**
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=white)

**DevOps & Tools:**
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![Docker Compose](https://img.shields.io/badge/Docker_Compose-2496ED?logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?logo=github-actions&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?logo=nginx&logoColor=white)
![Gunicorn](https://img.shields.io/badge/Gunicorn-499848?logo=gunicorn&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?logo=gnu-bash&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?logo=postman&logoColor=white)

**Testing:**
![Pytest](https://img.shields.io/badge/Pytest-0A9EDC?logo=pytest&logoColor=white)

**Frontend & Other:**
![HTML](https://img.shields.io/badge/HTML-E34F26?logo=html5&logoColor=white)
![REST API](https://img.shields.io/badge/REST_API-FF6C37?logo=postman&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?logo=json-web-tokens&logoColor=white)

## 🗣️ [Natural] Languages
*   🇷🇺  **Russian:** Native
*  🇬🇧🇺🇸 **English:** C2 (Proficient)
*   🇪🇸  **Spanish:** C1 (Advanced)
*   🇫🇷  **French:** B2 (Upper-Intermediate)
*   🇩🇪  **German:** B1 (Intermediate)

## 🎯 Open to Opportunities
I'm looking for a **Python Developer** role with a focus on **ML**/**NLP** projects in a product-driven team where I can bridge technical execution and business strategy—applying my tech stack and unique cross-domain experience to build efficient code that solves real-world problems.

**📍 Location:** Saint Petersburg, Russia (open to on-site, remote, and hybrid work)

**📧 Contact:** [ilia.a.shaposhnikov@gmail.com](mailto:ilia.a.shaposhnikov@gmail.com)

**📱 Telegram:** [@iliashaposhnikov](https://t.me/iliashaposhnikov)

## 🚀 Key Projects

| Category | Project | Key Technologies | Core Concept & Challenges |
| :--- | :--- | :--- | :--- |
| **Production Backend** | [💰 Wallet REST API](#-wallet-rest-api-fastapi-postgresql) | FastAPI, PostgreSQL, Docker, async | Asynchronous API for financial operations with guaranteed data consistency under concurrent requests (transactions, row-level locks). |
| **AI & Intelligent Systems** | [🤖 Video Analytics Bot](#-video-analytics-bot-ai-llm-postgresql) | Aiogram, Ollama (LLM), PostgreSQL, asyncpg | NLP-powered bot: transforms natural language queries into SQL analytics using a local LLM (Mistral 7B). |
| **Machine Learning (ML) & NLP** | [🎬 Movie Recommendation System](#-movie-recommendation-system-nlp-tf-idf) | scikit-learn, pandas, TF-IDF, Aiogram | End-to-end recommendation engine based on textual features (genres, cast) with dual interfaces: Telegram bot and console app with visualization. |
| **Data Research & Analysis** | [🔬 CountVectorizer Comparison](#-countvectorizer-comparison-project-nlp) | scikit-learn, NLTK, Matplotlib, Seaborn | Comparative analysis of 5 text preprocessing methods (stemming, lemmatization, etc.) for news classification. Includes evaluation by accuracy, speed, and vocabulary size. |
| **Data Research & Analysis** | [🔑 Text Keyword Extractor](#-text-keyword-extractor-tf-idf-nlp) | scikit-learn, pandas, NLTK | In-depth TF-IDF analysis: from-scratch algorithm implementation with detailed comparison (formulas, weights, ranking) against scikit-learn's version for keyword extraction. |
| **Web Services & API** | [🔗 URL Shortener Service](#-url-shortener-service-flask-rest-api) | Flask, SQLAlchemy, REST API, Alembic | Web service with REST API for generating short URLs. Features validation, custom identifier support, and history tracking in a database. |

### 💰 Wallet REST API [FastAPI, PostgreSQL]

**High-load asynchronous REST API for managing financial balances.** The service ensures data consistency during concurrent deposit/withdrawal operations, implementing an e-wallet pattern.

**✨ Key Features:**
*   **Concurrency Safety:** Guarantees data integrity through `READ COMMITTED` transactions and `SELECT ... FOR UPDATE` row-level locks.
*   **Production-Grade Stack:** Full cycle from asynchronous backend to containerization.
*   **Deployment Ready:** Fully configured for Docker with orchestration (`docker-compose`).
*   **Comprehensive Documentation:** Auto-generated interactive OpenAPI (Swagger) documentation at `/docs`.

**🛠 Tech Stack:**
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=for-the-badge&logo=python&logoColor=white)
![Alembic](https://img.shields.io/badge/Alembic-000000?style=for-the-badge&logo=alembic&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Pytest](https://img.shields.io/badge/Pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white)

[**📂 Project Repository**](https://github.com/IlyaShaposhnikov/wallet-api)


### 🤖 Video Analytics Bot [AI, LLM, PostgreSQL]

**Intelligent Telegram bot converting natural language queries into analytical SQL queries** for a video statistics database. Uses a local LLM (Ollama + Mistral 7B) for prompt engineering and code generation.

**✨ Key Features:**
*   **NLP Interface:** Users ask questions in natural language ("How many videos have >100K views?"), the bot returns a precise numerical answer.
*   **Local LLM:** **Mistral 7B model via Ollama** ensures complete data privacy, offline operation, and no limits/fees.
*   **Prompt Engineering:** Detailed system prompt with database schema description, strict rules, and examples for stable SQL query generation.
*   **Production Architecture:** Asynchronous bot on **Aiogram 3.7+**, optimized **PostgreSQL** with indexes, connection pooling via **asyncpg**.

**🛠 Tech Stack:**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Aiogram](https://img.shields.io/badge/Aiogram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-3BB143?style=for-the-badge&logo=ollama&logoColor=white)
![asyncpg](https://img.shields.io/badge/asyncpg-000000?style=for-the-badge&logo=postgresql&logoColor=white)

[**📂 Project Repository**](https://github.com/IlyaShaposhnikov/video_analytics_bot)


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


### 🔬 CountVectorizer Comparison Project [NLP]

**Проект для сравнения эффективности 5 методов предобработки текста** (стемминг, лемматизация, удаление стоп-слов и др.) при векторизации через `CountVectorizer` на датасете BBC News.

**✨ Ключевые особенности:**
*   **Сравнительный анализ:** Прямое сравнение 5 подходов к обработке текста по точности, размеру словаря, времени работы и плотности матрицы.
*   **Глубокий фокус на NLP:** Реализация и оценка лингвистических методов (лемматизация, стемминг).
*   **Четкие выводы:** Выявление оптимального метода, обеспечившего баланс точности и скорости.
*   **Полная визуализация:** Автоматическая генерация сравнительных графиков и таблиц.

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
