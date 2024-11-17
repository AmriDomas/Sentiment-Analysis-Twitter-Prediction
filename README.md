# Sentiment-Analysis-Twitter-Prediction
Muh Amri Sidiq
 -

Sentiment analysis is the process of analyzing text to determine the attitudes, emotions, or opinions contained within it. Typically, this analysis is used to identify whether a text has a positive, negative, or neutral sentiment, although some applications can also detect more specific emotions, such as angry, happy, or sad.

Data Exploration
 -
Data split into training and test from dataset

Data Dictionary
 - number : number of data row
 - theme : topic of sentiment
 - sentiment: target of us (negative, positive, neutral and irrelevant)
 - text : review of text

Exploratory data Analys
 -
![count theme](https://github.com/user-attachments/assets/fa687ccd-97c7-43e9-b714-003046a7680c)

biggest contribution theme maddenNFL and lowest contribution is AssasinsCreed

![Count Sentiment](https://github.com/user-attachments/assets/ada74cb9-e077-41e4-a237-5b05b192d571)

from bar above negative is largest and Irrelevant is lowest sentiment

Labels for Sentiment
 - 
 - Negative = 0
 - Positive = 1
 - Neutral  = 2
 - Irrelevant = 3

Stop Word Removal
 - 
clean text URL, number, tag HTML, special character and sign ask, clean space over

Tokenize
 -

Tokenize is the process of breaking the text into small units called tokens. Tokens can be words, phrases, characters, or even other elements depending on the purpose of the analysis. This process is the first step in natural language processing (NLP) to prepare the text for further analysis or processing.

Train-Test Split
 - 
separate for train and test, this data for model LSTM

Modeling
 - 

 - Naive Bayes
   
   Naive Bayes is one of the most popular algorithms for sentiment analysis, mainly due to its simplicity and computational efficiency. It is based on Bayes' Theorem with the assumption that all features are conditionally independent (which is often not strictly true, but sufficient for many practical applications). Text for Naive bayes must be string

   ![COnfusionmatrix NB Basic](https://github.com/user-attachments/assets/006fa402-1b98-49a0-9bd1-cd0db20de3a1)

   Confusion matric with basic model Naive Bayes

   ![Precision, Recall, F1 NB Basic](https://github.com/user-attachments/assets/a1a548b3-2e2f-41d9-b462-3a3c17629489)

   Precision, Recall, and F1-Score for Naive Bayes Model

- Super Vector Machine

  Support Vector Machine (SVM) is a machine learning algorithm often used for sentiment analysis due to its robust performance, especially on high-dimensional datasets such as text. SVM works by finding the best hyperplane that separates the classes in the feature space. Super vestor machine only use string, so we use data from above for naive bayes too.

  ![COnfusionmatrix SVC Basic](https://github.com/user-attachments/assets/1e98264e-6a1b-47ec-8101-ee761a4aa3d4)

  Confusion matric with basic model

  ![Precision, Recall, F1 SVC Basic](https://github.com/user-attachments/assets/09449e57-57b6-4def-a29b-b2a427b2d38e)

  Precision, Recall, and F1-Score for SVM Model

  - LSTM

    LSTM (Long Short-Term Memory) is a type of recurrent neural network (RNN) architecture that is very popular for sentiment analysis due to its ability to capture context from sequences of data, such as text. LSTM is designed to overcome the vanishing gradient problem often experienced by standard RNNs, making it better at capturing long-term relationships in text.

    ![LSTM basic Training vs loss](https://github.com/user-attachments/assets/85392d56-09e0-4d56-9a70-6217b55c49a0)

    Training and Validation loss, Training and Validation Accuracy

    ![COnfusionmatrix LSTM Basic](https://github.com/user-attachments/assets/7a9f3e2a-13a1-4886-8045-7f6e5e48e4b6)

    Precision, Recall, and F1-Score for LSTM Model

Hyperparamater Tuning
 - 

 - Naive Bayes

   ![COnfusionmatrix NB tuning](https://github.com/user-attachments/assets/5a06807c-a63a-4eb1-a8a4-a5c517be5c6c)

   Confusion matric with tuning model Naive Bayes

   ![Precision, Recall, F1 NB tuning](https://github.com/user-attachments/assets/ba361212-7f79-4e61-8dcc-0be1c38c0580)

   Precision, Recall, and F1-Score for Naive Bayes Model tuning

- Super Vector Machine

  ![COnfusionmatrix SVM tuning](https://github.com/user-attachments/assets/276e1d0f-c31b-4b4c-bdfe-69529d73c923)

  Confusion matric with tuning model SVM

  ![Precision, Recall, F1 SVC tuning](https://github.com/user-attachments/assets/e5751058-bccc-4249-b805-f554fc38afc8)

  Precision, Recall, and F1-Score for Naive Bayes Model tuning

- LSTM

  ![COnfusionmatrix LSTM tuning](https://github.com/user-attachments/assets/bec195f8-d9ae-4904-994b-f0f3f8b1b06c)

  Confusion matric with tuning model LSTM

Conclusion
 - 

 with high metric accuracy then we choose to use the LSTM model tuning

Refreence
 - 

  - https://github.com/anmolrk/Social-Media-Sentiment-Analysis/tree/main/data
  - https://d2l.ai/
  - https://www.analyticsvidhya.com/
  - https://xbe.at/
  - https://www.tensorflow.org/guide/keras







  







