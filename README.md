# Project Title: StyleSense Recommendation Forcasting Pipeline

The project is part of the 3rd student assignment for the Udacity Course "Data Scientist". Topic is to build a pipeline on historic data of a fashion company called StyleSense to predict customer recommendations based on a number of features.

The original features:

* Clothing ID: Integer Categorical variable that refers to the specific piece being reviewed.
* Age: Positive Integer variable of the reviewers age.
* Title: String variable for the title of the review.
* Review Text: String variable for the review body.
* Positive Feedback Count: Positive Integer documenting the number of other customers who found this review positive.
* Division Name: Categorical name of the product high level division.
* Department Name: Categorical name of the product department name.
* Class Name: Categorical name of the product class name.

The features are further processed in a machine learning pipeline, which includes a sentiment analysis of the Title feature, which is quite computation intensive.

The target:
* Recommended IND: Binary variable stating where the customer recommends the product where 1 is recommended, 0 is not recommended.

# Getting Started

The project contains the following project files:
* iPython notebook with the whole pipeline, including data exploration and fine tuning: "StyleSense_Forcasting.ipynb".
* Provided data for the assigment: "reviews.csv".
* A requirements file containing the necessary packages for the virtual environment: "requirements.txt".

# Dependencies

The pipeline needs the following python packages, as also listed in the "requirements.txt" file:
* scikit-learn: For building the pipline.
* pandas: For data processing.
* spacy: For NLP text processing.
* notebook: For iPython notebook functionality.
* spacytextblob: For sentinment analysis of the Title feature.

# Installation

A virtual environment first needs to be installed:
```bash
pip install -r requirements.txt
```

Further for spaCy NLP and sentiment analysis respective data has to be loaded (also part of the notebook):
```bash
python -m spacy download en_core_web_sm
python -m textblob.download_corpora
```

This only has to be done once.

# Important Notes

* Sentiment analysis with "spacytextblob" package doesn't run in parallel.
* Sentiment analysis is computational intensive. To run the project on a laptop in reasonable time, sentiment analysis is restricted to the Title feature.
* For the sentiment analysis the input and output data of the transformer had to be reshaped to work properly.
* For prediction a sklearn LogisticRegression model is used.

# License

[License](LICENSE.txt)
