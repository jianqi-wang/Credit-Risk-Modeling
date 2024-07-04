# Credit-Risk-Modeling Project
This is part of a comprehensive Python-based project on credit risk modeling, encompassing everything from data preprocessing, through probability of default (PD) modeling, loss given default (LGD), and exposure at default (EAD) modeling, to calculating expected loss (EL). It is one of the most critical activities in banking, receiving heightened attention since the financial crisis.
## Data Source
The dataset is sourced from Lending Club and contains complete loan data for loans issued from 2007 to 2015, including the current loan status (Current, Late, Fully Paid, etc.) along with the latest payment information. Additionally, the dataset includes extra features such as credit scores, the number of finance inquiries, address information, and more, covering approximately 890 thousand observations and 75 variables. Detailed information and a data dictionary are available on the original dataset page.
## Main Modeling Techniques
The project is implemented in Python, with key modeling steps including:

1. Data Preprocessing: Cleaning and formatting data to prepare for modeling.
2. Probability of Default (PD) Modeling: Using logistic regression to analyze the probability of a borrower defaulting.
3. Loss Given Default (LGD) and Exposure at Default (EAD) Modeling: Assessing the potential loss percentage and exposure amount in the event of a default. Loss Given Default (LGD) and Exposure at Default (EAD) Modeling: This process is broken down into two phases:
Phase 1: Determines whether the recovery rate is zero, in which case the regression outcome is zero.
Phase 2: If the recovery rate is not zero, the model then predicts the specific value of the recovery rate.
4. Expected Loss (EL) Calculation: Combining PD, LGD, and EAD to compute the expected credit losses.
## Tools and Libraries Used
Due to the considerable size of the dataset (702 MB), the project is developed using Google Colab for its cloud-based hardware acceleration. Key Python libraries employed include:

1. pandas and numpy for data manipulation and numerical calculations.
2. scikit-learn for data splitting, training models, and performance evaluation.
3. statsmodels for in-depth statistical analysis.
4. matplotlib and seaborn for visualizing the data.
## Quick Glance at the Results
### ROC OF PD

<img width="584" alt="PD_ROC" src="https://github.com/jianqi-wang/Credit-Risk-Modeling/assets/171050967/714daa4b-d4fa-44c2-a895-cb52b258a8c3">

### KS-OF PD
<img width="570" alt="PD_KS" src="https://github.com/jianqi-wang/Credit-Risk-Modeling/assets/171050967/4c8d6f52-2aca-4ef0-ba78-d075e73eae45">

### Confusion Matrix of LGD
<img width="192" alt="CM" src="https://github.com/jianqi-wang/Credit-Risk-Modeling/assets/171050967/25c5a6b5-0f01-4dca-b643-88087bd30383">

