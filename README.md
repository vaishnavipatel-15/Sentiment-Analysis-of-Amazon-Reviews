
# Amazon Reviews Sentiment Analysis

## Overview

This project is the final submission for the Data Science Engineering Tools and Methods course (INFO6105) at Northeastern University. The objective of this project is to perform sentiment analysis on Amazon book reviews to uncover sentiments associated with different book genres.

## Table of Contents

- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Results](#results)
- [Conclusion](#conclusion)
- [Contributors](#contributors)
- [License](#license)

## Introduction

### Background

Amazon, being one of the largest e-commerce platforms globally, accumulates a vast amount of customer reviews for its products, including books. Sentiment analysis plays a crucial role in extracting valuable insights from these reviews, aiding authors, publishers, and retailers in understanding customer opinions and preferences. This project focuses on performing sentiment analysis on an Amazon book reviews dataset to uncover sentiments associated with different book genres.

### Motivation

- **Customer Insights:** By analyzing customer reviews, businesses can uncover both praise and concerns, directly influencing product improvements and customer service practices.
- **Strategic Decision Making:** The insights gained from sentiment analysis are integral for strategic planning, helping to tailor products and marketing efforts to meet customer expectations more effectively.

### Goals

- **Immediate Goals:** Develop an efficient model capable of accurately classifying sentiments as positive, negative, or neutral in Amazon book reviews.
- **Long-Term Objectives:** Leverage these insights to predict future buying behaviors and trends and integrate this model into business analytics tools for ongoing monitoring.

## Project Structure

- `data/`: Contains the dataset used for training and testing.
- `notebooks/`: Jupyter notebooks for exploratory data analysis and model development.
- `src/`: Source code for data preprocessing, model training, and inference.
- `models/`: Pre-trained and trained models.
- `results/`: Output images and performance metrics.
- `report/`: Final report document.
- `ppt/`: Project presentation.
- `README.md`: Project documentation.

## Installation

To set up the project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/amazon-reviews-sentiment-analysis.git
   cd amazon-reviews-sentiment-analysis
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

To run the sentiment analysis model, use the following command:

```bash
python src/detect.py --input data/sample_review.txt --output results/output_sentiment.txt
```

## Dataset

The dataset used for this project includes Amazon book reviews with annotated sentiments. You can download the dataset from [Kaggle](https://www.kaggle.com/datasets) (specific dataset link will be provided in the final report).

## Methodology

### Data Cleaning

- Removing duplicates
- Correcting typographical errors
- Eliminating irrelevant content

### Exploratory Data Analysis (EDA)

- Techniques such as tokenization, lemmatization, and stopwords removal to prepare text data for analysis.

### Feature Engineering

- Utilizing TF-IDF for text vectorization to reflect the importance of words in relation to the dataset.

### Model Selection

- Chose a combination of Logistic Regression, Random Forest, and XGBoost due to their efficacy in text classification tasks.

## Results

- **Sentiment Trends:** Positive sentiments dominate in fiction genres, while non-fiction shows a higher incidence of critical reviews.
- **Model Performance:** XGBoost outperformed other models in accuracy and efficiency.
- **Visualizations:** Displayed through bar charts for sentiment distribution and line graphs showing sentiment trends over time.

## Conclusion

- Successfully implemented various preprocessing and EDA techniques on the dataset.
- Developed and compared the performance of multiple ML models using cross-validation.
- XGBoost became the cornerstone of our sentiment analysis.
- Created a function to pinpoint pros and cons within textual feedback, providing clear insights into customer perceptions.


## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

Feel free to modify this README description to better fit your project specifics and personal details.
