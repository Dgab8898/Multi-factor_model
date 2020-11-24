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
```


**issues**


**Contributing**

For major changes, please open an issue. First discuss what you would like to change.
please make sure to update tests as appropriate

**Licence**
None



**Further reading**
- [investopedia](https://www.investopedia.com/terms/m/multifactor-model.asp)
- [udacity](https://classroom.udacity.com/nanodegrees/nd880/PCA as a Factor Model - Coding Exercises)
- [sciencedirect](https://www.sciencedirect.com/topics/social-sciences/factor-model)
- J.H. Stock, M.W. Watson, in Handbook of Macroeconomics, 2016
- Moorad Choudhry, in The Bond & Money Markets, 2001
- Morton Glantz, Robert Kissell, in Multi-Asset Risk Modeling, 2014



