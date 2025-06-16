🧾 Loan Prediction - Internship Task
Objective
The goal of this task is to build a machine learning model that can predict whether a loan application will be approved or not, based on various applicant attributes like income, education, and credit history.

 Dataset Description
The dataset contains information about previous loan applicants, including:

Demographic features: Gender, Marital Status, Dependents, Education

Financial details: ApplicantIncome, CoapplicantIncome, LoanAmount, Loan_Amount_Term, Credit_History

Other features: Self_Employed, Property_Area
The target variable is Loan_Status, which indicates whether the loan was approved (Y) or not (N).

 Data Cleaning & Preprocessing
Handled missing values in both numerical and categorical columns using median and mode.

Replaced '3+' in Dependents with numeric value 3.

Encoded categorical variables using Label Encoding.

Scaled numerical features using StandardScaler.

Dropped irrelevant columns like Loan_ID.

📊 Exploratory Data Analysis (EDA)
Visualized the distribution of LoanAmount, ApplicantIncome.

Plotted Loan Status counts and income comparisons by Education.

Identified feature relationships and outliers to improve understanding.

 Model Training
Split data into training and test sets (80/20).

Trained a Logistic Regression model with class balancing.

Applied feature scaling to improve model performance.

 Model Evaluation
Achieved an accuracy of approximately 77.2%.

Confusion Matrix and Classification Report showed:

High recall for approved loans (1 class).

Balanced precision and F1-score.

✅ Key Insights
Credit_History had a strong impact on loan approval.

Logistic Regression performed well with simple preprocessing.

Model is suitable for basic binary classification in finance.

 Tools & Libraries
Python, Jupyter Notebook

Pandas, NumPy, Matplotlib, Seaborn

Scikit-learn (for model building and evaluation)

 Conclusion
The loan prediction model successfully meets the task objective. With clean data and basic classification techniques, we achieved a reasonably accurate and interpretable model. Future improvements could include using Decision Trees or ensemble methods for better performance.
