
# Exploratory Data Analysis of Wine Data

The two datasets are related to red and white variants of the Portuguese "Vinho Verde" wine. It has the different contents which use to make the wine such as salt, acid, alcohol levels ,So performed EDA to check which chemical or content effects the quality of wine.

## About Data
Two datasets were combined and few values were randomly removed.
Attribute Information:
**Input variables (based on physicochemical tests):** 1. fixed acidity 2 - volatile acidity 3 - citric acid 4 - residual sugar 5 - chlorides 6 - free sulfur dioxide 7 - total sulfur dioxide 8 - density 9 - pH 10 - sulphates 11 - alcohol Output variable (based on sensory data): 12 - quality (score between 0 and 10)

DataSetInformation:https://www.kaggle.com/datasets/rajyellow46/wine-quality

## Used Tool and Techniques
1. Used tools and techniques to perform this EDA
For withdraw insights from the data ,we must have the following python liberies installed to analyse data deeply.

2. Numpy: NumPy (Numerical Python) . https://numpy.org/doc/stable/user/absolute_beginners.html

3. Pandas: https://pandas.pydata.org/docs/

4. Seaborn: https://seaborn.pydata.org/

5. Matplotlib: https://matplotlib.org/

6. Sklearn: Simple and efficient tools for predictive data analysis https://scikit-learn.org/stable/

7. Google Analytics Colab
## Questions that derived
1. Which type of wine has more good quality & Has higher alcohol content?
2. Which of type of wine is more acidic and has more clorides and also can these affets the quality of wine?
3. Checked whether any relation b/w alcohol content and quality of wine, means if we increase the alcohol level than any effets of quality?
4. Which type of wine has more sugars and dose it can effect quality?
5. Which quality of wine has served at what ph .value?
simier kind of some questions has been drawn inside the notebook. 
## Techniques to performed EDA
1. **Loaded the required libraries**
Numpy, Pandas, Matplotlib, Seaborn, Scikit-learn

2. **Load the dataset**
By help of pandas as pd.read_filetype("Path_name"),load the dataset.

3. **Checked to understood the data**
Reat the first 5 rows and last 5 rows by help of head() and tail() functions.

4. **Checked information of data**
By help of info() fuctions checked the information such as how many column are there and what is the lenghts.

5. **Stistical analysis of data**
1. After checking lenght and columns of dataset i did the Stistical analysis by help of describe() function for both numerical and categorical columns which give 5 point analysis.

2. Than checked shape of data to get the actual lengh of rows and columns

3. Than Checked stistical analysis for string or categorical columns bu df.describe(include="O")

4. Than also returns the each column names and stored as list seperatly as categorical columns and numerical colums.

6. **Exploratory data analysis**
1. So after extracting the structure of data, Now i started the EDA part to mining the data by visualization of each columns.

2. Ananlysis of each numerical columns and categorical columns to derive insights by using diffrents pandas and numpy functions, which able to give us the different usefull insights.
numerical_columns=['fixed acidity', 'volatile acidity', 'citric acid', 'residual sugar',
       'chlorides', 'free sulfur dioxide', 'total sulfur dioxide', 'density',
       'pH', 'sulphates', 'alcohol', 'quality']

3. Statistical anlysis of each numerical columns and after ,By help of Histogram, Distribution plot , Box plot i successfully derived insights about each numerical columns , and by help of pie charts & count plots able to visualize categorical columns indivisually.

4. After combining numerical and categorical columns by help of bar diagrame, scatter plot, line plot, successfully extracted insights from data.

5. Visualiing those insights to make it interactive by diffrent techniques of Seaborn and Matplotlib by charts such as Histogram,Distribution plot ,Box plots for each nuerical columns and countplots for each categorical colums.

6. Sucessfully derive all the possible insights from the data with multiple trends ,that how the bbuisiness is going and how we can improve in functions.

7. Tried to derived correlation b/w some of columns to find relationships by using Heatmaps and regplots. Whether columns and other values effects the quality of wine.

#Data wranggling 
1. **Handled mssing values**
2. Removing np.nan values of missing values by replecing with specific mean or median of the column.
3. **Dropping duplicates**
4. Than checked for duplicates by trying to find the shape of dataset again after applied drop_duplicates()
4. **Outliers handling** 
5. Than handled outliers for each numerical columns the make the data more accurate and need to set the column to represent by their mean. #Standrization 
6. **Standrization**
 of each categorical and numeical columns that can help us in model building part. 20. Handling columns of Standrization of each numerical and categorical columns

Than handled categorical columns by One hot encoding pd.get_dummies() and numerical columns by minmax scaler and stadard scaler to standarize numerical columns.
## Conclusion
So, we can easily meke Conclusion after analyzing the data that the yes higher alcohot content is making the quality of wine very good, 
10% of wine has alcohol content 9.1 and below.
25% of wine has alcohol content 9.5 and below.
50% of wine has alcohol content 10.3 and below.
75% of wine has alcohol content 11.3 and below.
90% of wine has alcohol content 12.3 and below.