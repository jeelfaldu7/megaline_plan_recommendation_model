# 📱 Megaline Plan Recommendation Model

## 📊 Project Overview
Megaline, a mobile carrier, has identified that many of its customers still use outdated legacy plans. To enhance user experience and encourage the transition to modern plans, Megaline aims to implement a recommendation system that suggests one of their newer plans - Smart or Ultra, based on each subscriber's monthly usage behavior. This machine learning classification project focuses on analyzing subscriber data to build a model capable of accurately predicting the most appropriate plan for each user. The model is evaluated based on its performance , with a required minimum accuracy of 0.75 on the test set.

## 📌 Table of Contents
  - Project Overview
  - Dataset Description
  - Model Development
  - Results
  - Installation
  - How to Use
  - Lessons Learned
  - Credits

## 📁 Dataset Description
Each record in the dataset represents a subscriber's monthly behavior, with the following features:
  - `calls` — Number of calls made
  - `minutes` — Total call duration (minutes)
  - `messages` — Number of text messages sent
  - `mb_used` — Internet traffic used (MB)
  - `is_ultra` — Target variable (1 if the user is on the Ultra plan, 0 for Smart)

## 🔍 Model Development
The project explored several classification models including:
  - Decision Tree
  - Random Forest
  - Logistic Regression
Hyperparameters were tuned using validation accuracy as the main metric. The model with the best balance of performance and interpretability was selected.

## ✅ Results
The best-performing model is Random Forest Classifier which achieved an accuracy of 0.78 on the test set, exceeding the 0.75 threshold.

## ⚙️ Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/megaline-plan-recommender.git
   cd megaline-plan-recommender
2. Create a virtual environment and install dependencies:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r requirements.txt

## 🚀 How to Use
Run the project script to:
  - Load and preprocess the data
  - Split it into training, validation, and test sets
  - Train several classification models
  - Evaluate their performance

## 📚 Lessons Learned
  - Feature scaling wasn’t needed for every model—especially for tree-based models like decision trees.
  - Class imbalance didn’t have a big impact, but it’s worth looking into metrics like precision and recall for a deeper evaluation.
  - It's important to find the right balance between model accuracy and how easily the model can be explained, especially when the model is used in real-world applications.

## 🤝 Credits
This project was created as part of the TripleTen Data Science program - Introduction to Machine Learning course. Special thanks to:
  - TripleTen instructors and peers for ongoing support and feedback

## 🛡️ License
This project is licensed under the MIT License.
