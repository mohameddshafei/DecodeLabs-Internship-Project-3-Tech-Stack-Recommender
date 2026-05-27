# DecodeLabs Internship Project 3: Tech Stack Recommender

## Project Overview

This project is a simple AI-based recommendation system developed for DecodeLabs Internship Project 3.

The system recommends suitable technology career paths based on the user's skills or interests. The user enters three skills, and the program compares those inputs with a dataset of technology-related roles using TF-IDF vectorization and cosine similarity.

The goal of this project is to demonstrate basic recommendation logic, text matching, and similarity-based ranking.

## Project Objective

The main objective is to build a recommendation system that can:

- Take user skills or interests as input
- Compare the input with available technology roles
- Calculate similarity scores
- Recommend the top 3 most suitable career paths

## Dataset

The dataset used in this project is `raw_skills.csv`.

It contains 54 technology-related roles with the following columns:

- `role`: The name of the career path or job role
- `skills`: Skills commonly required for the role
- `tools_platforms`: Tools and platforms used in the role
- `description`: A short explanation of the role

## Technologies Used

- Python
- Pandas
- Scikit-learn
- TF-IDF Vectorizer
- Cosine Similarity
- Jupyter Notebook

## How the System Works

1. The dataset is loaded using Pandas.
2. The important text columns are combined into one text column.
3. The user enters three skills or interests.
4. TF-IDF converts the text data into numerical vectors.
5. Cosine similarity compares the user's input with each role.
6. The roles are ranked based on similarity score.
7. The top 3 matching career paths are displayed.

## Example

If the user enters:

```text
Python
Machine Learning
Data Analysis
```

The system may recommend roles such as:

```text
Data Scientist
Machine Learning Engineer
AI Engineer
```

The final recommendations depend on the similarity between the user's input and the role information in the dataset.

## Files in This Repository

```text
DecodeLabs-Internship-Project-3-Tech-Stack-Recommender/
│
├── AI_Tech_Stack_Recommender_p3.ipynb
├── raw_skills.csv
└── README.md
```

## Key Concepts Applied

- Recommendation Systems
- Content-Based Filtering
- Text Preprocessing
- TF-IDF Vectorization
- Cosine Similarity
- Ranking Based on Similarity Scores

## Conclusion

This project successfully builds a simple content-based recommendation system for technology career paths. It shows how user interests can be matched with job roles using text similarity techniques.

Through this project, I learned how recommendation systems can work using basic AI logic without needing complex machine learning models. The system is simple, beginner-friendly, and demonstrates the core idea behind personalized recommendations.
