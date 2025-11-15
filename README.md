# Travel Insurance Project

## Context
A Tour & Travels Company is offering a travel insurance package to its customers. **The new insurance package also includes COVID cover** (hereinafter called: **"COVID Insurance"** for short). The company requires a system to predict which customers would be interested in buying this insurance package based on historical database records.

The insurance was initially offered to some customers in 2019, and the provided dataset has been extracted from the sales performance of the package during that period.

---

## Content
The dataset includes the following features:

1. **Age**: Age of the customer.
2. **Employment Type**: The sector in which the customer is employed.
3. **GraduateOrNot**: Whether the customer is a college graduate or not.
4. **AnnualIncome**: The yearly income of the customer in Indian Rupees (rounded to the nearest 50,000).
5. **FamilyMembers**: The number of members in the customer’s family.
6. **ChronicDisease**: Whether the customer suffers from any major conditions like diabetes, high blood pressure, or asthma.
7. **FrequentFlyer**: Derived data indicating whether the customer booked air tickets on at least 4 different instances in the last 2 years (2017-2019).
8. **EverTravelledAbroad**: Whether the customer has ever traveled to a foreign country (not necessarily using the company’s services).
9. **TravelInsurance**: Whether the customer bought the travel insurance package during the introductory offer in 2019.

---

## Goal
The objective is to build an intelligent predictive model that can determine if a customer will be interested in buying the travel insurance package.

---

## Summary of Analysis
- **Dataset Overview**: The analysis was performed on a sample of Indian customers who were offered COVID Travel Insurance in 2019.
- **Customer Profile**: The majority of the customers are wealthy, college graduates, employed in the private sector, and free of chronic diseases. Most had flown less than 4 times between 2017 and 2019 and had never traveled abroad.
- **Predictive Model**: A machine learning model ensemble was created using the Voting Classifier, combining three high-performing models:
  1. Radial Support Vector Machine (RBF SVM)
  2. k-Nearest Neighbors (KNN)
  3. Random Forest Classifier
- **Preprocessing**: The Standard Scaler was applied to ensure feature scaling before modeling.
- **Feature Importance**: The most significant predictor of customer behavior was **Annual Income**. Wealthier customers were more likely to buy the COVID Insurance package, likely due to the costlier holidays and trips they book.

---

## Further Improvement
To enhance the model’s performance and applicability, consider the following improvements:

1. **Advanced Models**:
   - Implement more complex algorithms like XGBoost, LightGBM, CatBoost, or Neural Networks.

2. **Hyperparameter Tuning**:
   - Explore alternative tuning methods such as Random Search and Bayesian Optimization.

3. **Feature Selection**:
   - Use advanced techniques like Recursive Feature Elimination (RFE) for feature selection.

4. **Evaluation Metrics**:
   - Experiment with additional metrics such as ROC-AUC, F1-Score, and Precision-Recall curves for better evaluation of model performance.

5. **Cross-Validation**:
   - Apply advanced cross-validation techniques such as Stratified K-Fold to ensure balanced and robust training.

---

## Instructions for Downloading
1. Clone this repository to your local machine:
   ```bash
   git clone <repository_url>
   ```

2. Navigate to the project directory:
   ```bash
   cd <project_directory>
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run the analysis or model training scripts as per the provided documentation.

---

## Conclusion
This project demonstrated the feasibility of predicting customer interest in COVID Travel Insurance using machine learning models. While initial results are promising, further refinements in modeling techniques and hyperparameter tuning can significantly improve predictive accuracy and generalizability.

