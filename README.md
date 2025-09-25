# Decision-Tree-Personal-Loan-Campaign-Case-Study-AllLife-Bank-
![alt text](<Assets/Personal Loan Campaign Image.jpg>)

## Business Context
AllLife Bank is a U.S.-based bank with a strong depositor base (liability customers) but a relatively small borrower base (loan customers).  
The bank wants to **increase personal loan adoption** by converting some of its depositors into borrowers without losing them as depositors.  

Last year, a campaign achieved **9% success in loan conversions**, which showed potential. The marketing team now wants to improve that number with smarter targeting.

---

##  Objectives
This project has three main goals:
1. **Predict Loan Acceptance** – Build a model to identify customers likely to accept a personal loan.  
2. **Identify Key Drivers** – Understand which customer attributes (e.g., income, education, spending) most influence loan acceptance.  
3. **Segment Customers** – Highlight customer groups with the highest probability of loan uptake for targeted marketing campaigns.  

---

## Data Overview
- **Source**: Bank customer dataset with **5,000 records** and **14 variables**.  
- **Features**: Age, Income, Education, Family size, Mortgage, Credit Card spending, etc.  
- **Target Variable**: `Personal_Loan` (1 = Accepted, 0 = Not Accepted).  
- **Acceptance Rate**: ~9% (480 out of 5,000 customers accepted loans).  

---

##  Approach
1. **Data Cleaning & Preprocessing**
   - Fixed anomalies (e.g., negative values in experience).
   - Converted categorical variables (e.g., Education, ZIPCode).
   - Removed irrelevant identifiers (e.g., Customer ID).

2. **Exploratory Data Analysis**
   - Found that higher income, larger family size, and higher education levels strongly correlate with loan acceptance.
   - Spending patterns (credit card usage) also signal likelihood of loan uptake.

3. **Model Building**
   - Built a **Decision Tree model** to predict personal loan acceptance.  
   - Applied **pre-pruning** and **post-pruning** to avoid overfitting and improve generalization.  

4. **Model Evaluation**
   - Final post-pruned model achieved:  
     - **Accuracy**: 97.9%  
     - **Recall**: 85.2%  
     - **Precision**: 93.4%  
     - **F1 Score**: 89.1%  

---

##  Key Insights
- **Income**: Customers with incomes **> $100K** are significantly more likely to accept loans.  
- **Education**: Graduate and Advanced degree holders show higher loan uptake.  
- **Spending**: Customers spending **> $4K/month** on credit cards are strong prospects.  
- **Family**: Households with **3–4 members** are more likely to accept loans.  

---

##  Business Recommendations
1. **Target High-Income, Educated Customers** – Focus on graduates/advanced degree holders earning above $100K.  
2. **Leverage Spending Patterns** – Prioritize customers with above-average monthly credit card spending.  
3. **Family-Oriented Offers** – Tailor personal loan campaigns to families of 3–4 members (e.g., home improvement, education loans).  
4. **Optimize Campaign Efficiency** – Use the model’s probability scores to prioritize high-potential customers, reducing costs by avoiding low-likelihood segments.  

---

## Technical Stack
- **Language**: Python  
- **Libraries**: Pandas, NumPy, Matplotlib, Scikit-learn  
- **Model Used**: Decision Tree Classifier (with pruning for optimization)  

---

##  Results
- The model can **accurately identify potential loan buyers** while keeping false positives low.  
- It provides **actionable customer segments** for marketing campaigns.  
- Using this model, AllLife Bank can **increase conversion rates beyond the previous 9% baseline**.  

---

