🇷🇺 **[Russian Version / На русском](README.full.ru.md)**

# 📚 Full Project List

🔙 **[Key Projects](README.md#-key-projects)**

## 🚀 All Projects

| Category | Project | Key Technologies | Core Concept & Challenges |
| :--- | :--- | :--- | :--- |
| **Production Backend** | [💰 Wallet REST API](#-wallet-rest-api-fastapi-postgresql) | FastAPI, PostgreSQL, Docker, async | Asynchronous API for financial operations with guaranteed data consistency under concurrent requests (transactions, row-level locks). |
| **AI & Intelligent Systems** | [🤖 Video Analytics Bot](#-video-analytics-bot-ai-llm-postgresql) | Aiogram, Ollama (LLM), PostgreSQL, asyncpg | NLP-powered bot: transforms natural language queries into SQL analytics using a local LLM (Mistral 7B). |
| **Machine Learning (ML) & NLP** | [🎬 Movie Recommendation System](#-movie-recommendation-system-nlp-tf-idf) | scikit-learn, pandas, TF-IDF, Aiogram | End-to-end recommendation engine based on textual features (genres, cast) with dual interfaces: Telegram bot and console app with visualization. |
| **Machine Learning (ML) & NLP** | [🔬 Embedding Playground](#-embedding-playground-ml-nlp-visualization) | Gensim, scikit-learn, Matplotlib | Interactive toolkit for deep semantic analysis of word embeddings with vector-arrow analogy visualization, semantic cluster projection (PCA/t-SNE), and evaluation on Google Analogy Test Set through an intuitive CLI. |
| **Data Research & Analysis** | [🔬 CountVectorizer Comparison](#-countvectorizer-comparison-project-nlp) | scikit-learn, NLTK, Matplotlib, Seaborn | Comparative analysis of 5 text preprocessing methods (stemming, lemmatization, etc.) for news classification. Includes evaluation by accuracy, speed, and vocabulary size. |
| **Data Research & Analysis** | [🔑 Text Keyword Extractor](#-text-keyword-extractor-tf-idf-nlp) | scikit-learn, pandas, NLTK | In-depth TF-IDF analysis: from-scratch algorithm implementation with detailed comparison (formulas, weights, ranking) against scikit-learn's version for keyword extraction. |
| **Web Services & API** | [🔗 URL Shortener Service](#-url-shortener-service-flask-rest-api) | Flask, SQLAlchemy, REST API, Alembic | Web service with REST API for generating short URLs. Features validation, custom identifier support, and history tracking in a database. |
| **Web Services & API** | [🍳 Recipe Network](#-recipe-network-django-rest-framework) | Django, Django REST Framework, Djoser, PostgreSQL, Docker | Web application for publishing cooking recipes with subscriptions, favorites, and shopping lists. Backend (API) and containerization implemented. |
| **Backend & API** | [🎗️ Funds Allocation API](#-funds-allocation-api-fastapi) | FastAPI, SQLAlchemy, JWT, Alembic, Pydantic | API for managing charitable projects with automatic donation distribution (FIFO), JWT authentication, and comprehensive documentation. |
| **Backend & API** | [👥 Social Network API](#-social-network-api-django-rest-framework) | Django, Django REST Framework, JWT, SQLite | REST API for a social network with posts, comments, subscriptions, and groups. Full JWT-based authentication. |

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


### 🔬 Embedding Playground [ML, NLP, Visualization]

**Interactive research toolkit for deep semantic analysis of word embeddings with vector-arrow visualizations of semantic relationships.** Enables intuitive exploration of semantic structure in Word2Vec and GloVe models through analogy visualization with directional arrows, semantic cluster projection, and quality evaluation.

**✨ Key Features:**
*   **Vector-Arrow Analogy Visualization:** Unique 2D plots showing semantic relationships as directional arrows (`w2 → w1` and `result → w3`), visually demonstrating parallelism in vector arithmetic (`king - man + woman = queen`).
*   **Semantic Cluster Projection:** Automatic 2D mapping of seed words and their nearest neighbors with color-coded clusters using PCA (global structure) and t-SNE (local neighborhoods).
*   **Quality Evaluation:** Testing on Google Analogy Test Set (19,544 questions) with accuracy breakdown by semantic/syntactic categories and vocabulary coverage analysis.
*   **Zero-Code Exploration:** Intuitive command-line interface with contextual help, demo mode, and persistent session — no programming required for deep semantic analysis.
*   **Smart Model Management:** Automatic download with integrity checks, mirror fallback, and binary caching for instant subsequent loads.

**🛠 Tech Stack:**
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Gensim](https://img.shields.io/badge/Gensim-3BB143?style=for-the-badge&logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=python&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)

[**📂 Project Repository**](https://github.com/IlyaShaposhnikov/embedding-playground)


### 🔬 CountVectorizer Comparison Project [NLP]

**Research project comparing the effectiveness of 5 text preprocessing methods** (stemming, lemmatization, stop-word removal, etc.) when vectorizing with `CountVectorizer` on the BBC News dataset.

**✨ Key Features:**
*   **Comparative Analysis:** Direct comparison of 5 text processing approaches by accuracy, vocabulary size, execution time, and matrix density.
*   **Deep NLP Focus:** Implementation and evaluation of linguistic methods (lemmatization, stemming).
*   **Clear Conclusions:** Identification of the optimal method that achieved a balance of accuracy and speed.
*   **Full Visualization:** Auto-generated comparative charts and tables.

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


🔙 **[Key Projects](README.md#-key-projects)**

🇷🇺 **[Russian Version / На русском](README.full.ru.md)**
