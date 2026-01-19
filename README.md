# Lead Scoring & Conversion Prediction using Logistic Regression
<img width="300" height="423" alt="image" src="https://github.com/user-attachments/assets/422739f0-651b-4eab-a4c1-f19c8eb9ac64" />

## Project Overview
In high-volume marketing environments, sales teams often face limited capacity and cannot follow up with every incoming lead. This project addresses that challenge by building a **lead scoring system** that predicts the probability of lead conversion and prioritizes leads based on business value.

Using historical lead interaction data, a machine learning model assigns a **lead score (0–100)** to each prospect, enabling the sales team to focus on high-probability leads and improve overall conversion efficiency.

---

## Business Objective
The primary goals of this project are:
- Predict the probability of lead conversion
- Convert probabilities into an interpretable lead score
- Segment leads into actionable priority buckets
- Quantify business impact using lift analysis

---

## Files Including
This projects includes 4 files as:
  1. Leads.csv - Dataset containing information about leads along with target variable
  2. Leads_Data_Dictionary.csv - A brief description about all the features in the Dataset
  3. Lead_Scoring_and_Conversion_Analysis.ipynb - The project file
  4. Business Subjective Questions - Contains few important business oriented questions and their answers according to the result of the model

---

## Dataset Description
The dataset contains information on leads generated through various marketing channels, including:
- Demographics and location
- Lead source and origin
- Website interaction metrics
- Sales interaction history

The target variable indicates whether a lead ultimately converted.

<img width="1799" height="205" alt="image" src="https://github.com/user-attachments/assets/ffd995f9-54cb-4ef8-89ed-f78bffd4f946" />

---

## 🔍 Project Workflow

1. **Business Understanding**  
   Defined the problem, objectives, and success criteria from a sales-efficiency perspective.

2. **Data Cleaning**  
   - Handled missing values and invalid categories  
   - Removed columns with excessive missing data  
   - Standardized categorical values  

3. **Exploratory Data Analysis (EDA)**  
   - Identified class imbalance  
   - Analyzed key behavioral and engagement patterns  

4. **Data Preparation**  
   - One-hot encoded categorical variables  
   - Scaled numerical features  
   - Performed train–test split to avoid data leakage  

5. **Modeling Strategy**  
   - Logistic Regression chosen for interpretability and business explainability  
   - Used sklearn for robust, production-ready modeling  
   - Statsmodels explored selectively for feature insights  

6. **Model Evaluation**  
   - Evaluated using ROC-AUC, precision, recall, and confusion matrix  
   - Accuracy intentionally deprioritized due to class imbalance  

7. **Cutoff Optimization**  
   - Used Precision–Recall tradeoff to select a business-driven probability cutoff  

8. **Lead Scoring System**  
   - Converted probabilities into a 0–100 lead score  
   - Segmented leads into Hot, Warm, Cold, and Drop categories  

9. **Business Impact & Lift Analysis**  
   - Compared model-driven targeting vs random targeting  
   - Measured conversion capture and lift at different lead percentiles
  
## Key Visuals
### 1. Target Variable Distribution

<img width="270" height="271" alt="image" src="https://github.com/user-attachments/assets/0809c925-7da1-4b66-91fe-8c96788c9382" />

### 2. ROC Curve

<img width="536" height="468" alt="image" src="https://github.com/user-attachments/assets/c727c1fb-7df5-41fd-bac1-257f49f87a0c" />

### 3. Precision vs Recall curve

<img width="536" height="468" alt="image" src="https://github.com/user-attachments/assets/a91909d5-0896-4590-87f9-70d524ddc591" />

### 4. Bucket Distribution

<img width="549" height="456" alt="image" src="https://github.com/user-attachments/assets/0d32e277-8fa7-4e8f-bbb9-44bd18388cd1" />

---

## Key Results
- **Top 3 variables contributing the lead conversions are:
  1. Total time spent on website
  2. Last Activity – Had a Phone Conversation / SMS Sent
  3. Lead Source (e.g., Welingak Website / Referral Sites)
- **Top 20% of model-ranked leads capture ~51% of total conversions**
- **Lift of ~2.5×** compared to random lead targeting
- Clear monotonic increase in conversion rates across lead score buckets

These results demonstrate that the model effectively prioritizes high-value leads and significantly improves sales efficiency.

---

## Business Insights
- Leads spending more time on the website show higher conversion likelihood  
- Specific lead interaction tags strongly indicate purchase intent  
- Targeted outreach can drastically reduce wasted sales effort  

---

## Conclusion
This project demonstrates how a well-designed machine learning solution can drive tangible business value. By focusing sales efforts on high-probability leads, organizations can:
- Improve conversion rates  
- Optimize sales team productivity  
- Increase ROI without increasing marketing spend  

---

## Tech Stack
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- Statsmodels  

---

## Author
**Ishant Cane**  
Aspiring Data Scientist | Machine Learning | Business Analytics  

---

⭐ If you found this project useful, feel free to star the repository!
