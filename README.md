# Haiti Earthquake Relief Effort: Fidning Blue Tarps

>This project was completed for the Statistical Learning course (DS 6030) in the University of Virginia's Masters of Science in Data Science Program.

Analyzing data from Haiti Earthquake Relief Effort from 2010.

Goal: use various classification methods (logistic regression, LDA, QDA, KNN, Support Vector Machine, and Random Forest) to correctly identify pixels labeled as Blue Tarps.
    + Blue tarps were used as makeshift shelters following the destruction from the 2010 Haiti earthquake.

Software: R and R Studio

Size of data set:

+ 63,241 observations (train/test data with 80/20 split)
+ 2,008,623 observations (hold-out data)
+ 4 variables:
    + Red, Green, Blue (RGB) color scale: range from 0 to 250
+ Classes: Blue Tarp, Rooftop, Soil, Various Non-Tarp, and Vegetation
    + Focused on Blue Tarps vs all others for modeling

According to Wikipedia, the RGB color model is additive. Therefore, the models used throughout the analysis utilized additive models without transformations or interaction effects.

# Results: Best Performing Model

The best performing model based on both the original and hold-out data sets was Logistic Regression. Overall, logistic regression had the best performance metrics on the hold-out data for all four metrics where:

+ Accuracy = 99.03%
+ AUC = 0.9994
+ TPR = 98.76%
+ FPR = 0.96%

See the powerpoint file and R files for full data pipeline and other findings. 
