# Wine Quality Classifier
You can download the dataset from my Github repository: https://github.com/rodrickmascarenhas/wine-quality

The dataset is related to red and white variants of the Portuguese "Vinho Verde" wine. For more details, consult: <a href="https://www.vinhoverde.pt/en/">[Web Link]</a>  or the reference [Cortez et al., 2009]. 

In the above reference, we are conducting study on wine samples. The inputs include objective tests (e.g. PH values) and the output is based on sensory data (median of at least 3 evaluations made by wine experts). Each expert graded the wine quality between 0 (very bad) and 10 (very excellent). Due to privacy and logistic issues, only physicochemical (inputs) and sensory (the output) variables are available (e.g. there is no data about grape types, wine brand, wine selling price, etc.).

The classes are ordered and not balanced (e.g. there are many more normal wines than excellent or poor ones). No missing values were found. Outlier detection algorithms could be used to detect the few excellent or poor wines. Additionally, we are using feature selection techniques.

## Goal

The objective is to classify the data into the various quality score categories. A list of machine learning models will be trained and tested to determine which will yield the best results in this multinomial classification problem:

- Support Vector Machines (SVM)
- Decision Trees
- Random Forest
- Linear Regression
- Logistic Regression

## Checking for Outliers

Eliminating outliers from our dataset to limit the z-score values to 3.

## Exploratory Data Analysis

![correlation-heatmap](https://github.com/rodrickmascarenhas/wine-quality/assets/30309234/e5fe8395-71c0-4a2c-abba-0041386a8fd7)

It appears that volatile acidity values appear to be most correlated with quality

## Results

![actual-expected-results](https://github.com/rodrickmascarenhas/wine-quality/assets/30309234/2009c506-50ea-4284-bc23-056ae2902da8)

Best Scaler: Standard Scaler
<br />Best Feature Selection: Variance Threshold
<br />Best Model: SVM
<br /> Best Accuracy Score: 67%
