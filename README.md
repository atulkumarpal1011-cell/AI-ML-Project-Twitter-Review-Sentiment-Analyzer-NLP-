📝 Sentiment Analysis using Multinomial Naive Bayes
https://colab.research.google.com/drive/1QcnPi64NmZd8T66MaDgWe3E6ICawWofN
 
📌 Project Overview
This project is a Natural Language Processing (NLP) application designed to classify text-based reviews into two categories: Positive or Negative. Using a probabilistic approach, the model analyzes the frequency of specific words to determine the overall sentiment of a given statement.

🎯 Key Features
Automated Text Cleaning: Uses English stop-word removal to filter out non-informative data.

Vectorization: Converts raw text into a numerical format using a "Bag of Words" model.

Efficient Classification: Implements the Naive Bayes algorithm, known for its speed and effectiveness in text classification.

Live Predictor: Includes a function to test custom strings in real-time.

🛠️ Technical Workflow (As per main.py)
The project follows these six distinct steps:

Data Loading: Utilizes pandas to manage the dataset (supports both dummy data for testing and .csv files for production).

Preprocessing: Employs CountVectorizer to handle tokenization and lowercase normalization.

Data Splitting: Uses a 80/20 train-test split to ensure the model is evaluated on unseen data.

Model Training: Trains a MultinomialNB classifier on the vectorized word counts.

Evaluation: Generates an Accuracy Score and a Classification Report (Precision, Recall, and F1-Score).

Inference: A predict_sentiment() function provides a user-friendly interface for new inputs.
📈 Evaluation Results
Upon execution, the model outputs the following metrics:

Accuracy: (e.g., 100% on dummy data, varies on full datasets).

Precision/Recall: High scores indicate the model effectively distinguishes between "Masterpiece" (Positive) and "Trash" (Negative).

🧠 Reflection & Critical Thinking
Algorithm Choice: I chose Multinomial Naive Bayes because it treats word counts as discrete features, which is mathematically ideal for text classification compared to standard Logistic Regression.

Limitations: The current model uses CountVectorizer which only counts word occurrences. A future improvement would be using TF-IDF to penalize words that appear frequently across all documents but carry little sentiment (like "movie" or "film").

Impact: This logic can be scaled to analyze thousands of customer reviews or Twitter mentions to provide instant feedback on brand health.

👤 Author
Atul Kumar Pal

Submission Date: March 31, 2026
