# Parameter Optimization of SVM
Assignment for UCS654

## About SVM and Parameter Optimization

Support Vector Machine or SVM is one of the most popular Supervised Learning algorithms, which is used for Classification as well as Regression problems. However, primarily, it is used for Classification problems in Machine Learning.

Some of the most important parameters of SVM such as kernel, C, and gamma can be changed in order to achieve a higher accuracy. This is called as Hyperparameter Tuning. 

We can perform this task using GridSearchCV for optimizing these parameters.

In this python file, I've used a Fitness Function to optimize the parameters.

## Dataset

The dataset for the project has been downloaded from the UCI Machine Learning Repository.
https://archive.ics.uci.edu/ml/datasets/Bias+correction+of+numerical+prediction+model+temperature+forecast

This data is for the purpose of bias correction of next-day maximum and minimum air temperatures forecast of the LDAPS model operated by the Korea Meteorological Administration over Seoul, South Korea. This data consists of summer data from 2013 to 2017. The input data is largely composed of the LDAPS model's next-day forecast data, in-situ maximum and minimum temperatures of present-day, and geographic auxiliary variables. There are two outputs (i.e. next-day maximum and minimum air temperatures) in this data. Hindcast validation was conducted for the period from 2015 to 2017.

Number of Instances: 7588

Number of Attributes: 27

## Final Result Table

| Sample  | Best Accuracy | Best Kernel | Best Nu | Best Epsilon |
| -----   | ------------- | ----------- | ------- | ------------ |
| 1 | 0.94 | Linear | 5.92 | 7.25 |
| 2 | 0.86 | Linear | 0.10 | 8.04 |
| 3 | 0.94 | Poly   | 3.28 | 7.72 |
| 4 | 0.71 | Poly   | 1.33 | 1.95 |
| 5 | 0.74 | Linear | 3.98 | 3.50 |
| 6 | 0.77 | Linear | 5.75 | 5.54 |
| 7 | 0.77 | Poly   | 7.22 | 6.70 |
| 8 | 0.77 | Poly   | 7.71 | 6.16 |
| 9 | 0.74 | Poly   | 6.85 | 2.69 |
| 10| 0.61 | Poly   | 3.40 | 9.43 |

## Convergence Graph
![graphh](https://user-images.githubusercontent.com/98264294/233139100-e95e07b3-5097-4c0c-af14-ee58fa69e7c9.png)

## Discussion
From the above graph, we can conclude that the model is well trained and parameter have been optimized due to the less gap between training and cross-validation curve.

The graph is made for the sample which has best accuracy. Sample 1 has the best accuracy of 0.94 having kernel = Linear, Nu = 5.92 and Epsilon = 7.25.

## Written By
Name : Parv Gupta
  
Roll No. : 102017186

Sub-Group: 3CS8
