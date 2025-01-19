# Quora Duplicate Question Pair Detection
This project focuses on detecting duplicate question pairs on Quora using various text classification techniques. The goal is to identify whether two questions are semantically similar, which can enhance user experience by minimizing redundancy.
<img width="784" alt="quoratext" src="https://github.com/user-attachments/assets/51d8beea-f0bc-4ab9-bb61-685c5adfef1f" />

## Usage
**Data Preparation:** The dataset is unzipped and loaded into a DataFrame.  

**Text Classification:** The training is done in the notebook quora-similar-ques-text-classification in which the all the necessary steps are taken you can run this notebook and save the trained model to be used while prediction.  

**Deployment:**  The notebook quora-dup-ques-deploy contains the code for deploying the same to the grado interface in which you can input two questionS and check whether they are duplicate or not.  


## Data
The dataset used in this project is the Quora Question Pairs dataset, which can be [found here](https://www.kaggle.com/c/quora-question-pairs/data). The dataset contains pairs of questions along with a label indicating whether they are duplicates (1) or not (0).  

## Data Structure
- train.csv: Contains training data with question pairs and labels.
- test.csv: Contains test data for evaluation.
  
## Modeling Techniques
This project employs various techniques for text classification, including:

**Text Preprocessing:**  
- Lowercasing, removing special characters, and handling contractions.
- Lemmatization using spaCy.
  
**Feature Extraction:**  
- Bag of Words (BoW) and TF-IDF vectorization.
- Word embeddings using Word2Vec.

**Machine Learning Models:** 
- Random Forest Classifier.
- XGBoost Classifier.
  
 **Evaluation Metrics:**
Accuracy, confusion matrix, and other relevant metrics.

**Results**  

The Random Forest model achieved an accuracy of 78.6%, while the XGBoost model achieved an accuracy of 78.37% on the test dataset. The confusion matrices for both models are provided in the results section of the notebook.


## Contributing 
Contributions are welcome! If you have suggestions for improvements or want to add new features, please fork the repository and submit a pull request.
