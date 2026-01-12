# phishing-url-detection-ml
Phishing URL Detection project using Python and ML. Features are extracted from URLs to classify them as phishing or legitimate. Models include Logistic Regression and Random Forest, with evaluation via confusion matrix, precision, recall, and F1-score. Beginner-friendly ML workflow.

This project is a **phishing URL detection system** built using **Python** and **machine learning**. It demonstrates how to clean, preprocess, and extract features from URLs to classify them as **phishing (malicious)** or **legitimate**.

---

## Dataset

- The dataset used is from Kaggle: `Phishing Site URLs`  
- It contains a large collection of URLs labeled as `good` (legitimate) or `bad` (phishing) .  
- The dataset includes potential duplicates and inconsistent formatting, which are handled during preprocessing.

---

## Project Workflow

1. **Data Cleaning**
   - Remove duplicates
   - Strip whitespace and lowercase URLs
   - Handle missing or inconsistent labels

2. **Feature Engineering**
   - Extract URL-based features:
     - URL length
     - Number of dots and hyphens
     - Presence of `@` symbol
     - Use of HTTPS
     - Digit count
     - IP address presence
     
3. **Train-Test Split**
   - Split dataset into training and testing sets (80/20)  
   - Stratified split ensures class balance

4. **Machine Learning Models**
   - **Logistic Regression** (baseline)
   - **Random Forest Classifier** (final model)  
   - Model evaluation using:
     - Confusion Matrix
     - Accuracy
     - Precision, Recall, F1-score

5. **Model Evaluation**
   - Compare models to identify the best performing one  
   - Random Forest achieves better phishing detection due to capturing non-linear patterns

---

## Results

- **Random Forest Classifier** shows higher accuracy and recall for phishing URLs compared to Logistic Regression.  
- Confusion matrix, classification report, and evaluation metrics are included in the notebook.

---

## Notebook
The complete implementation is available on Kaggle:
https://www.kaggle.com/code/karnikakumari/phishing-urls-detection-ml-model

---
## Future Improvements

- Hyperparameter tuning for better performance  
- Additional URL-based features (path length, query parameters, etc.)  
- Deep learning approaches (e.g., LSTM for sequential URL patterns)  

---

## Technologies Used

- Python 3.x  
- Pandas, NumPy for data handling  
- Scikit-learn for machine learning  
- Jupyter Notebook / Kaggle Notebook  

---

**License:** MIT
