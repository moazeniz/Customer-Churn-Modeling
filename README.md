# Customer Churn Prediction Project  

This project is focused on predicting customer churn using machine learning algorithms. Churn is a key business metric that reflects the percentage of customers who discontinue their subscription or stop using a service. By identifying factors that influence churn, businesses can proactively retain customers and enhance customer satisfaction.  

## Features  

The dataset used for this project contains 14 columns representing customer behaviors and attributes:  

1. **Call Failure**: Number of failed calls.  
2. **Complains**: Complaints made by the customer.  
3. **Subscription Length**: Duration of the customer's subscription in months.  
4. **Charge Amount**: Amount charged to the customer.  
5. **Seconds of Use**: Total seconds of service usage.  
6. **Frequency of Use**: How often the service is used.  
7. **Frequency of SMS**: Number of SMS messages sent.  
8. **Distinct Called Numbers**: Number of unique contacts.  
9. **Age Group**: Age group of the customer.  
10. **Tariff Plan**: The customer's selected tariff plan.  
11. **Status**: Subscription status (active/inactive).  
12. **Age**: Age of the customer.  
13. **Customer Value**: Value score assigned to the customer.  
14. **Churn**: Target variable indicating whether the customer churned (Yes/No).  

---

## Machine Learning Algorithms  

The following machine learning algorithms were implemented to classify customer churn:  

### 1. **CART (Classification and Regression Tree)**  
   - **Criterion**: Gini impurity.  
   - Implemented using `DecisionTreeClassifier`.  

### 2. **ID3 (Iterative Dichotomiser 3)**  
   - Approximated using entropy as the splitting criterion.  

### 3. **C4.5**  
   - Based on entropy, similar to ID3, implemented with adjustments to simulate the behavior of C4.5.  

### 4. **Extra Tree Classifier**  
   - A randomized version of decision trees that improves variance reduction.  

### 5. **Random Forest Classifier**  
   - An ensemble of decision trees to improve prediction accuracy and reduce overfitting.  

### 6. **Gradient Boosting Classifier**  
   - A boosting algorithm that builds models sequentially to minimize errors.  

### 7. **AdaBoost Classifier**  
   - Adaptive boosting with decision trees as the base estimator.  

### 8. **XGBoost Classifier**  
   - An optimized gradient boosting algorithm for better performance and scalability.  

---

## Installation  

To set up this project locally:  

1. Clone the repository:  
   ```bash  
   git clone https://github.com/your_username/customer-churn-prediction.git  
   cd customer-churn-prediction  
   ```  

2. Install dependencies:  
   ```bash  
   pip install -r requirements.txt  
   ```  

3. Run the scripts:  
   ```bash  
   python train_and_evaluate.py  
   ```  

---

## Results  

Each algorithm was evaluated on the dataset using performance metrics such as accuracy, precision, recall, and F1 score. Detailed results and comparisons can be found in the `results` folder.  

---

## Key Takeaways  

1. Decision tree algorithms like **CART**, **ID3**, and **C4.5** provide interpretable models but may suffer from overfitting.  
2. Ensemble methods like **Random Forest** and **Gradient Boosting** offer higher accuracy and robustness.  
3. **XGBoost** demonstrated superior performance due to its advanced optimization techniques.  

---

## Contributing  

Contributions are welcome! If you would like to enhance this project, please submit a pull request or create an issue for discussion.  

---

## License  

This project is licensed under the [MIT License](LICENSE).  

---

## Acknowledgments  

Special thanks to the contributors and open-source libraries used in this project, including `scikit-learn`, `xgboost`, and `numpy`.  

---

## Citation  

This project utilized the **"Iranian Churn"** dataset from the UCI Machine Learning Repository:  

"Iranian Churn," UCI Machine Learning Repository, 2020. [Online]. Available: [https://doi.org/10.24432/C5JW3Z](https://doi.org/10.24432/C5JW3Z).  

Please cite this source if you build upon or reference this project.
