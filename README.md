# Lab-4-Regression-Analysis-with-Regularization-Techniques
Lab 4: Regression Analysis with Regularization Techniques

Purpose:
This lab explores regression techniques and regularization methods using the Diabetes dataset. Models include Simple Linear Regression, Multiple Regression, Polynomial Regression, Ridge, and Lasso Regression. from the results below, we can see that regularization effectively controls model complexity. the results also shows that multiple regression leveraged all features for improved predictions. we have also learned taht increasing polynomial degrees can lead to diminishing returns or overfitting.

the following are the results of data analysis. 
Missing values: age       0
sex       0
bmi       0
bp        0
s1        0
s2        0
s3        0
s4        0
s5        0
s6        0
target    0
dtype: int64
                age           sex           bmi            bp            s1  \
count  4.420000e+02  4.420000e+02  4.420000e+02  4.420000e+02  4.420000e+02   
mean  -2.511817e-19  1.230790e-17 -2.245564e-16 -4.797570e-17 -1.381499e-17   
std    4.761905e-02  4.761905e-02  4.761905e-02  4.761905e-02  4.761905e-02   
min   -1.072256e-01 -4.464164e-02 -9.027530e-02 -1.123988e-01 -1.267807e-01   
25%   -3.729927e-02 -4.464164e-02 -3.422907e-02 -3.665608e-02 -3.424784e-02   
50%    5.383060e-03 -4.464164e-02 -7.283766e-03 -5.670422e-03 -4.320866e-03   
75%    3.807591e-02  5.068012e-02  3.124802e-02  3.564379e-02  2.835801e-02   
max    1.107267e-01  5.068012e-02  1.705552e-01  1.320436e-01  1.539137e-01   

                 s2            s3            s4            s5            s6  \
count  4.420000e+02  4.420000e+02  4.420000e+02  4.420000e+02  4.420000e+02   
mean   3.918434e-17 -5.777179e-18 -9.042540e-18  9.293722e-17  1.130318e-17   
std    4.761905e-02  4.761905e-02  4.761905e-02  4.761905e-02  4.761905e-02   
min   -1.156131e-01 -1.023071e-01 -7.639450e-02 -1.260971e-01 -1.377672e-01   
25%   -3.035840e-02 -3.511716e-02 -3.949338e-02 -3.324559e-02 -3.317903e-02   
50%   -3.819065e-03 -6.584468e-03 -2.592262e-03 -1.947171e-03 -1.077698e-03   
75%    2.984439e-02  2.931150e-02  3.430886e-02  3.243232e-02  2.791705e-02   
max    1.987880e-01  1.811791e-01  1.852344e-01  1.335973e-01  1.356118e-01   

           target  
count  442.000000  
mean   152.133484  
std     77.093005  
min     25.000000  
25%     87.000000  
50%    140.500000  
75%    211.500000  
max    346.000000  

Simple Linear Regression:
MAE: 52.25997644534553, MSE: 4061.8259284949268, RMSE: 63.73245584860925, R²: 0.23335039815872138

Multiple Regression:
MAE: 42.794094679599944, MSE: 2900.1936284934827, RMSE: 53.85344583676594, R²: 0.45260276297191926

Polynomial Regression:

MAE: 52.38391176015265, MSE: 4085.025480871632, RMSE: 63.91420406194254, R²: 0.2289715971205667
Key Results:

Best Model: Multiple Regression outperformed others with the highest R² (0.453) and lowest error metrics.

Regularization Effect: Ridge and Lasso regression helped mitigate overfitting but showed reduced performance with larger alpha values.

Polynomial Complexity: Polynomial regression offered no significant improvement, indicating overfitting risks.
Ridge Regression (alpha=0.1):
MAE: 52.27416510238435, MSE: 3969.193513439806, RMSE: 63.00153580223109, R²: 0.25083430942665674
Lasso Regression (alpha=0.1):
MAE: 52.26123410833456, MSE: 4017.0287468800143, RMSE: 63.38003429219658, R²: 0.2418056451469669
Ridge Regression (alpha=1.0):
MAE: 55.958916405864045, MSE: 4196.977562827367, RMSE: 64.78408417834868, R²: 0.20784119405367074
Lasso Regression (alpha=1.0):
MAE: 54.2844294922772, MSE: 4050.8402988914545, RMSE: 63.646211975980584, R²: 0.23542388154027005
Ridge Regression (alpha=10.0):
MAE: 62.62706771123811, MSE: 5104.0802201953, RMSE: 71.4428458293432, R²: 0.03663004336854614
Lasso Regression (alpha=10.0):
MAE: 64.00646146990485, MSE: 5361.533457238513, RMSE: 73.22249283682244, R²: -0.011962984778542296

Insights
we can learn that regularization effectively controls model complexity.

tehre were also multiple regression leverages all features for improved predictions.

Increasing polynomial degrees can lead to diminishing returns or overfitting.
