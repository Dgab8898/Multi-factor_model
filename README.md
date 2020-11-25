# **Multi-factor_model**

## **Project Description**

The Purpose of this project, to build a statistical risk model using PCA, and to use this model to build a portfolio along with 5 alpha factors.\
We ’ll create these factors, then evaluate them using factor-weighted returns, quantile analysis, sharpe ratio, and turnover analysis.\
At the end of the project, we ’ll optimize the portfolio using the risk model and factors using multiple optimization formulations.\
For the dataset, we'll be using the end of day from [Quotemedia](https://www.quotemedia.com) and sector data from[Sharadar](https://www.quandl.com/publishers/SHARADAR).


## **Installation**
```
import sys
!{sys.executable} -m pip install -r requirements.txt
! cat requirements.txt
!{sys.executable} -m pip install tensorflow --upgrade
!{sys.executable} -m pip install numpy==1.17.0
!{sys.executable} -m pip install alphalens==0.3.6 

```
## **Load Packages**
```
port cvxpy as cvx
import numpy as np
import pandas as pd
import time
import project_tests
import project_helper

import matplotlib.pyplot as plt
%matplotlib inline
plt.style.use('ggplot')
plt.rcParams['figure.figsize'] = (14, 8)
import os
import project_helper
from zipline.data import bundles
from sklearn.decomposition import PCA

```

## **Data process**
- We automate the process of dataflow using zipline environment to bundle our data and to  build pipline engine.\
- With the pipline engine built, we get the stocks at the end of the period in the universe, then we use these tickers to generate the returns data for the our risk model.\

Statistical Risk Model
we built the risk model using PCA,  and implemented the following risk factors:
- then we implement _factor_betas_ to get the factor betas from the PCA model.
- Implement _factor_returns_ to get the factor returns from the PCA 
- Implement _factor_cov_matrix_ to get the factor covariance matrix.
- Implement _factor_cov_matrix_ to get the factor covariance matrix.
- Implement idiosyncratic_var_matrix to get the idiosyncratic variance matrix.
- Implement idiosyncratic_var_vector to get the idiosyncratic variance Vector.\
 We explore the possibility the possibilities of using predict_portfolio_risk to predict portfolio risk.
 Then we thrown alpha into optimizer to caculate the ultimate portfolio weight by maximize our predictive return and simanltaneously trying to normalize,\
 attempting to neautralise the risk factor which are source of return variance.

**issues**


**Contributing**

For major changes, please open an issue. First discuss what you would like to change.
please make sure to update tests as appropriate

**Licence**
None



**Further reading**
- [investopedia](https://www.investopedia.com/terms/m/multifactor-model.asp)
- [udacity](https://udacity.com/nanodegrees/)
- [sciencedirect](https://www.sciencedirect.com/topics/social-sciences/factor-model)
- J.H. Stock, M.W. Watson, in Handbook of Macroeconomics, 2016
- Moorad Choudhry, in The Bond & Money Markets, 2001
- Morton Glantz, Robert Kissell, in Multi-Asset Risk Modeling, 2014



