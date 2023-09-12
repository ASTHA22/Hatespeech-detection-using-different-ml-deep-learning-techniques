# Hatespeech-detection-using-different-ml-deep-learning-techniques

Social media platforms allow users to express themselves freely, but this can come at a cost. The moderators who are responsible for keeping social media clean are often overworked and underpaid, which can lead to hate speech and other harmful content going unchecked. This can have serious consequences for individuals and communities, including harassment, discrimination, and the spread of harmful ideologies. This project aims to compare and identify the best approach for detecting hate speech on social media. By developing a model that can automatically identify and flag hate speech content, we hope to make social media a safer and more inclusive space for everyone.


Design:
The system design of the projects involves
1. Data retrieval - Collect data from various sources using web scraping or API calls.
2. Data preprocessing - Text is cleaned by converting to lowercase, removing retweet mentions, URLs, and punctuations, and tokenizing and stemming the words
3. EDA – To understand the characteristics, distribution of classes and possible patterns in the dataset.
4. Train-Test Split - Divide the preprocessed dataset into training and testing sets.
5. Model Development - Feature engineering prepares the text data for the model. The neural network architecture is defined, compiled with categorical cross-entropy loss
6. Model Training and Evaluation - Using training data with model checkpoints. The model's performance is evaluated with classification metrics on the test set, allowing for potential improvements.
7. Hyperparameter Tuning - Perform hyperparameter tuning to find the best combination of hyperparameters for the model
   
Implementation:
1. Download the dataset from Google Drive using gdown library
2. Load the dataset into a pandas dataframe
3. Drop unnecessary columns and using nltk, preprocess the data to remove stopwords and punctuations. Perform stemming by using the Snowball Stemmer.
4. Generate the vectorized input for the bag of words models using the Tf-Idf vectorizer and for
the deep learning model using the Keras Tokenizer. Split the vectorized output into train and test data
5. Using Sklearn, import and initialize the bag of words models and fit them to the training data. Using the trained models, predict the output for the test data and display the accuracy and classification matrix for each model.
6. Create the deep learning lstm model by importing the keras library. Create a sequential model with an embedding layer, a bidirectional layer and a fully connected layer. Fit the model on the train data for a certain number of epochs. Predict the test data output and print accuracy along with classification matrix.
7. Generate bar plot for all the accuracies and print out the same in a tabular format.
