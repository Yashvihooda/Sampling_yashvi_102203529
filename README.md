
### README FILE

#### **Overview**  
Detecting credit card fraud is a crucial challenge, particularly when dealing with highly imbalanced datasets that can degrade machine learning model performance. This project includes:  
1. Balancing the dataset using the Synthetic Minority Oversampling Technique (SMOTE).  
2. Creating five different samples using diverse sampling techniques.  
3. Training five machine learning models on these samples.  
4. Comparing model performance to determine the most effective sampling technique for each model.

---

#### **Dataset**  
The dataset, `Creditcard_data.csv`, contains:  
1. **Features (V1 to V28):** Principal components derived from transaction data.  
2. **Time:** Seconds elapsed between transactions.  
3. **Amount:** Transaction amount.  
4. **Class:** Fraud label (0 for legitimate, 1 for fraud).  

**Class Imbalance:**  
- **Class 0:** 98.83% of transactions are legitimate.  
- **Class 1:** 1.17% of transactions are fraudulent.  

After applying SMOTE, the dataset was balanced to have an equal proportion of legitimate and fraudulent transactions.

---

#### **Sampling Techniques**  
1. **Random Sampling:** Randomly selects a subset of data.  
2. **Stratified Sampling:** Maintains class proportions in the selected subset.  
3. **Systematic Sampling:** Selects every nth sample from the dataset.  
4. **Cluster Sampling:** Divides the dataset into clusters and selects entire clusters.  
5. **Oversampling:** Augments the minority class to address imbalance.

---

#### **Machine Learning Models**  
1. Logistic Regression  
2. Decision Tree  
3. Random Forest  
4. Support Vector Machine (SVM)  
5. Gradient Boosting  

---

#### **Observations**  
Based on the model results:  
1. **Logistic Regression:** Performed best with **Sample 5**, achieving an accuracy of 91.7%.  
2. **Decision Tree:** Performed best with **Sample 4**, achieving an accuracy of 96.3%.  
3. **Random Forest:** Achieved the highest accuracy with **Sample 4**, reaching 98.9%.  
4. **SVM:** Showed improvement across samples but performed best with **Sample 5**, achieving 65.9% accuracy.  
5. **Gradient Boosting:** Reached its peak accuracy of 97.8% with **Sample 4**.

---

This analysis demonstrates how sampling techniques influence model performance and highlights the importance of addressing data imbalance in fraud detection tasks.
