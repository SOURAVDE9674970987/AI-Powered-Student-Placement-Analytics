# **Student Placement Prediction Using Machine Learning**

## **Project Overview**

**Student Placement Prediction Using Machine Learning** is a machine learning project that predicts whether a student is likely to be placed based on academic performance, technical skills, internships, projects, certifications, communication skills, and other placement-related factors.

The project also generates a **placement probability** and provides personalized recommendations to help students improve their placement prospects.

---

## **Objectives**

* Predict whether a student will be placed or not.  
* Analyze factors that influence student placement.  
* Compare multiple machine learning algorithms.  
* Calculate the probability of placement.  
* Categorize students into High, Medium, and Low placement probability.  
* Provide personalized recommendations for skill improvement.

---

## **Dataset**

The project uses:

student\_placement\_train.csv

The dataset contains **8,000 student records** with **28 original columns**.

### **Target Variable**

| Value | Meaning |
| ----- | ----- |
| `0` | Not Placed |
| `1` | Placed |

The dataset contains approximately **20.38% placed students** and **79.62% non-placed students**.

---

## **Technologies Used**

* Python  
* Pandas  
* NumPy  
* Matplotlib  
* Seaborn  
* Scikit-learn  
* Jupyter Notebook

---

## **Project Workflow**

Dataset  
   ↓  
Data Loading  
   ↓  
Data Cleaning & Preprocessing  
   ↓  
Exploratory Data Analysis  
   ↓  
Feature Engineering  
   ↓  
Feature Selection  
   ↓  
Train-Test Split  
   ↓  
Feature Scaling & Encoding  
   ↓  
Model Training  
   ↓  
Model Evaluation  
   ↓  
Placement Probability Prediction  
   ↓  
Personalized Recommendations

---

## **Feature Engineering**

The following features are created during preprocessing:

### **Total Experience**

total\_experience \= internship\_months \+ training\_hours / 10

### **Achievement Score**

achievement\_score \=  
certifications\_count  
\+ hackathons\_won  
\+ major\_projects  
\+ github\_projects

### **Overall Skill Score**

overall\_skill\_score \=  
(coding\_score  
\+ aptitude\_score  
\+ communication\_score  
\+ technical\_score  
\+ soft\_skills\_score) / 5

---

## **Machine Learning Models**

Three classification algorithms are used:

### **1\. Logistic Regression**

Used as a baseline classification model for predicting placement.

### **2\. Decision Tree**

A tree-based classification algorithm used to identify relationships between student characteristics and placement outcomes.

### **3\. Random Forest**

An ensemble learning algorithm consisting of multiple decision trees. It is also used to calculate placement probabilities.

---

## **Model Evaluation**

The models are evaluated using:

* Accuracy  
* Precision  
* Recall  
* F1-Score

Because the dataset is highly imbalanced, accuracy alone should **not** be considered sufficient for evaluating placement prediction performance.

The placed class has relatively low recall in the current model results, indicating that the model does not identify placed students effectively.

---

## **Placement Probability**

The Random Forest model is used to calculate the probability of a student being placed.

Placement probability is categorized as:

| Probability | Category |
| ----- | ----- |
| ≥ 75% | High |
| 50% – \<75% | Medium |
| \<50% | Low |

---

## **Personalized Recommendations**

The system can provide recommendations based on a student's profile.

Examples include:

* Improve coding skills if the coding score is low.  
* Improve aptitude preparation.  
* Improve communication skills.  
* Improve technical knowledge.  
* Work on additional projects.  
* Gain internship experience.  
* Obtain relevant certifications.  
* Improve mock interview performance.

---

## **Project Structure**

Student-Placement-Prediction/  
│  
├── student\_placement.ipynb  
├── student\_placement\_train.csv  
├── requirements.txt  
├── README.md  
└── report/  
    └── Project\_Report.pdf

---

## **🚀 Installation**

### **1\. Clone or download the project**

git clone \<repository-url\>  
cd Student-Placement-Prediction

### **2\. Install dependencies**

pip install \-r requirements.txt

### **3\. Start Jupyter Notebook**

jupyter notebook

### **4\. Open the notebook**

Open:

student\_placement.ipynb

Run the notebook cells sequentially.

---

## **Requirements**

The required Python libraries are listed in `requirements.txt`:

pandas  
numpy  
matplotlib  
seaborn  
scikit-learn  
jupyter  
notebook

---

## **Limitations**

* The dataset is imbalanced, with substantially more non-placed students.  
* The current models have low recall for the placed class.  
* Placement prediction depends on the quality and representativeness of the dataset.  
* The prediction should be considered an analytical estimate rather than a guarantee of placement.  
* Additional real-world factors such as interview performance, company requirements, market conditions, and communication during actual interviews may affect placement outcomes.

---

## **Future Scope**

Possible improvements include:

* Handling class imbalance using techniques such as SMOTE or class weighting.  
* Hyperparameter tuning.  
* Testing additional machine learning algorithms.  
* Improving recall for the placed class.  
* Developing a web-based prediction interface.  
* Adding interactive dashboards.  
* Using larger and more diverse datasets.  
* Adding explainable AI techniques to explain individual predictions.

---

## **Author**

**Student Placement Prediction Using Machine Learning**

Developed as an academic machine learning project.

