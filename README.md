# Adult Dataset Analysis - Income Prediction

**Description**
This project uses the Adult (Census Income) dataset from sklearn.datasets to perform data analysis and visualization for predicting whether an individual's annual income exceeds $50,000. The dataset contains demographic attributes such as age, sex, education, occupation, and native country.

**Purpose**
The main objective of this project is to understand key factors that influence income levels and to prepare the dataset for machine learning models in future stages.

**Technologies and Libraries Used**
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

  **Steps Performed**
1. Data Loading and Exploration
- The dataset is loaded using fetch_openml with the name 'adult'.
- The number of records and features is displayed.
- Basic information, including data types and non-null counts, is explored using .info().
- Minimum and maximum values of numerical features are computed.

**2. Handling Missing Data**
- Missing values in the columns workclass, occupation, and native-country are filled with the mode (most frequent value) of each respective column.

**3. Data Transformation**
- The target variable class is converted to binary: <=50K to 0 and >50K to 1.
- The sex column is also converted to binary: Male to 1 and Female to 0.

**4. Data Exploration**
- The class distribution (income levels) is visualized using bar and pie charts.
- The education-num column is binned into four categories: Low, Medium, High, and Very High using quartiles.
- The mean, median, and mode of the education-num feature are calculated.

**5. Correlation Analysis**
- The correlation matrix of all numerical features is computed.
- Features that are strongly correlated (correlation > 0.2) with income are identified.
- A heatmap is used to visualize the correlation matrix.

**6. Additional Visualizations**
- Distribution of education-num is shown using a density plot.
- A scatter plot is created for age vs hours-per-week.
- Class distributions are further analyzed by race and sex using count plots.
