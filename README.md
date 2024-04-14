# **Disaster Tweet prediction, NLP**
## **Data Exploration**
### **Load the Data:**
* Import the dataset into your programming environment (e.g., Python with libraries like Pandas, NumPy) or any other tools that you prefer.
### **Inspect the Data:**
* Get a general overview of the dataset by examining its structure, size, and data types. 
### **Explore the Structure:**
* Understand the structure of the dataset by examining the number of rows and columns, data types of each column, and any missing values.
## **Text Preprocessing**
* This section cleans and preprocesses the text data from the "text" column in the Data Frame "df".
* It performs various text preprocessing tasks, such as converting text to lowercase, removing URLs, special characters, stopwords, and tokenizing the text.
* The code utilizes NLTK's modules like word_tokenize, stopwords, and Stemming for this purpose.
* The preprocessed text is stored in a new column named "cleaned_text" in the DataFrame "df".
## **Feature Extraction**
* This section converts the cleaned text data into numerical feature vectors using the Term Frequency-Inverse Document Frequency (TF-IDF) vectorization.
* It uses the Tfidf Vectorizer from Scikit-learn to perform TF-IDF transformation on the "cleaned_text" column in the DataFrame "df".
* The result is stored in the variable "X," which represents the feature vectors.
## **Data splitting**
* This section splits the feature vectors "X" and target labels "y" into training and testing sets using the train_test_split function from Scikit-learn.
* It randomly divides the data, with 80% for training and 20% for testing.
* The training set is stored in "X_train" and "y_train", while the testing set is stored in "X_test" and "y_test".
## **Model Selection**
* Select the model with the best performance based on the evaluation metrics. Consider its accuracy, generalizability, and ability to handle unseen data.
