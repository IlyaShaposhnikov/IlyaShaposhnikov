🇬🇧 **[English Version / На английском](README.md)**

# 👋 Привет, я Илья Шапошников

**ML/NLP/LLM-инженер**: создаю готовые к промышленной эксплуатации системы машинного обучения и интеллектуальные приложения для работы с языком. Сочетаю **лингвистическое образование** с сильной инженерной базой, чтобы доводить ML-решения от исследовательского ноутбука до продакшена.

**Моя специализация** — **надежные ML-пайплайны полного цикла**: от предобработки текста и обучения моделей до строгой оценки качества, объяснимости (SHAP), контейнеризации, CI/CD и деплоя. Ниже — проекты, которые я спроектировал и реализовал: **система триажа GitHub issues**, где сравниваются дообученный трансформер, эмбеддинги и TF-IDF, а дубликаты ищутся векторным поиском; сравнительное исследование **тематического моделирования** (LDA/NMF/LSA) на 20 тыс. аннотаций arXiv; сквозной **пайплайн анализа тональности** со сравнением TF-IDF и sentence-эмбеддингов, логистической регрессии и MLP на PyTorch; аналитический бот на локальной LLM и мультиязычный **экстрактивный суммаризатор**. У четырех из них есть **онлайн-демо**.

## Почему NLP и ML?

Мой путь в ML был нестандартным, и именно в этом мое преимущество. Имея базу в **лингвистике и восточных языках**, я более **12 лет** работал с языковыми данными в международной корпорации: управлял процессами машинного перевода (NMT), CAT-системами, терминологическими базами и памятью переводов. Я видел изнутри, как движутся языковые данные, где прячутся лингвистические _узкие места_ и как автоматизация экономит тысячи часов.

Понимание того, как устроен язык — от морфологии до семантики, — естественным образом привело меня в машинное обучение. Сегодня я сочетаю лингвистическое чутье с современной ML-разработкой, чтобы создавать системы, которые по-настоящему понимают человеческий язык.

## 🚀 Ключевые проекты

