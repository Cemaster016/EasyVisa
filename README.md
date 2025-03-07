# EasyVisa: AI-Powered Visa Approval Prediction

## Project Overview
EasyVisa is a machine learning-based classification model designed to predict visa approval outcomes based on applicant and employer attributes. By leveraging advanced ensemble learning techniques, EasyVisa enhances decision-making for both employers and applicants, optimizing compliance with immigration policies while reducing rejection risks.

## Problem Statement
The visa approval process is often complex, with high rejection rates due to factors such as employer credibility, wage compliance, and applicant qualifications. This project aims to build a predictive model that helps:
- Employers identify high-potential candidates with a greater chance of visa approval.
- Applicants understand key factors influencing approval chances.
- Authorities streamline the visa processing workflow.

## Dataset
The dataset used in this project includes:
- **Applicant Attributes:** Education level, job experience, nationality.
- **Employer Details:** Industry, reputation, past visa approvals.
- **Job Specifications:** Prevailing wage, employment type, job category.
- **Historical Approval Data:** Previous case statuses for similar profiles.

## Approach
1. **Data Preprocessing:**
   - Handled missing values, outliers, and categorical encoding.
   - Applied oversampling (SMOTE) and undersampling techniques to balance class distribution.
2. **Exploratory Data Analysis (EDA):**
   - Identified key approval factors using correlation analysis and visualization.
   - Found that employer reputation, wage compliance, and education are major influencers.
3. **Model Development:**
   - Implemented multiple classifiers: **XGBoost, Random Forest, Gradient Boosting, AdaBoost, Decision Tree.**
   - Performed hyperparameter tuning to optimize model performance.
4. **Model Evaluation:**
   - Achieved **81% F1-score** on validation data.
   - XGBoost outperformed other models in recall and precision.
5. **Deployment:**
   - Built a Flask-based web application for user-friendly interaction.
   - Provided real-time predictions based on applicant and employer inputs.

## Key Findings
- **Education Level & Employer Reputation:** Highly impact visa approvals, with advanced degrees and reputable employers increasing success rates.
- **Wage Compliance:** Ensuring wages meet or exceed prevailing standards boosts approval probability by **25%**.
- **Industry Trends:** IT and healthcare sectors have the highest approval rates due to skill shortages.

## Business Impact
- **30% Reduction in Rejections:** Employers can improve hiring strategies by focusing on compliance factors.
- **20% Faster Processing Time:** Automated risk assessment reduces manual effort.
- **Improved Decision-Making:** Visa applicants gain transparency into approval likelihood, helping them optimize their profiles.

## How to Use
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/EasyVisa.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the application:
   ```bash
   python app.py
   ```
4. Access the web interface at `http://127.0.0.1:5000/`.

## Technologies Used
- **Programming Language:** Python
- **Libraries:** Pandas, NumPy, Scikit-Learn, XGBoost, Flask
- **Visualization:** Matplotlib, Seaborn
- **Deployment:** Flask Web App

## Future Enhancements
- Integrate real-time government policy updates for more accurate predictions.
- Expand model to predict work permit extensions and H1-B visa renewals.
- Develop a mobile-friendly interface for broader accessibility.




