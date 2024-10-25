# COVID19-Rumour-Detection

A project to build a classifier for detecting rumours in COVID-19-related tweets. Utilises SVM, MLP, and BERT models for classification, along with analysis of tweet topics, hashtags, sentiment, and user behaviour. Includes code for data preprocessing, model training, and results analysis.

- **Project Overview**: Developed a binary classifier to detect rumours in tweets and performed an in-depth analysis of COVID-19-related tweets.
- **Data Retrieval**: Used Twitter API and Tweepy to retrieve tweet objects and processed over 15,000 tweet sets for rumour detection.
- **Data Preprocessing**: Cleaned text data by removing special characters, hyperlinks, hashtags, and emojis, then concatenated tweet text and replies for model input.
- **Models Implemented**:
  - **SVM (Support Vector Machine)**: Developed an SVM model with TF-IDF transformation and SMOTE for handling data imbalance.
  - **MLP (Multi-layer Perceptron)**: Implemented MLP using Keras, employing a bag-of-words approach, and used oversampling to mitigate dataset imbalance.
  - **BERT (Bidirectional Encoder Representations from Transformers)**: Trained BERT models (both cased and uncased) for state-of-the-art performance in text classification. The uncased BERT achieved the best results with an F1 score of 0.917.
- **Performance Evaluation**: Achieved the highest F1 score on the rumour detection task using BERT, outperforming other models like SVM and MLP.
- **COVID-19 Rumour Analysis**: Applied the trained BERT model to analyse COVID-19 tweets, revealing that 20% of the dataset were classified as rumours.
- **Key Findings**:
  - **Topic Analysis**: Identified key topics in rumours and non-rumours, such as government figures in rumours and factual updates in non-rumours.
  - **Hashtag Analysis**: Found significant overlap in popular hashtags but identified rumour-specific ones like #Trump and #Wuhan.
  - **Sentiment Analysis**: Discovered that rumours tended to spread more negative sentiment than non-rumours.
  - **User Behaviour**: Rumour-creating users had more followers and influence compared to non-rumour users.
- **Tools and Technologies**: Python, TensorFlow/Keras, PyTorch, Twitter API, BERT, SVM, MLP, SMOTE.
