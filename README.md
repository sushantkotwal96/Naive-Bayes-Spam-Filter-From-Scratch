# Naive-Bayes-Spam-Filter-From-Scratch

## Project Overview
This project demonstrates the creation of a spam filter using the Naive Bayes algorithm, implemented entirely from scratch. The goal is to classify messages as either "spam" or "ham" based on their content. The dataset used for this project is a collection of messages labeled accordingly.

## Data Preprocessing
1. Loading Data:
- The dataset is loaded into a Pandas DataFrame for easy manipulation and analysis. 
- Only the relevant columns (Message and Label) are selected for further processing.

2. Data Cleaning and Preparation:
- Unique words from the messages are extracted and their occurrences are counted.
- Functions are created to calculate word occurrences and unique word counts.

3. Word Occurrence Calculation:
- A function is designed to iterate through each message and count the occurrences of each word. This helps in understanding the distribution of words across the dataset.

4. Unique Word Count:
- Another function is created to identify and count the unique words present in the dataset. This aids in feature engineering for the Naive Bayes algorithm.

5. Count of Unique Words:
- This function creates a DataFrame where each column represents a unique word, and each row corresponds to a message. The values indicate the count of each word in the respective message.

## Model Training and Evaluation

1. Data Splitting:
-The dataset is split into training and testing sets using Stratified K-Folds cross-validation to ensure a balanced distribution of spam and ham messages in both sets.

2. Visualization:
-The most frequent words in the training dataset are plotted to visualize their distribution. This helps in understanding which words are more common in spam or ham messages.

3. Model Implementation:
- The Naive Bayes classifier is implemented from scratch using Maximum Likelihood Estimation to calculate the probabilities of words occurring in spam and ham messages.

4. Performance Evaluation:
- The model is evaluated using a confusion matrix, classification report, and ROC-AUC curves. These metrics provide insights into the model's accuracy, precision, recall, and overall performance.

## Results
- The spam filter achieved high accuracy in classifying messages as "spam" or "ham".
- The project demonstrated the effectiveness of the Naive Bayes algorithm implemented from scratch, providing a solid understanding of its inner workings and practical application.

## Conclusion
This project showcases the implementation of a Naive Bayes spam filter without relying on external libraries, emphasizing the understanding of the underlying algorithm and its practical application in classifying text data.

