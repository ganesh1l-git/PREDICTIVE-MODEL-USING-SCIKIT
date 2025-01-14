# PREDICTIVE-MODEL-USING-SCIKIT

name:killari Ganesh
company:CODTECH IT SOLUTIONS
ID:CT08FAH
DOMAIN:PYTHON 
DURATION:DECEMBER TO JANUARY

**Description of the Spam Email Detection Model:**

This project involves building a predictive model to detect spam emails using scikit-learn, a popular machine learning library in Python. The objective of the model is to classify text messages or emails into two categories:

Key Steps in the Project:
1. Data Collection:
The project uses a public SMS Spam Collection dataset, which contains a set of text messages labeled as "spam" or "ham" (non-spam).
The dataset consists of two columns:
label: The label indicating whether the message is "spam" or "ham".
message: The text of the message itself.
This dataset can be downloaded from the UCI Machine Learning Repository.

2. Data Preprocessing:
The label column, which contains the values "spam" or "ham", is converted into binary values (0 for ham and 1 for spam). This conversion helps the machine learning model in processing the labels as numerical values.
The message column, which contains the text of the messages, is transformed into a bag-of-words representation using CountVectorizer. This process converts the text into numerical vectors that represent the frequency of words in each message. The stop_words='english' parameter ensures that common words (like "the", "is", "in") are ignored, as they don't carry significant meaning for spam detection.

4. Model Training:
The dataset is divided into training and testing sets using an 80-20 split, with 80% of the data used for training the model and 20% used for testing its performance.
We use a Multinomial Naive Bayes classifier, which is particularly effective for text classification tasks involving word counts. Naive Bayes works well in situations where the features (in this case, the words in the message) are independent of each other, making it a good fit for spam detection.

5. Model Evaluation:
After training the model, we evaluate its performance on the test set by calculating the accuracy of the predictions, i.e., the percentage of correct classifications.
In addition to accuracy, we compute a confusion matrix to show how many spam and ham messages were correctly and incorrectly classified. The confusion matrix helps us understand the model's false positives (ham messages labeled as spam) and false negatives (spam messages labeled as ham).
A classification report is generated, providing additional performance metrics like precision, recall, and F1-score. These metrics offer more detailed insights into the model's performance, especially in imbalanced datasets where one class (like spam) might be underrepresented.

7. Making Predictions:
After evaluating the model, it can be used to predict whether a new, unseen message is spam or ham. In this project, we demonstrate predictions with two example messages:
"Free money now!" (likely spam)
"Hey, how are you doing today?" (likely ham)
The trained model uses the same vectorization process to transform the new messages into numerical features and then predicts their labels (spam or ham).

output:

![Screenshot 2025-01-14 180032](https://github.com/user-attachments/assets/9c4959e8-f7b3-4108-a3a6-b05fa30c9720)
![Screenshot 2025-01-14 180043](https://github.com/user-attachments/assets/4054f15f-28e1-434c-a3db-56c63813ae05)

