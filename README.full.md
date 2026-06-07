🇷🇺 **[Russian Version / На русском](README.full.ru.md)**

# 📚 Full Project List

🔙 **[Key Projects](README.md#-key-projects)**

## 🚀 All Projects

| Category | Project | Key Technologies | Core Concept & Challenges |
| :--- | :--- | :--- | :--- |
| **AI & LLM Systems** | [🤖 Video Analytics Bot](#-video-analytics-bot-ai-llm-postgresql) | Aiogram, Ollama (LLM), PostgreSQL, asyncpg | NLP-powered bot: transforms natural language queries into SQL analytics using a local LLM (Mistral 7B) with prompt engineering and few-shot examples. |
| **ML/NLP Pipeline** | [✈️ Airline Sentiment Analysis Pipeline](#-airline-sentiment-analysis-pipeline-ml-nlp-fastapi-streamlit) | FastAPI, Streamlit, scikit-learn, TF-IDF, SHAP, pytest | End-to-end sentiment classification pipeline with confidence-weighted training, explainable predictions (SHAP), production REST API, interactive Streamlit dashboard, and CI/CD with >90% test coverage. |
| **ML & NLP** | [🔬 Embedding Visualizer](#-embedding-visualizer-ml-nlp-visualization) | Gensim, scikit-learn, Matplotlib | Interactive toolkit for deep semantic analysis of word embeddings with vector-arrow analogy visualization, semantic cluster projection (PCA/t-SNE), and evaluation on Google Analogy Test Set through an intuitive CLI. Built with a robust, modular architecture. |
| **ML & NLP** | [🎬 Movie Recommendation System](#-movie-recommendation-system-nlp-tf-idf) | scikit-learn, pandas, TF-IDF, Aiogram | End-to-end recommendation engine based on textual features (genres, cast) with dual interfaces: Telegram bot and console app with visualization. |
| **ML & NLP** | [🚫 SMS Spam Detector](#-sms-spam-detector-ml-nlp-cli) | scikit-learn, pandas, CLI | Modular pipeline for binary SMS classification using Naive Bayes/Logistic Regression, featuring CLI interface, structured logging, artifact persistence, and interpretability via confusion matrices and word clouds. |
| **NLP Research** | [🔬 CountVectorizer Comparison](#-countvectorizer-comparison-project-nlp) | scikit-learn, NLTK, Matplotlib, Seaborn | Comprehensive comparative analysis of 5 text preprocessing methods (basic, stop-word removal, lemmatization, stemming, simple tokenization) for news classification using CountVectorizer. Includes evaluation by accuracy, speed, and vocabulary size. |
| **NLP Research** | [🔑 Text Keyword Extractor](#-text-keyword-extractor-tf-idf-nlp) | scikit-learn, pandas, NLTK | In-depth TF-IDF analysis: from-scratch algorithm implementation with detailed comparison (formulas, weights, ranking) against scikit-learn's version for keyword extraction. |
| **ML Research** | [🔮 Pumpkin Price & Color Forecast](#-pumpkin-price--color-forecast-scikit-learn-pandas-eda) | scikit-learn, pandas, matplotlib, EDA | Dual predictive models for agricultural economics: regression for price forecasting (R² = 0.969) and classification for color prediction (F1 = 0.94) with interpretable outputs and production-ready structure. |
| **Production Backend (MLOps)** | [💰 Wallet REST API](#-wallet-rest-api-fastapi-postgresql) | FastAPI, PostgreSQL, Docker, async | Asynchronous API for financial operations with guaranteed data consistency under concurrent requests (transactions, row-level locks). *Demonstrates production-grade engineering skills required for deploying ML models at scale.* |
| **Backend & API** | [🎗️ Funds Allocation API](#-funds-allocation-api-fastapi) | FastAPI, SQLAlchemy, JWT, Alembic, Pydantic | API for managing charitable projects with automatic donation distribution (FIFO), JWT authentication, and comprehensive documentation. |
| **Web Services & API** | [🍳 Recipe Network](#-recipe-network-django-rest-framework) | Django, Django REST Framework, Djoser, PostgreSQL, Docker | Web application for publishing cooking recipes with subscriptions, favorites, and shopping lists. Backend (API) and containerization implemented. |
| **Backend & API** | [👥 Social Network API](#-social-network-api-django-rest-framework) | Django, Django REST Framework, JWT, SQLite | REST API for a social network with posts, comments, subscriptions, and groups. Full JWT-based authentication. |
| **Web Services & API** | [🔗 URL Shortener Service](#-url-shortener-service-flask-rest-api) | Flask, SQLAlchemy, REST API, Alembic | Web service with REST API for generating short URLs. Features validation, custom identifier support, and history tracking in a database. |

### 🤖 Video Analytics Bot [AI, LLM, PostgreSQL]

**Intelligent Telegram bot converting natural language queries into analytical SQL queries** for a video statistics database. Uses a local LLM (Ollama + Mistral 7B) for prompt engineering and code generation.

**✨ Key Features:**
*   **NLP Interface:** Users ask questions in natural language ("How many videos have >100K views?"), the bot returns a precise numerical answer.
*   **Local LLM:** **Mistral 7B model via Ollama** ensures complete data privacy, offline operation, and no limits/fees.
*   **Prompt Engineering:** Detailed system prompt with database schema description, strict rules, and few-shot examples for stable SQL query generation.
*   **Production Architecture:** Asynchronous bot on **Aiogram 3.7+**, optimized **PostgreSQL** with indexes, connection pooling via **asyncpg**.

**🛠 Tech Stack:**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Aiogram](https://img.shields.io/badge/Aiogram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-3BB143?style=for-the-badge&logo=ollama&logoColor=white)
![asyncpg](https://img.shields.io/badge/asyncpg-000000?style=for-the-badge&logo=postgresql&logoColor=white)

[**📂 Project Repository**](https://github.com/IlyaShaposhnikov/video_analytics_bot)


### ✈️ Airline Sentiment Analysis Pipeline [ML, NLP, FastAPI, Streamlit]

**Production-ready end-to-end ML pipeline for airline tweet sentiment classification** with confidence-aware training, explainable AI, async REST API, and interactive dashboard.

**✨ Key Features:**
*   **Confidence-Aware Training**: Sample weighting based on annotation confidence scores for more robust model learning.
*   **Explainable Predictions**: Per-prediction insights via top contributing words and optional SHAP value visualizations.
*   **Production REST API**: Async-safe FastAPI service with Pydantic v2 validation, thread-safe model serving, CORS support, and timeout handling.
*   **Interactive Dashboard**: Streamlit UI for single/batch predictions with CSV/JSON export, real-time health checks, and session persistence.
*   **Comprehensive Testing**: >90% coverage with unit/integration tests, GitHub Actions CI, security auditing via pip-audit.
*   **Modular Architecture**: Clean separation of data loading, preprocessing, modeling, API, and dashboard layers with centralized config management.

**🛠 Tech Stack:**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NLTK](https://img.shields.io/badge/NLTK-3BB143?style=for-the-badge&logo=python&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)

[**📂 Project Repository**](https://github.com/IlyaShaposhnikov/airline-sentiment-analysis)


### 🔬 Embedding Visualizer [ML, NLP, Visualization]

**Interactive research toolkit for deep semantic analysis of word embeddings with vector-arrow visualizations of semantic relationships.** Built with a robust, modular architecture for enhanced stability and maintainability. Enables intuitive exploration of semantic structure in Word2Vec and GloVe models through analogy visualization with directional arrows, semantic cluster projection, and quality evaluation.

**✨ Key Features:**
*   **Semantic Cluster Projection:** Automatic 2D mapping of seed words and their nearest neighbors with color-coded clusters using PCA (global structure) and t-SNE (local neighborhoods).
*   **Vector-Arrow Analogy Visualization:** Unique 2D plots showing semantic relationships as directional arrows (`w2 → w1` and `result → w3`), visually demonstrating parallelism in vector arithmetic (`king - man + woman = queen`).
*   **Smart Model Management:** Automatic download with integrity checks, mirror fallback, and binary caching for instant subsequent loads.
*   **Lazy Model Loading**: Models load on demand via Model Manager, improving startup speed and memory efficiency.
*   **Robust Modular Architecture**: Separated concerns across `services`, `presentation`, `visualization`, and `data` layers for clean, testable code. Centralized configuration and enhanced logging.
*   **Quality Evaluation:** Testing on Google Analogy Test Set (19,544 questions) with accuracy breakdown by semantic/syntactic categories and vocabulary coverage analysis.
*   **Zero-Code Exploration:** Intuitive command-line interface with contextual help, demo mode, and persistent session — no programming required for deep semantic analysis.

**🛠 Tech Stack:**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Gensim](https://img.shields.io/badge/Gensim-3BB143?style=for-the-badge&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)

[**📂 Project Repository**](https://github.com/IlyaShaposhnikov/embedding-visualizer)


### 🎬 Movie Recommendation System [NLP, TF-IDF]

**Film recommendation engine with dual UI: Telegram bot and console application.** The system analyzes descriptions and cast using NLP and ML techniques.

**✨ Key Features:**
*   **Two Algorithms:** Recommendations based on **genres/keywords** and **weighted cast analysis**.
*   **Two Interfaces:** Convenient **Telegram bot** and a visual **console interface** with charts.
*   **End-to-End Pipeline:** From data preprocessing (TF-IDF) to an interactive web application.

**🛠 Tech Stack:**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)
![Telegram Bot API](https://img.shields.io/badge/Telegram_Bot-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)

[**📂 Project Repository**](https://github.com/IlyaShaposhnikov/film-recommendation-tfidf)


### 🚫 SMS Spam Detector [ML, NLP, CLI]

**Modular pipeline for binary SMS classification using scikit-learn vectorizers and probabilistic models**, designed with production-ready patterns and an intuitive command-line interface.

**✨ Key Features:**
*   **Flexible Model Selection**: Support for **Naive Bayes** (fast baseline) and **Logistic Regression** (higher accuracy) via `--model` CLI argument.
*   **Adaptive Vectorization**: Switch between **CountVectorizer** and **TfidfVectorizer** with configurable n-grams, max features, and stop-word handling.
*   **Comprehensive Evaluation**: Automated calculation of accuracy, F1, precision, recall, and ROC-AUC with JSON export for experiment tracking.
*   **Interpretability Tools**: Confusion matrix visualization via sklearn's `ConfusionMatrixDisplay`, word clouds for spam/ham analysis, and misclassification inspection with probability scores.
*   **CLI-Driven Workflow**: Full pipeline execution via `python scripts/train.py` with argparse validation, reproducibility via `--random-state`, and optional plot generation.
*   **Production Patterns**: Structured logging to console + file, graceful error handling with exit codes, and artifact persistence (models, metrics, plots) with timestamps.
*   **Modular Architecture**: Clean separation of concerns across `data`, `features`, `models`, `evaluation`, and `visualization` modules for maintainable, testable code.

**🛠 Tech Stack:**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge&logo=python&logoColor=white)

[**📂 Project Repository**](https://github.com/IlyaShaposhnikov/sms-spam-detector)


### 🔬 CountVectorizer Comparison Project [NLP]

**Research project comparing the effectiveness of 5 text preprocessing methods** (basic, stop-word removal, lemmatization, stemming, simple tokenization) when vectorizing with `CountVectorizer` on the BBC News dataset. **Built with a modular architecture** for enhanced readability and maintainability.

**✨ Key Features:**
*   **Comparative Analysis:** Direct comparison of 5 text processing approaches by accuracy, vocabulary size, execution time, and matrix density.
*   **Deep NLP Focus:** Implementation and evaluation of linguistic methods (lemmatization, stemming).
*   **Clear Conclusions:** Identification of the optimal method that achieved a balance of accuracy and speed.
*   **Full Visualization & Reporting:** Auto-generated comparative charts, tables, and detailed CSV reports.
*   **Modular Design**: Code structured into dedicated modules (`methods`, `utils`) following DRY principles.

**🛠 Tech Stack:**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![NLTK](https://img.shields.io/badge/NLTK-3BB143?style=for-the-badge&logo=python&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)

[**📂 Project Repository**](https://github.com/IlyaShaposhnikov/count-vectorizer)


### 🔑 Text Keyword Extractor [TF-IDF, NLP]

**Research project conducting in-depth analysis of the TF-IDF algorithm: from-scratch implementation with detailed comparison against scikit-learn's version** for extracting keywords from text documents (BBC News dataset).

**✨ Key Features:**
*   **TF-IDF from Zero:** Clean, documented pure-Python implementation without using third-party libraries for vector representation.
*   **Algorithm Comparison:** Step-by-step comparison of manual TF-IDF (`idf = log(N / df)`) vs. scikit-learn's optimized TF-IDF (`idf = log((1 + N) / (1 + df)) + 1` with L2 normalization).
*   **Analytical CLI:** Interactive console interface for comprehensive exploration: document search by terms, top-N keyword extraction with weights, TF-IDF comparison, and random document analysis.
*   **Industry Practices:** `NLTK` for stop-word processing, result pagination, modular architecture, and real-world dataset usage.

**🛠 Tech Stack:**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NLTK](https://img.shields.io/badge/NLTK-3BB143?style=for-the-badge&logo=python&logoColor=white)

[**📂 Project Repository**](https://github.com/IlyaShaposhnikov/text-keyword-extractor)


### 🔮 Pumpkin Price & Color Forecast [scikit-learn, pandas, EDA]

**Dual predictive modeling project for US agricultural market data: regression for pumpkin price forecasting and classification for color prediction, with emphasis on interpretability and production-ready code.**

**✨ Key Features:**
*   **Interpretable Regression Models:** From simple linear (`y = kx + b`) to multivariate polynomial models achieving **R² = 0.969**, with clear formulas and performance metrics (MSE, RMSE).
*   **High-Accuracy Classification:** Logistic regression classifier predicting pumpkin color with **F1 = 0.94** and **AUC = 0.975**, including threshold optimization and confusion matrix analysis.
*   **Comprehensive EDA Pipeline:** Automated exploratory analysis with visualizations of seasonality, correlations, and feature distributions saved to structured output directories.
*   **Production-Ready Architecture:** Modular code structure (`src/`, `scripts/`, `utils/`), reusable components, and demo script for end-to-end pipeline execution.
*   **Practical Agricultural Economics Focus:** Real-world dataset (US pumpkin market) with actionable insights on price drivers (variety, location, packaging) and color predictors.

**🛠 Tech Stack:**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge&logo=python&logoColor=white)

[**📂 Project Repository**](https://github.com/IlyaShaposhnikov/pumpkin-price-color-forecast)


### 💰 Wallet REST API [FastAPI, PostgreSQL]

**High-load asynchronous REST API for managing financial balances.** The service ensures data consistency during concurrent deposit/withdrawal operations, implementing an e-wallet pattern. *This project demonstrates my ability to write production-grade, concurrent backend code — essential for deploying ML models at scale and handling high-throughput inference workloads.*

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


### 🎗️ Funds Allocation API [FastAPI, SQLAlchemy]

**An API application for managing charitable projects and automatically distributing donations.** The system implements a FIFO (First In, First Out) algorithm for fair distribution of funds among projects.

**✨ Key Features:**
*   **Automatic Donation Distribution:** Implemented FIFO algorithm for distributing incoming donations among open projects, ensuring transparency and predictability.
*   **Comprehensive Authentication System:** Using JWT tokens to protect API endpoints, with support for superusers and a role model.
*   **Professional Project Structure:** Clear separation into modules (API, CRUD, models, schemas, services) using asynchronous SQLAlchemy 2.0.
*   **Full Documentation:** Auto-generated interactive OpenAPI documentation (Swagger UI and ReDoc) at `/docs` and `/redoc`.
*   **Development Ready:** Configured migration system via Alembic, configuration via environment variables, data validation via Pydantic.

**🛠 Tech Stack:**
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=for-the-badge&logo=python&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)
![Alembic](https://img.shields.io/badge/Alembic-000000?style=for-the-badge&logo=alembic&logoColor=white)
![Pydantic](https://img.shields.io/badge/Pydantic-92000?style=for-the-badge&logo=pydantic&logoColor=white)

[**📂 Project Repository**](https://github.com/IlyaShaposhnikov/funds_allocation_system)


### 🍳 Recipe Network [Django, Django REST Framework]

**A web application for publishing cooking recipes with subscriptions, favorites, and shopping lists.** The project involved implementing the backend (API), containerization (Docker), and CI/CD setup.

**✨ Key Features:**
*   **Full-Featured API:** All necessary endpoints implemented for registration, authentication, working with recipes, subscriptions, favorites, and shopping lists.
*   **Authentication & Authorization:** Using Djoser for user management, JWT tokens.
*   **Data Management:** Ability to load ingredients from a JSON file, filtering by tags, pagination.
*   **Deployment Ready:** Configured containerization with Docker and Docker Compose, prepared a CI/CD pipeline (GitHub Actions) for automatic deployment.

**🛠 Tech Stack (Backend):**
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
![Django REST Framework](https://img.shields.io/badge/DRF-092E20?style=for-the-badge&logo=django&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)

[**📂 Project Repository**](https://github.com/IlyaShaposhnikov/recipe_network)


### 👥 Social Network API [Django, Django REST Framework]

**A REST API for a social network with functionality for publishing posts, comments, subscriptions, and group management.** Provides a complete set of endpoints for interacting with the platform, using modern JWT token authentication.

**✨ Key Features:**
*   **Full-Featured Social Network API:** All necessary CRUD operations implemented for working with posts, comments, groups, and subscriptions.
*   **Modern Authentication:** Using JWT tokens (Simple JWT) with separation of access and refresh tokens for secure API interaction.
*   **Clear Endpoint Structure:** RESTful architecture with logical URL hierarchy (e.g., `/api/v1/posts/{id}/comments/` for comments on a specific post).
*   **Comprehensive Documentation:** All available API methods are described in the project README with request and response examples, simplifying integration for third-party developers.

**🛠 Tech Stack:**
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
![Django REST Framework](https://img.shields.io/badge/DRF-092E20?style=for-the-badge&logo=django&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)

[**📂 Project Repository**](https://github.com/IlyaShaposhnikov/social_network_api)


### 🔗 URL Shortener Service [Flask, REST API]

**Web service for generating short URLs with a full-featured REST API and web interface.** Supports both auto-generated short links and custom identifiers, with validation and storage in a database.

**✨ Key Features:**
*   **Dual Interface:** User-friendly **web interface** for manual link creation and **REST API** for automated integration with other services.
*   **Creation Flexibility:** Both auto-generated short IDs (6 characters) and **custom short identifiers**.
*   **Full Data Lifecycle:** **Flask-Migrate (Alembic)** for database schema versioning, ensuring reliable storage of link history.
*   **Robust Validation:** Built-in validation of source URLs and custom identifiers via **Flask-WTF** and **WTForms**.

**🛠 Tech Stack:**
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=for-the-badge&logo=python&logoColor=white)
![Alembic](https://img.shields.io/badge/Alembic-000000?style=for-the-badge&logo=alembic&logoColor=white)
![REST API](https://img.shields.io/badge/REST_API-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![Jinja2](https://img.shields.io/badge/Jinja2-B41717?style=for-the-badge&logo=jinja&logoColor=white)

[**📂 Project Repository**](https://github.com/IlyaShaposhnikov/shortlink_generator)


🔙 **[Key Projects](README.md#-key-projects)**

🇷🇺 **[Russian Version / На русском](README.full.ru.md)**
