# Classification-of-agricultural-crops


Academic Context

This project was carried out as part of a university assignment for the course *Object-Oriented Programming* at Universidad del CEMA (UCEMA). The main objective was to apply data analysis tools in Python to build a model capable of classifying different types of agricultural crops based on climatic and soil chemical variables.

---

Procedure

Data Loading and Exploration

- The dataset included variables such as nitrogen, phosphorus, and potassium content, temperature, relative humidity, pH level, and precipitation.
- A preliminary cleaning was performed, removing unnecessary columns (e.g., `Unnamed: 0`), and the dataset structure was inspected using `.info()` and `.describe()`.

Visualization and Exploratory Analysis

- Outliers were visualized using customized boxplots, and variable distributions were analyzed with histograms.
- A heatmap of the correlation matrix was constructed to identify relationships between variables.

Data Encoding and Preparation

- The target variable `Tipo_de_Cultivo` was transformed using OneHotEncoding, converting each crop type into a binary column.
- A new dataset (`cultivos2`) was generated, including only the numeric predictor variables for analysis.

Modeling and Evaluation

- Classification models were trained using multinomial logistic regression (`statsmodels.formula.api`), fitting a model with the predictor variables.
- Model performance metrics were reviewed to evaluate the predictive ability of the system.

---

Conclusions

- The analysis revealed how certain soil and climate variables are associated with specific crops, such as relative humidity or nitrogen levels.
- Encoding using OneHotEncoder facilitated the transformation of a multiclass categorical variable into a format suitable for supervised algorithms.
- The project demonstrated the applicability of machine learning in the agricultural field, opening possibilities to improve decision-making in agronomy based on objective data.
- This project served to reinforce skills in data analysis, modular programming, and the use of key Python libraries such as `pandas`, `seaborn`, `scikit-learn`, and `statsmodels`.
