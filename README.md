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


## Architecture Diagram

Illustrates the data flow, including the integration of recommendation algorithms, audio synthesis, and the user interface components.
Technology Stack
  [![Python](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)](https://www.python.org/)
  [![Snowflake](https://img.shields.io/badge/Snowflake-387BC3?style=for-the-badge&logo=snowflake&logoColor=light)](https://www.snowflake.com/)
  [![Beautiful Soup](https://img.shields.io/badge/Beautiful%20Soup-59666C?style=for-the-badge&logo=python&logoColor=blue)](https://www.crummy.com/software/BeautifulSoup/)
  [![Grobid](https://img.shields.io/badge/Grobid-007396?style=for-the-badge&logo=java&logoColor=white)](https://github.com/kermitt2/grobid)
  [![Apache Airflow](https://img.shields.io/badge/Apache%20Airflow-017CEE?style=for-the-badge&logo=apache-airflow&logoColor=white)](https://airflow.apache.org/)
  [![Google Cloud Platform](https://img.shields.io/badge/Google%20Cloud%20Platform-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white)](https://cloud.google.com/)
  [![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)](https://www.streamlit.io/)
  [![Amazon S3](https://img.shields.io/badge/Amazon%20S3-569A31?style=for-the-badge&logo=amazon-s3&logoColor=white)](https://aws.amazon.com/s3/)


Project File Structure
```
├── Makefile
├── airflow
│   ├── dags                   # Airflow DAGs for ETL and data processing
│   ├── logs                   # Logs for Airflow execution
│   └── plugins                # Airflow plugins
├── backend
│   ├── main.py                # FastAPI backend for user and data operations
│   ├── utils                  # Utility modules for backend operations
├── docker-compose.yaml        # Configuration for container orchestration
├── requirements.txt           # Python dependencies
├── scripts
│   ├── DataPreprocessing      # Scripts for data cleaning and transformation
│   ├── GoodreadsScraper       # Scraper for collecting Goodreads data
└── streamlit
    ├── main.py                # Main application for the Streamlit frontend
    ├── utils                  # Helper scripts for frontend functionality
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