| Категория | Проект | Ключевые технологии | Суть и ключевые задачи |
| :--- | :--- | :--- | :--- |
| **NLP и семантический поиск** | [🧭 TriageLens](README.full.ru.md#-triagelens-ml-nlp-semantic-search) | Transformers (DistilBERT), Sentence-Transformers, Chroma, BM25, scikit-learn, Streamlit | Классификация типа и поиск дубликатов на 38 тыс. реальных GitHub issues (uv, pandas): векторный поиск (bge-small) находит оригинал в топ-10 для 52–58% дубликатов против 27–33% у BM25; сравнение дообученного DistilBERT, TF-IDF и zero-shot без утечки метки и с разбиением по времени. Демо с еженедельным обновлением индекса, 140+ тестов. |
| **NLP-исследование** | [🔎 TopicLens](README.full.ru.md#-topiclens-ml-nlp-topic-modeling) | scikit-learn, NLTK, Plotly, Streamlit, pytest | Сравнение LDA, NMF и LSA на 20 тыс. аннотаций arXiv (2018–2026): когерентность, разнообразие тем и согласие с реальными категориями, сопоставление тем между моделями венгерским алгоритмом, динамика тем за 8 лет. Демо с ежемесячным автообновлением, 280+ тестов. |
| **NLP-пайплайн** | [✈️ Airline Sentiment Analysis](README.full.ru.md#%EF%B8%8F-airline-sentiment-analysis-pipeline-ml-nlp-fastapi-streamlit) | scikit-learn, PyTorch, Sentence-Transformers, FastAPI, Streamlit, SHAP | TF-IDF против sentence-эмбеддингов × логистическая регрессия против MLP на PyTorch на 5 случайных разбиениях: эмбеддинги дают +2–3 п.п. macro-F1 ценой ~40× задержки. Взвешивание примеров по уверенности разметчиков, SHAP-объяснения, REST API, дашборд для сравнения моделей. Демо, 290+ тестов. |
| **LLM-приложение** | [🤖 Video Analytics Bot](README.full.ru.md#-video-analytics-bot-ai-llm-postgresql) | Aiogram, Ollama (LLM), PostgreSQL, asyncpg | Бот, который переводит вопросы на естественном языке в SQL-запросы для аналитики с помощью локальной LLM (Mistral 7B), промпт-инжиниринга и few-shot примеров. |
| **NLP-приложение** | [🌍 Polyglot Extractive Summarizer](README.full.ru.md#-polyglot-extractive-summarizer-nlp-textrank-streamlit) | sumy (TextRank), NLTK, Streamlit, wikipedia-api | Мультиязычный (5 языков) экстрактивный суммаризатор статей Википедии и локальных файлов с гибкой настройкой длины, веб-интерфейсом на Streamlit с демо и CLI. |
| **Backend и API** | [💰 Wallet REST API](README.full.ru.md#-wallet-rest-api-fastapi-postgresql) | FastAPI, PostgreSQL, Docker, async | Асинхронный API для финансовых операций с гарантией консистентности данных при конкурентных запросах. *Бэкенд-основа для обслуживания ML-моделей под конкурентной нагрузкой.* |

▶️ **Демо:** [🧭 TriageLens](https://triage-lens.streamlit.app/) · [🔎 TopicLens](https://topic-lens.streamlit.app/) · [✈️ Airline Sentiment Analysis](https://airline-sentiment-lab.streamlit.app/) · [🌍 Polyglot Extractive Summarizer](https://polyglot-extractive-summarizer.streamlit.app/)

📚 **[Полный список проектов](README.full.ru.md)** — все проекты с подробными описаниями


## 🛠 Технологический стек

| Категория | Технологии |
|-----------|------------|
| **ML, NLP и LLM** | ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikit-learn&logoColor=white) ![pandas](https://img.shields.io/badge/pandas-150458?logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/NumPy-013243?logo=numpy&logoColor=white) ![Gensim](https://img.shields.io/badge/Gensim-3BB143?logo=python&logoColor=white) ![NLTK](https://img.shields.io/badge/NLTK-3BB143?logo=python&logoColor=white) ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white) ![Sentence-Transformers](https://img.shields.io/badge/Sentence--Transformers-FFD21E?logo=huggingface&logoColor=black) ![Transformers](https://img.shields.io/badge/Transformers-FFD21E?logo=huggingface&logoColor=black) ![Hugging Face Hub](https://img.shields.io/badge/Hugging_Face_Hub-FFD21E?logo=huggingface&logoColor=black) ![Ollama](https://img.shields.io/badge/Ollama-3BB143?logo=ollama&logoColor=white) ![SHAP](https://img.shields.io/badge/SHAP-FF8C00?logo=python&logoColor=white) ![SciPy](https://img.shields.io/badge/SciPy-654FF0?logo=scipy&logoColor=white) ![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?logo=python&logoColor=white) ![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?logo=python&logoColor=white) ![Plotly](https://img.shields.io/badge/Plotly-3F4F75?logo=plotly&logoColor=white) ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?logo=streamlit&logoColor=white) |
| **Backend и MLOps** | ![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white) ![Django](https://img.shields.io/badge/Django-092E20?logo=django&logoColor=white) ![Django REST Framework](https://img.shields.io/badge/DRF-092E20?logo=django&logoColor=white) ![Flask](https://img.shields.io/badge/Flask-000000?logo=flask&logoColor=white) ![Aiogram](https://img.shields.io/badge/Aiogram-26A5E4?logo=telegram&logoColor=white) ![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?logo=python&logoColor=white) ![Alembic](https://img.shields.io/badge/Alembic-000000?logo=alembic&logoColor=white) ![Pydantic](https://img.shields.io/badge/Pydantic-E92063?logo=pydantic&logoColor=white) |
| **Базы данных** | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white) ![asyncpg](https://img.shields.io/badge/asyncpg-000000?logo=postgresql&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white) ![SQLite](https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=white) ![Chroma](https://img.shields.io/badge/Chroma_(Vector_DB)-FF6446?logo=python&logoColor=white) |
| **DevOps, тестирование и инструменты** | ![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white) ![Docker Compose](https://img.shields.io/badge/Docker_Compose-2496ED?logo=docker&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?logo=github-actions&logoColor=white) ![Nginx](https://img.shields.io/badge/Nginx-009639?logo=nginx&logoColor=white) ![Gunicorn](https://img.shields.io/badge/Gunicorn-499848?logo=gunicorn&logoColor=white) ![Bash](https://img.shields.io/badge/Bash-4EAA25?logo=gnu-bash&logoColor=white) ![Pytest](https://img.shields.io/badge/Pytest-0A9EDC?logo=pytest&logoColor=white) |
| **API и безопасность** | ![REST API](https://img.shields.io/badge/REST_API-FF6C37?logo=postman&logoColor=white) ![JWT](https://img.shields.io/badge/JWT-000000?logo=json-web-tokens&logoColor=white) ![Postman](https://img.shields.io/badge/Postman-FF6C37?logo=postman&logoColor=white) ![GraphQL](https://img.shields.io/badge/GraphQL-E10098?logo=graphql&logoColor=white) |

## 🗣️ [Естественные] языки
*   🇷🇺  **Русский:** Родной
*   🇬🇧  **Английский:** C2 (В совершенстве)
*   🇪🇸  **Испанский:** C1 (Продвинутый)
*   🇫🇷  **Французский:** B2 (Средне-продвинутый)
*   🇩🇪  **Немецкий:** B1 (Средний)
*   🇸🇦  **Арабский:** B1 (Средний)

*Мультиязычность дает мне практическое преимущество в NLP — я на практике понимаю морфологию, синтаксис и семантику разных языковых семей.*

## 🎯 Открыт к предложениям
Ищу позицию **ML/NLP/LLM-инженера** в продуктовой команде, где смогу применить сочетание **лингвистической интуиции, опыта в ML и промышленной разработки**, чтобы создавать интеллектуальные системы для реальных задач бизнеса.

**📍 Город:** Санкт-Петербург (готов к работе в офисе, удаленно и в гибридном формате)

**📧 Почта:** [ilia.a.shaposhnikov@gmail.com](mailto:ilia.a.shaposhnikov@gmail.com)

**📱 Telegram:** [@iliashaposhnikov](https://t.me/iliashaposhnikov)

**💼 LinkedIn:** [@iliashaposhnikov](https://linkedin.com/in/iliashaposhnikov)

🇬🇧 **[English Version / На английском](README.md)**
