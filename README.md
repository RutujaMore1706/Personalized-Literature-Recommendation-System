# Personalized-Literature-Recommendation-System

## Overview
  This project is an innovative digital library platform designed to revolutionize the way users connect with books, stories, and knowledge. With a focus on personalization, it provides tailored book recommendations, immersive audio trailers, and an intuitive interface to enhance user engagement. Our mission is to deliver a unique digital library experience that aligns with individual preferences, making reading discovery more satisfying and enjoyable.

## Project Goals
The platform addresses limitations in traditional digital libraries, such as limited personalization and static content presentation, by leveraging advanced technologies and data-driven approaches. Key features include:

1. **Personalized Book Recommendations**: AI-based suggestions based on users' reading history, interests, and preferences.
2. **Audio Trailers for Books**: AI-driven text-to-speech previews to give users a sense of a book's content, helping them make informed choices.
3. **User-Centric Experience**: A dynamic, interactive interface to improve accessibility, engagement, and satisfaction.

## Features
**1. User Registration and Profile Setup**
    1. New users can sign up and log in to create their profiles.
    2. A chatbot greets new users, asking about book preferences, themes, and reading pace to customize recommendations.

**2. Book Recommendation System**
   1. Users receive initial book recommendations based on their profile.
   2. A "Refresh Recommendations" feature provides updated suggestions tailored to reading history and book ratings.

**3. Book Search and Categorization**
  1. Users can search for books by title and add them to custom lists: "Started Reading," "To Be Read," or "Read."
  2. The dashboard displays categorized books and allows users to rate them.

**4. User Dashboard**
  1. Provides an overview of the user’s reading progress, book lists, and ratings.
  2. Allows users to update ratings or categories for any book.

