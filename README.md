# Marketing-Analytics-Business-Case


📊 Customer Review & Engagement Data Analysis with Sentiment Scoring
This project is focused on end-to-end data cleaning, transformation, and sentiment analysis using SQL and Python. The dataset simulates a marketing analytics environment where customer feedback, product interactions, and content engagement data are collected and prepared for deeper insights and dashboarding.

🚀 Project Overview
The goal of this project was to:

Clean and transform raw data stored in SQL Server.

Perform sentiment analysis on customer review text using NLP techniques.

Prepare a clean, analysis-ready dataset for visualization tools like Power BI.

Gain insights into customer behavior, content performance, and product sentiment.

🛠 Tools & Technologies
SQL Server (SSMS) – Data extraction, cleaning, and transformation

Python (Jupyter Notebook) – Sentiment analysis using nltk

Pandas – Data manipulation and preprocessing

NLTK (VADER) – Sentiment scoring of textual reviews

Power BI – (Optional) Dashboarding and data visualization

GitHub – Version control and portfolio sharing

🧹 Data Cleaning & Transformation (SQL)
Performed the following data preparation tasks:

🔸 Customer Journey Table
Identified duplicate rows using ROW_NUMBER() over key columns (CustomerID, ProductID, etc.).

Replaced missing Duration values with the average duration using an UPDATE + AVG() query.

🔸 Engagement Data Table
Fixed inconsistent ContentType entries using REPLACE() and UPPER().

Split ViewsClicksCombined field into separate Views and Clicks columns.

Formatted EngagementDate into readable dd.MM.yyyy format.

Filtered out irrelevant Newsletter entries.

🔸 Customer Reviews Table
Removed extra white spaces in ReviewText using REPLACE() for cleaner NLP input.

💬 Sentiment Analysis (Python + NLTK)
Used the VADER sentiment analyzer from NLTK to extract and classify the sentiment from review text.

Calculated SentimentScore for each review using VADER’s compound score.

Classified reviews into categories like Positive, Negative, Mixed Positive, etc., based on both text sentiment and user rating.

Bucketed sentiment scores into interpretable ranges (e.g., 0.5 to 1.0, -1.0 to -0.5).

Exported the final dataset to CSV for downstream use.

