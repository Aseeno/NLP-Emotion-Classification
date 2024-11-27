1. Loading and Preprocessing
Explanation:
Text Cleaning: The clean_text function removes non-alphanumeric characters, extra spaces, and converts text to lowercase.
Tokenization and Stopword Removal: After cleaning, the text is split into words (tokens). Then, stopwords (common words like "the", "is", etc.) are removed using the NLTK stopword list.

2. Feature Extraction
Explanation:
TF-IDF: TfidfVectorizer transforms the text data into a matrix of term frequencies, weighing words by their inverse document frequency. This helps highlight important words and reduces the impact of common words that don’t provide meaningful distinctions.
Max Features: We limit the number of features to 5000 to avoid overfitting and excessive computation time.

3. Model Development
Explanation:
Naive Bayes: A probabilistic model that is particularly effective for text classification tasks, especially when features (words) are independent.
Support Vector Machine (SVM): A powerful model for classification that creates a hyperplane to separate classes, suitable for high-dimensional text data.

4. Model Comparison
Explanation:
Accuracy: Measures the percentage of correct predictions.
F1-Score: Provides a balance between precision and recall, especially useful when dealing with imbalanced datasets.
Classification Report: Provides detailed performance metrics for each class.