## Application Links
[![Application Link](https://img.shields.io/badge/Application-green?style=for-the-badge)](http://34.75.0.13:8500/)

[![Codelabs](https://img.shields.io/badge/Codelabs-blue?style=for-the-badge)](https://codelabs-preview.appspot.com/?file_id=1jFy6Rx0jzpvzu8b_3Qoau-6H9RGZU_eqZh1-KDYAFwI#0)

[![Video](https://img.shields.io/badge/Video-CC6699?style=for-the-badge)](https://youtu.be/mWA-ZNdFogo)

## Architecture Diagram
![image](https://github.com/BigDataIA-Spring2024-Sec1-Team4/FinalProject/assets/114356265/a50711ae-f3d1-486a-9812-526c7925966a)

## Technology Stack
  [![Python](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)](https://www.python.org/)
  [![Snowflake](https://img.shields.io/badge/Snowflake-387BC3?style=for-the-badge&logo=snowflake&logoColor=light)](https://www.snowflake.com/)
  [![Beautiful Soup](https://img.shields.io/badge/Beautiful%20Soup-59666C?style=for-the-badge&logo=python&logoColor=blue)](https://www.crummy.com/software/BeautifulSoup/)
  [![Grobid](https://img.shields.io/badge/Grobid-007396?style=for-the-badge&logo=java&logoColor=white)](https://github.com/kermitt2/grobid)
  [![Apache Airflow](https://img.shields.io/badge/Apache%20Airflow-017CEE?style=for-the-badge&logo=apache-airflow&logoColor=white)](https://airflow.apache.org/)
  [![Google Cloud Platform](https://img.shields.io/badge/Google%20Cloud%20Platform-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white)](https://cloud.google.com/)
  [![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)](https://www.streamlit.io/)
  [![Amazon S3](https://img.shields.io/badge/Amazon%20S3-569A31?style=for-the-badge&logo=amazon-s3&logoColor=white)](https://aws.amazon.com/s3/)

## Project Structure:

```
├── Makefile
├── airflow
│   ├── config
│   ├── dags
│   │   ├── __pycache__
│   │   │   └── run.cpython-312.pyc
│   │   ├── run.py
│   │   └── scripts
│   │       ├── audio_linkgeneration.py
│   │       ├── audio_processing.py
│   │       ├── getSeattleLibrary.py
│   │       └── inventory_preprocessing.py
│   ├── logs
│   │   ├── dag_processor_manager
│   │   │   └── dag_processor_manager.log
│   │   └── scheduler
│   │       ├── 2024-04-25
│   │       │   └── run.py.log
│   │       └── latest -> 2024-04-25
│   └── plugins
├── backend
│   ├── Dockerfile
│   ├── __init__.py
│   ├── __pycache__
│   │   ├── get_book_details.cpython-39.pyc
│   │   ├── main.cpython-310.pyc
│   │   ├── main.cpython-311.pyc
│   │   └── main.cpython-39.pyc
│   ├── main.py
│   ├── requirements.txt
│   └── utils
│       ├── __pycache__
│       │   ├── login_backend.cpython-310.pyc
│       │   ├── login_backend.cpython-311.pyc
│       │   ├── login_backend.cpython-39.pyc
│       │   ├── snowflake_connector.cpython-310.pyc
│       │   ├── snowflake_connector.cpython-311.pyc
│       │   └── snowflake_connector.cpython-39.pyc
│       ├── login_backend.py
│       └── snowflake_connector.py
├── docker-compose.yaml
├── requirements.txt
├── scripts
│   ├── DataPreprocessing
│   │   ├── Goodreads_Preprocessing.py
│   │   ├── Goodreads_Preprocessing_2.py
│   │   └── getBookInventory.py
│   ├── GoodreadsScraper
│   │   ├── CSV
│   │   │   ├── goodreads_merged.csv
│   │   │   ├── out_books.csv
│   │   │   ├── out_decade_books.csv
│   │   │   ├── out_mystrey_books.csv
│   │   │   ├── out_once_books.csv
│   │   │   └── out_young_books.csv
│   │   ├── GoodreadsScraper
│   │   │   ├── __init__.py
│   │   │   ├── __pycache__
│   │   │   │   ├── __init__.cpython-310.pyc
│   │   │   │   ├── items.cpython-310.pyc
│   │   │   │   ├── pipelines.cpython-310.pyc
│   │   │   │   └── settings.cpython-310.pyc
│   │   │   ├── custom_filters.py
│   │   │   ├── items.py
│   │   │   ├── middlewares.py
│   │   │   ├── pipelines.py
│   │   │   ├── settings.py
│   │   │   └── spiders
│   │   │       ├── __init__.py
│   │   │       ├── __pycache__
│   │   │       │   ├── __init__.cpython-310.pyc
│   │   │       │   ├── author_spider.cpython-310.pyc
│   │   │       │   ├── book_spider.cpython-310.pyc
│   │   │       │   ├── list_spider.cpython-310.pyc
│   │   │       │   └── mybooks_spider.cpython-310.pyc
│   │   │       ├── author_spider.py
│   │   │       ├── book_spider.py
│   │   │       └── list_spider.py
│   │   ├── book_goodreads_book.jl
│   │   ├── book_goodreads_decade_book.jl
│   │   ├── book_goodreads_mystrey_book.jl
│   │   ├── book_goodreads_once_book.jl
│   │   ├── book_goodreads_young_book.jl
│   │   ├── chromedriver
│   │   ├── cleanup.py
│   │   ├── crawl.py
│   │   ├── merge.py
│   │   ├── scrapy.cfg
│   │   └── scrapy.log
│   ├── book_attributes.csv
│   ├── book_attributes_null.csv
│   ├── csv_snowflake.py
│   ├── getBookProfile.py
│   └── openai_newkey.py
└── streamlit
    ├── Dockerfile
    ├── __pycache__
    │   ├── book_recommendation.cpython-310.pyc
    │   ├── book_recommendation.cpython-311.pyc
    │   ├── book_recommendation.cpython-39.pyc
    │   ├── search_book.cpython-310.pyc
    │   ├── search_book.cpython-311.pyc
    │   ├── search_book.cpython-39.pyc
    │   ├── search_book_new.cpython-310.pyc
    │   ├── search_book_new.cpython-311.pyc
    │   ├── search_book_new.cpython-39.pyc
    │   ├── user_dashboard.cpython-310.pyc
    │   ├── user_dashboard.cpython-311.pyc
    │   ├── user_dashboard.cpython-39.pyc
    │   ├── user_survey.cpython-310.pyc
    │   ├── user_survey.cpython-311.pyc
    │   └── user_survey.cpython-39.pyc
    ├── book_recommendation.py
    ├── login.py
    ├── main.py
    ├── pages
    ├── requirements.txt
    ├── search_book.py
    ├── search_book_new.py
    ├── streamlit_app.py
    ├── user_dashboard.py
    ├── user_survey.py
    └── utils
        ├── __pycache__
        │   ├── book_details.cpython-310.pyc
        │   ├── book_details.cpython-311.pyc
        │   └── book_details.cpython-39.pyc
        ├── book_details.py
        └── get_user_profile.py
```


## Using the Application
1. **User Registration and Login**
  Sign Up: New users can register, set preferences, and get initial recommendations.
  Log In: Returning users can access their personalized dashboard and recommendations.
2. **Book Search and Recommendations**
  Search: Users can search for books and add them to various reading lists.
  Recommendations: Navigate to the “Book Recommendations” tab for suggestions, and refresh them based on your activity.
3. **User Dashboard**
  Access categorized reading lists, add or update ratings, and explore suggested books.

## Installation and Setup
1. **Clone Repository**:
    ```
    git clone <repository-url>
    cd digital-library-platform
    ```
2. **Install Dependencies**:

    ```pip install -r requirements.txt```

3. **Run Services**:
    1. Start Airflow for ETL processes.
    2. Launch Streamlit for the user interface.
    3. Deploy FastAPI for backend operations.

## Future Enhancements
  1. Advanced Filtering Options: Introduce filters based on genres, themes, and ratings.
  2. Community Features: Enable user reviews, comments, and book discussions.
  3. Mobile App: Expand accessibility through mobile platforms for enhanced engagement.

## References:
- ChatGPT: https://chat.openai.com/
- OpenAI CLIP: https://towardsdatascience.com/quick-fire-guide-to-multi-modal-ml-with-openais-clip-2dad7e398ac0 
- Fast API: https://fastapi.tiangolo.com/
- Airflow: https://airflow.apache.org/docs/apache-airflow/stable/core-concepts/dags.html
- Pinecone: https://www.pinecone.io/learn/vector-database/
- Docker: https://www.docker.com/#
- JWT Tokens: https://jwt.io/introduction
- gTTs: https://gtts.readthedocs.io/en/latest/

