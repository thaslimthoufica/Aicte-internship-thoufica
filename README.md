
# **Spam Email Classifier with Streamlit GUI**  

This repository contains a **machine learning-based email spam classifier** that uses a **Naive Bayes MultinomialNB model** to classify emails as "spam" or "not spam." The application includes:  

- A **Streamlit-based graphical user interface (GUI)** for easy interaction.  
- A trained model and vectorizer saved as pickle files (`spam.pkl`, `vec.pkl`).  
- A Jupyter Notebook used for model training.  

---

## **Table of Contents**  
- [Overview](#overview)  
- [Features](#features)  
- [Dataset](#dataset)  
- [Requirements](#requirements)   
- [Usage](#usage)  
- [Future Improvements](#future-improvements)  
- [Contributing](#contributing)  
- [License](#license)  

---

## **Overview**  
This project uses the **spam.csv** dataset to train a spam email classification model. The trained model is deployed via a **Streamlit app**, enabling users to input email text and get instant classification results.  

---

## **Features**  
1. **Spam Detection:** Classifies emails as spam or not spam.  
2. **Interactive GUI:** User-friendly interface built with Streamlit.  
3. **Machine Learning Model:** Naive Bayes (MultinomialNB) trained on vectorized text data.  
4. **Pre-trained Model:** Saves time and resources by reusing the trained model (`spam.pkl`).  

---

## **Dataset**  
The model is trained on the **spam.csv** dataset.  
- **Columns Used:**  
  - `Category`: Labels (Spam/Ham).  
  - `message`: Email content.  

The dataset is preprocessed, and the labels are encoded (`ham` = 0, `spam` = 1).  

---

## **Requirements**  
- Python 3.7+  
- Libraries:  
  - streamlit  
  - scikit-learn  
  - pandas  
  - numpy  

---


**Run the Streamlit App**  
   ```bash  
   streamlit run spamdetector.py  
   ```  

---

## **Usage**  
1. Enter an email in the input box.  
2. Click the **"Classify"** button.  
3. The app will display whether the email is spam or not spam.  

---

## **File Structure**  
```plaintext  
├── spam.csv           # Dataset used for training  
├── spam.pkl           # Trained Naive Bayes model  
├── vec.pkl            # Trained CountVectorizer  
├── spamdetector.py    # Streamlit app for GUI  
├── train_model.ipynb  # Jupyter Notebook for training  
├── requirements.txt   # Dependencies for the project  
```  

---

## **Future Improvements**  
- Display confidence scores for classifications.  
- Include support for additional datasets.  
- Implement advanced NLP techniques like TF-IDF or transformers.  
- Deploy the app on Streamlit Cloud or other hosting services.  

---

## **Contributing**  
Contributions are welcome! Feel free to fork the repository and submit pull requests.  

---

## **License**  
This project is licensed under the MIT License.  
