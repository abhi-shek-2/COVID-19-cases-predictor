# COVID-19-cases-predictor
It will predict number of covid cases using data analysis model based on Pandas library of Python



                                                                    DATA
The date used for prediction should be up-to-dated so to get readily available data each time prediction is made, it is brought from an API in Json format using requests API of python.

                                                                         PREPROCESSING
1. After extracting data to avoid any failure in future this data is stored in form of excel file using pandas converting to Dataframe format of file itself.
2. Data is processed to with some new column know as day number extracted from the date it is been started

                                                                           ANALYSIS
Before moving any further working and to find a perfect model a study over data is conducted where, for any input country a pie chart depicting the ratio of recovery death and present is created with a plot of increasing cases in every day to construct a study over the day number to cases increased

                                                                            MODEL 
After the analysis is completely studied it is found that the best fit model based on trend fashion, Polynomial model could help to predict a close outcome, it is itself a Linear regressor where the number of features used to predicted is polynomially constructed from day number, transforming the input equation from 
y = b0 + b1x + e -----> y = b0 +b1x +b2x2 + b3x3.......
where b0,b1,b2 are the coeffients that are fitted by model for best prediction, over test set.

                                                                          CONCLUSION
Model used : Linear Regression
Feature Engineered : PolynomialFeature
Testing : rms ,r2_score
wherer RMS provides the mean error from the prediction to the true value and r2 score for the percentage score of error to provide a better conclusion the final testing report is created through visualization
