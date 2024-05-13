# Montana State University Math Placement

## Introduction

As part of my MSBA capstone project, the code in this repository analyzes math placement at Montana State University. The python code included, reviews the accuracy of the current placement model and explores multiple machine learning models, using ACT/SAT, reported high school GPA and Ed Ready scores to assist in predicting math placement for incoming freshmen.

## Code Blocks Explained

### Block 1

This chunk of code imports all of the packages necessary to preform transform the data and preform statistical analysis.This also, reads in the data from the two data files (math_placement2024-02-29 and edready_raw_scores).

### Block 2

Here, historical students grades are tagged as "Successful" or "Unsuccessful". Students who received a C+ or lower were coded as "Unsuccessful" and students who received a B- or higher were "Successful". Courses and course combinations were mapped to their corresponding course levels and data was cleaned to ensure no duplication.

### Block 3 & 4

Converts the term to a numeric values, sorts the data and then sorts the terms by newest to oldest. White space is removed and the two data frames are merged together. 

### Block 5

This code uses the current criteria of the math placement model at MSU and codes students as either "Compliant" or "Uncompliant".

### Block 6 & 7

Counts the number os "Successful" and "Unsuccessful" students total and then at each course level.

### Block 8 & 9

Calculates statistical outcomes for the current model. Including an f-score, accuracy and specificity.


### Block 10-13

This code counts the number of "Successful" and "Unsuccessful" students that were compliant with the model. Then a success ratio was calculated at each course level and course number.

### Block 14

Populates descriptive statistics for each input variable. Including, high school GPA, ACT, SAT, Ed Ready Scores and course level.

### Logistic Regression

Here, the code runs a logistic regression for each course number and input variable, predicts student success at each course level, then outputs the results in a table for each course.

### Decision Tree

The decision tree model is ran for multiple input variables, with course level being the dependent variable. A summary of results is output for each course level and each model, as well as a visualization of the decision trees.

### Random Forest

A random forest model also uses course level as the dependent variable and multiple inputs. Here the code outputs a summary of results for each course level and an overall model outcome. 

### XG Boost

Lastly, XG Boost is ran for prediction of student placement into each course level and the same input variables are used as the other classification tree models. Again, the code outputs a summary of results at each course level and for each model. 

## Files Included

- math_placement.ipnb

This includes all of the python code described above.

- three_ps.txt

This file provides information on key developments as I was working on the capstone project.

- README.md

An explanation of the code and repository. 


