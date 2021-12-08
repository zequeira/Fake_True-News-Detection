# Fake / True News Detection

In this notebook I conduct an exploratory data analysis on the text data.
Then, I train three models for fake news detection.
Data is taken from [this kaggle](https://www.kaggle.com/clmentbisaillon/fake-and-real-news-dataset) competition.

The models are:

* The pretrained **DistilBERT** and **ALBERT Base v1** models using implementations from the `Hugging Face` framework. I used transfer learning to retrain these two models for fake news detection.  
* **XGBoost Classifier** from the `XGBoost` library with `TF-IDF` features.

## Results

| Model             | Dataset    | Accuracy   | F1-Score | 
|-------------------|------------|------------|----------|
| **DistilBERT**    | Validation | 0.9996     |0.9996    |
|                   | Test       | 0.9998     |0.9998    |
| **ALBERT Base v1**| Validation | 0.999      |0.999     |
|                   | Test       | 0.9998     |0.9998    |
| **XGBClassifier** | Validation | 0.975      |0.975     |
|                   | Test       | 0.973      |0.973     |