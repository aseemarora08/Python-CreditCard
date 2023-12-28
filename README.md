# Python-CreditCard

**Introduction:**

This project delves into credit card applications, scrutinizing diverse factors such as gender, age, debt history, and employment duration to assess an applicant's reliability for bank approval. The central question is whether we can predict successful credit card applications using a multivariate business dataset from Quinlan, J. R. The dataset encompasses a mix of integer, real, and categorical variables, including "Gender," "Age," "Debt," "CreditScore," and more. This exploration aims to unravel the complex relationships influencing credit card approval decisions.

**Preliminary Exploratory Data Analysis:**
- Imported necessary packages, read data from a Google spreadsheet, and cleaned it for analysis.
- Altered categorical column values for better readability.
- Created separate datasets for male and female applicants to examine gender-specific effects on approvals.

**Dataset Split and Summary:**
- Split the dataset into training and testing sets for model evaluation.
- Provided comprehensive data summaries, including non-null columns, quantitative variable descriptions, approval statistics by gender, and means of predictor variables.

**Data Visualization:**
- Visualized approvals by gender using bar charts.
- Explored predictor variable distributions through histograms.

**Methods:**
- Planned to train a classification model using various factors to predict credit card approval.
- Considered additional columns, such as the percentage of ethnic groups, to enhance prediction insights.
- Utilized scatter plots, facet functions, bar graphs, or pie charts for detailed relationship visualization and comparisons.

**Expected Outcomes and Significance:**
**Expected Findings:**
- Anticipated uncovering potential biases among ethnicities, genders, and social classes in credit card approvals.
**Impact of Findings:**
- Significance lies in highlighting biases within the approval system, paving the way for improvements that ensure equal opportunities.
**Future Questions:**
- Potential future inquiries include identifying and rectifying biases in credit card approval, improving the system for fairness, assessing the impact of prior debt on approval, and developing predictive tools for approval likelihood.



## **Credit Card: *Navigating Insights and Building Models***

For this comprehensive analysis of credit card applications, I delved into various factors, including gender and employment history, to evaluate applicants' reliability for bank approval. My traditional focus on credit score as a primary consideration for loan and credit card decisions, as highlighted by Wagner (2004), prompted a nuanced exploration. The comparison of credit score with debt history, age, and income led to the development of a KNN-Neighbors algorithm, aiming to predict approvals based on the "Credit Approval" dataset from the UC Irvine Machine Learning Repository.

The model-building journey commenced with the import of relevant packages, data transfer to a Google spreadsheet, and subsequent loading into the workspace as "data" using the read_csv function. Streamlining the dataset by dropping unnecessary columns, our attention honed in on pivotal variables: "Debt," "Income," "Age," and "CreditScore." Preliminary steps involved generating summary statistics, crafting visualizations, and constructing scatter plots, all amplifying the critical role of credit score in approval dynamics.

A meticulous application of KNN-Neighbors analysis ensued, involving the selection of the optimal number of neighbors through an evaluation of accuracy and standard error across various values (7, 11, 15, 25, etc.). The integration of a preprocessor featuring StandardScaler() for quantitative predictors maintained the integrity of "approved" data. Cross-validation outcomes were promising, revealing a reliable classifier with a mean test score of 75% and a standard error of 2.5%.

To augment predictive capabilities, I created new observations and predicted their approval status using the established model. Visualizing nearest neighbors offered enhanced insights, spotlighting the robust correlation between credit score and income with approvals, while age and debt exhibited a comparatively lesser impact.

These revelations bear substantial significance, guiding the refinement of approval criteria, the mitigation of biases in decision algorithms, and the pursuit of fairer financial systems. The path forward involves further exploration to assess model generalization and consider additional features for heightened accuracy. In conclusion, this analysis serves as a beacon illuminating the intricacies of credit card approval dynamics, underscoring the perpetual need for exploration, ethical considerations, and a nuanced understanding of the multifaceted factors shaping financial decisions.

**References:**

Quinlan,J. R.. Credit Approval. UCI Machine Learning Repository. https://doi.org/10.24432/C5FS30.
Surekha, M., Umesh, U., & Dhinakaran, D. P. (2022). A study on utilization and convenient of credit card. Journal of Positive School Psychology, 5635-5645.

Wagner, H. (2004). The use of credit scoring in the mortgage industry. Journal of Financial Services Marketing, 9(2), 179–183. https://doi.org/10.1057/palgrave.fsm.4770151
