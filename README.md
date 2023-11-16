# Using Machine Learning to Diagnose Diabetes

## 0. Abstract
Diabetes is more prevalent among the Pima Indian tribe of southern Arizona than any other population globally(1). This paper demonstrates the accurate diagnosis of diabetes in Pima women by optimizing parameters for three machine learning algorithms: Random Forest decision trees, a Support Vector Machine (SVM), and a Multilayer Perceptron (MLP) artificial neural network (ANN). These results underscore the potential of machine learning as a valuable tool for assisting doctors in disease diagnosis.

## 1. Introduction
This study explores the application of machine learning in the field of medicine. Can statistical learning algorithms aid doctors in making accurate diagnoses and informed decisions about patient health? To answer this question, we trained three distinct machine learning algorithms—Random Forest decision trees, a Support Vector Machine (SVM), and a Multilayer Perceptron (MLP) artificial neural network—using data on diabetes occurrences in Pima Indian Women. All analyses were conducted using the R statistical computing software package within the RStudio integrated development environment. Our findings indicate that all three algorithms achieved a high success rate in correctly diagnosing diabetes in Pima women, providing support for the hypothesis that machine learning has a role in a doctor’s toolkit.

### 1.1 About the Data
The data on diabetes incidence in Pima women used in this analysis are freely available from the University of California, Irvine Machine Learning Repository at [http://archive.ics.uci.edu/ml/](http://archive.ics.uci.edu/ml/). This dataset was created to predict the onset of diabetes in women from the Pima Indian Tribe, containing 768 observations of nine features.

| Feature Description                                       | Feature Name in Dataset  |
|----------------------------------------------------------|--------------------------|
| Number of times pregnant                                  | timesPregnant            |
| Plasma glucose concentration at 2 hours in an OGTT         | plasmaGlucose            |
| Diastolic blood pressure (mm Hg)                          | diastolicPressure        |
| Triceps skin fold thickness (mm)                          | tricepThickness          |
| 2-Hour serum insulin (mu U/ml)                            | serumInsulin             |
| Body mass index (weight in kg/(height in m)^2)             | bmi                      |
| Diabetes pedigree function                                | pedigreeFunction         |
| Age (years)                                               | age                      |
| Class variable (diabetic or not diabetic)                 | diabetes                 |

A comprehensive description of this dataset is available at: [https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2245318/](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2245318/)

### 1.2 Software Used in Analysis
All analyses were performed using the R statistical computing environment, with extended functionality provided by the following software libraries: caret, mice, randomForest, kernlab, VIM, and RSNNS. These libraries support data imputation and the three machine learning algorithms used in this analysis.
The analysis was conducted within the RStudio integrated development environment, and this report was generated using the rmarkdown library.

### 1.3 Outline of Analysis
The analysis workflow included data loading, exploratory analysis, missing data imputation, data standardization, splitting data into training and test sets, model construction, parameter optimization, and model evaluation.
