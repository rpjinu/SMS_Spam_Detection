# SMS_Spam_Detection
whole project analysis ,building model and deployment
<img src="https://github.com/rpjinu/SMS_Spam_Detection/blob/main/spam_logo.png" width="600">
#SMS Spam Detection Project
Project Overview\
This project aims to detect spam messages from SMS data using machine learning. The dataset contains labeled messages as either 'spam' or 'ham' (not spam). The project involves data extraction, preprocessing, model training, and deployment using Streamlit.

#Table of Contents:-
1.Dataset\
The dataset used for this project is spam.csv, which contains the following columns:\

   a.label: Indicates whether the message is 'spam' or 'ham'.\
   b.message: The content of the SMS message\
2.Project Structure\
3.Installation\
4.Data Extraction and Preprocessing\
5.Model Training and Evaluation\
6.Saving the Best Model and Vectorizer\
7.Deployment\
8.Streamlit Web App\
#Project Structure:-
├── data\
│   ├── spam.csv\
├── models\
│   ├── best_model.pkl\
│   ├── vectorizer.pkl\
├── app\
│   ├── app.py

#Data Extraction and Preprocessing:-
Load the Dataset:\

The dataset is loaded from spam.csv.\
Text Preprocessing:\

Messages are cleaned and preprocessed, including tasks like lowercasing, removing punctuation, and tokenization.\
NLTK's CountVectorizer is used to convert the text messages into a matrix of token counts.\
Data Splitting:\

The dataset is split into training and testing sets.\
Model Training and Evaluation\
Model Selection:\

Various classification models are trained on the training data.\
Evaluation:\

The models are evaluated based on accuracy, precision, recall, and F1-score.\
Choosing the Best Model:\

The model with the highest accuracy is selected as the best model.\
Saving the Best Model and Vectorizer\
Save the Best Model:\
The best-performing model is saved as best_model.pkl in the models/ directory.\
Save the Vectorizer:\
The CountVectorizer used for text transformation is saved as vectorizer.pkl in the models/ directory.\
Deployment\
Streamlit Setup:\

A Streamlit application is created to deploy the model for real-time predictions.\
Deployment in PyCharm:\

The Streamlit app is run in PyCharm for testing and deployment.\
Streamlit Web App\
#deploy image
<img src="https://github.com/rpjinu/SMS_Spam_Detection/blob/main/Deploy_image.png" width="900">
The web application allows users to input a raw SMS message and predict whether it's spam or ham.\
The app utilizes the saved vectorizer.pkl to convert text into a matrix form and the best_model.pkl for prediction.

