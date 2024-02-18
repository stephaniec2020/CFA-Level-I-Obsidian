- # 7 - Introduction to Linear Regression
202210031115
Status: #📥 
Tags: [[CFA Level I]]

## Objectives:
- [x] describe a simple linear regression model and the roles of the dependent and independent variables in the model.
- [x] describe the least squares criterion, how it is used to estimate regression coefficients, and their interpretation.
- [x] explain the assumptions underlying the simple linear regression model, and describe how residuals and residual plots indicate if these assumptions may have been violated.
- [x] calculate and interpret the coefficient of determination and the F-statistic in a simple linear regression.
- [x] describe the use of analysis of variance (ANOVA) in regression analysis, interpret ANOVA results, and calculate and interpret the standard error of estimate in a simple linear regression.
- [ ] formulate a null and an alternative hypothesis about a population value of a regression coefficient, and determine whether the null hypothesis is rejected at a given level of significance.
- [ ] calculate and interpret the predicted value for the dependent variable, and a prediction interval for it, given an estimated linear regression model and a value for the independent variable.
- [ ] describe different functional forms of simple linear regressions.

## Review:
- [ ] describe the use of analysis of variance (ANOVA) in regression analysis
- [ ] interpret ANOVA results, and calculate and interpret the standard error of estimate in a simple linear regression
- [ ] describe the least squares criterion, how it is used to estimate regression coefficients, and their interpretation.
- [ ] explain the assumptions underlying the simple linear regression model, and describe how residuals and residual plots indicate if these assumptions may have been violated.
- [ ] describe different functional forms of simple linear regressions
- [ ] Goodness of Fit and Hypothesis Tests
- [ ] Coefficient of determination


---

## Simple Linear Regression
### Independent vs dependent variable
**Dependent variable (Y)** - variable you are trying to predict or explain, aka endogenous variable, predicted variable
**Independent variable (X)** - variable you are using to explain the variation in Y

If there is only one independent variable against the dependent variable, it can be termed as **simple linear regression**, and two variables share a simple linear relationship, which is described by the regression model:

$$Y_i = b_0+b_1X_i+\epsilon_i$$
where $b_0$: y-intercept; $b_1$: slope coefficient; $\epsilon_i$: **error** term (also known as **residual** term)

#### There are certain assumptions when constructing the simple linear regression: (details in below section)
- relationship between the dependent and independent variable is linear
- independent variable is uncorrelated with error term ($\epsilon_i$) (i.e. there are no noticeable trend of  $\epsilon_i$ ↑ as $X$↑ )
- E($\epsilon_i$) = 0 (i.e. expected value of error term is 0)
- Var($\epsilon_i$) = constant (i.e. the variance of error term is constant, homoskedasticity)
- $\epsilon_i$ is independently distributed (i.e. $\epsilon_i$ is not correlated to $\epsilon_{i+1}$ nor $\epsilon_{i-1}$)
- $\epsilon_i$ is normally distributed

### Estimated Line of best fit
The straight line that minimises the sum of squared errors is the line of best fit for a simple linear regression.

#### Sum of Squared Errors (SSE)
Criteria: $min(\sum\epsilon_i^2)$, it is also known as least squares method or $min(SSE)$, with the degrees of freedom (d.f.) at $n-1$;
where the sum of the error values with predicted Y values with actual Y values are minimised

The equation of **line of best fit**:
$$\hat{Y_i}=\hat{b_0}+\hat{b_1}X_i$$
where $\hat{Y_i}$ denotes estimate of $Y_i$; $\hat{b_0}$: constant term/intercept; $\hat{b_1}$: slope.

The **slope coefficient** formula is as follows:
$$\hat{b_1} = \frac{Cov_{xy}}{\sigma^2{_x}}$$
where $\hat{b_1}$: slope of the line; $cov$: covariance of x and y; $\sigma^2_{x}$: variance of x

and the **intercept $b_0$** can be estimated with this formula:
$$\hat{b_0} = \bar{Y} - \hat{b_1}\bar{X}$$
where $\hat{b_0}$: y-intercept; $\bar{Y}$: mean of Y; $\bar{X}$: mean of X, and it is the estimate of Y when X=0.

### Sample calculation table for covariance and variance 
![[Screenshot 2022-10-03 at 11.53.30.png]]

### Underlying assumptions of the simple linear regression model
There are several underlying assumptions of the simple linear regression model:
- **Linearity** - linear relationship between the independent and dependent variables (i.e. most of the residuals should be close to 0; it is impossible to fit a straight line without most residuals deviating from 0)
- **Homoskedasticity** -  Var($\epsilon_i$) = constant (i.e. the variance of error term is constant), no matter where you split the data, they should all be equal in variance in error/residual; as ***heteroskedasticity*** is the condition where the variances of residuals are not equal across observations and it creates significant problems for statistical inference.
- **Independence** - Residual $\epsilon_i$ for one observation is not correlated with that of another observation; a violation of it would be from **autocorrelation** such as seasonal sales
- **Normality** - Residuals $\epsilon_i$ are normally distributed, when the sample size is large, we can assume it's normal through CLT; (only the residuals have to be normally distributed and not the dependent/independent variable); the normality is essential for hypothesis testing

## Measures of goodness-of-fit
**Goodness-of-fit** is a statistical technique used to determine whether an observed data set follows a specific theoretical distribution.

**Goodness-of-fit**:
- quantify the level of confidence of the linear regression model
- to answer the question of "how well does the regression model fit the observed data?"
- Through 3 methods which will be discussed in detail in later part of this section:
	- $R^2$ (Coefficient of determination)
	- Standard error of estimate (SEE)
	- F-statistics 

### ANOVA table (Analysis of Variance) 
To construct the variance of table:
- analyse variability of the model to the observed data
- analyse the fitting of the regression model to the observed data

There are several sources of variations:
- **unexplained** -  sum of squared errors(SSE)
- **explained** - regression sum of squares (RSS)
- **total variation** - total sum of square (SST)

### Total sum of squares (SST)
The **total sum of squares (SST)** is the squared differences between the observed **_dependent variable_** and its **mean**, it can be think of the **total variation**.

The **total sum of squares (SST)** equation is as follows:
$$SST =\sum(Y_i-\bar{Y})^2$$
and **total sum of squares (SST)** can also be calculated by **variance**:
$$SST = \sigma^2 \times (n-1)$$
where $\sigma^2$: variance; $n$: number of samples collected; where variance is square of standard deviation (i.e. $\sigma$ = standard deviation).

### Regression Sum of Squares (RSS)
The **regression Sum of Squares (RSS)** is the sum of the **explained variation**.  It is the sum of the differences between the _predicted_ value and the **mean** of the _dependent variable_.

The **regression Sum of Squares (RSS)** equation is as follows:
$$RSS = \sum(\hat{Y_i}-\bar{Y})^2$$

### Sum of Squared Errors (SSE)
The **sum of squared errors (SSE)**, the error is the difference between the _observed_ value and the _predicted_ value, which is the **unexplained variation**.

The **sum of squared errors (SSE)** is also known as the sum of the unexplained variation:
$$SSE = \sum({Y_i}-\hat{Y_i})^2$$

### Demonstration of relationships of SST, RSS, and SSE
![[Screenshot 2022-10-03 at 12.47.27.png]]

Formula for **total variation or sum of square total (SST)**:
$$SST = RSS+SSE$$
where the SST: total sum of squares; RSS: regression sum of squares; SSE: sum of squared errors, therefore the total variation is the sum of explained and unexplained variation.

![[Screenshot 2022-10-03 at 12.58.24.png]]

Through 3 methods which will be discussed in detail in later part of this section:
- $R^2$ (Coefficient of determination)
- Standard error of estimate (SEE)
- Confidence interval of forecast  F-statistics 

### 1. Standard Error of Estimate (SEE)
**Standard Error of Estimate (SEE)** is a measure of the variation or dispersion of the observed values around the regression line in a linear regression model.

Don't confuse standard error of estimate (SEE) with sum of squared errors (SSE), where SEE: standard error of estimate, and the other, SSE: sum of squared errors.

**SEE is the standard deviations of the error term only ($\epsilon_i$)**, and the equation is as follow:
$$SEE = \sqrt{MSE} = \sqrt{\frac{SSE}{n-2}}$$
where SEE: Standard error of estimate; MSE: mean squared error; SSE: squared sum of errors.

### 2. Coefficient of determination ($R^2$)
**Coefficient of determination ($R^2$)** determines the percentage of simple regression model explains the observed data

The equation of coefficient of determination is the **explained variation (RSS)** over **total variation (SST)**, which is as follows:
$$R^2 =  \frac{RSS}{SST}$$
where $R^2$: coefficient of determination; RSS: regression sum of squares; SST: sum of squares total.

The coefficient of determination for a linear regression describes the percentage of the variation in the dependent variable explained by the variation of the independent variable.

The **correlation coefficient** (r), which is the square root of the coefficient of determination for a simple regression:
$$\mathrm{Correlation\,coefficient}\,(r)= \sqrt{R_2}$$

### How to understand whether the regression model is a good fit to observed data?
- The explained variation would be larger in proportion in the total variation.
- Sum of squared error (unexplained portion) ↓, therefore the standard error of estimate (SEE) is low
- The $R^2$ is high, because of the proportion of explained variation (RSS) is high.
- Therefore, the observed data are close to the regression line, which is a good fit.

### 3. Confidence interval of forecast
#### Point estimate
Recall the formula for the **point estimate equation** is as follow:
$$\mathrm{Point\, estimate \pm CV_{\alpha/2} \times Std.\,error}$$
where $CV_{\alpha/2}$: critical value; $\alpha$: significance level.

#### Confidence interval of forecast
In the **confidence interval of forecast**, the point estimate formula is adapted:
$$\hat{Y} \pm t_\frac{\alpha}{2} \times s_f$$
where $CV_{\alpha/2}$: critical value; $\alpha$: significance level, and $CV_{\alpha/2}$ should use **t-test (i.e. $t_{\alpha/2}$) and (d.f. = n-2)** and  $S_f$ is the standard error of the forecast, which includes the standard error of estimate in $b_1$ (i.e. slope coefficient) and $b_0$ (i.e. y-intercept).

For the **confidence interval of forecast**:
- use t-statistics
- degree of freedom (d.f): $n$-2 from the ANOVA table
- std. error of forecast ($S_f$) includes the estimates of $b_0$ and $b_1$ (i.e. the intercept and slope coefficient)

There is no need to memorise the formula, but this is the formula for $S_f$:
$$S_f{^2} = SEE^2[1+\frac{1}{n}+\frac{(X-\bar{X})^2}{(n-1)s_x{^2}}]$$

#### Example of how to calculate confidence interval of forecast
![[Screenshot 2022-10-03 at 13.41.28.png]]

## Hypothesis tests on slope coefficient
There are **several ways to test the slope coefficient**:
- Confidence interval
- t-test approach
- p-value approach
- f-test approach

### Confidence interval on slope coefficient hypothesis test
If you suspect there's a significant relationship between X and Y on regression model:
Null hypothesis ($H_0$): $b_1 = 0$
Alternative hypothesis ($H_A$): $b_1 \ne 0$

**Confidence Interval (C.I.)** approach equation for **testing slope coefficient**:
$$\hat{b_1} \pm t_\frac{\alpha}{2} \times s_{\hat{b_1}}$$
where $\hat{b_1}$: slope estimate; $s_\hat{b_1}$: standard error of coefficient, and the degrees of freedom (d.f.): $n-2$; where stronger regression will have ↓SEE, ↓$s_\hat{b_1}$ and C.I. ↓

where the hypothesised value falls within the C.I. ⇒ fail to reject $H_0$
where the hypothesised value falls outside of C.I. ⇒ reject $H_0$

### t-test approach on slope coefficient hypothesis test
The **t-test** approach equation for **testing slope coefficient**:
$$t_{b_1} = \frac{\hat{b_1} - b_1}{s_\hat{b_1}}$$
where $\hat{b_1}$: estimated value of $b_1$; $b_1$: hypothesised value; $s_{b_1}$: std. err of coefficient
where $b_1$ = 0 if it's unprovided with; and it is a two-tailed test.

### p-value approach on slope coefficient hypothesis test
After the t-test, some instead of rejecting the $H_0$, it may decided to just report the 
probability value (p-value), so it is up to the reader to determine whether to reject the $H_0$.

In the p-value approach:
- smallest level of significance which $H_0$ can be rejected
- which is the inverted of t-table, using the value to estimate the p-value

### F-test approach on slope coefficient hypothesis test
The F-test approach on slope coefficient hypothesis test (require the ANOVA table):
- mean of RSS (regression sum of square) (i.e. explained) ⇒ MSR (mean squared regression)
- mean of SSE (sum of squared errors) (i.e. unexplained)⇒ MSE (mean squared error)

$$F=\frac{MSR}{MSE}=\frac{(\frac{RSS}{1})}{(\frac{SSE}{n-2})}$$
where MSR: mean squared regression; MSE: mean square error, d.f. of MSR = $1$ and d.f. of MSE = $n$-2.
therefore high F ⇒ $b_1 \ne 0$, and the model is a good fit.

![[Screenshot 2022-10-03 at 15.49.31.png]]

It will be helpful in the exam to formulate a table like this to solve this type of question:

|Source of Variation | d.f. | Sum of Sq. | Mean Sum of Squares|
|---|---|---|---|
| Unexplained (SSE) |	$n-2$	| $std. dev. \times n$ |	SSE / (n-2)
| Explained (RSS) |	1	| given or calculate through $SST - SSE$ | same as RSS |

## Functional forms for simple linear regression
There are several functional forms for simple linear regression:
- Time series regression
- Log-lin model
- Lin-log model
- Log-log model

## Time series regression
In time series regression:
- **Dependent variable (Y)** - things that you would like to predict
- **Independent variable (X)** - time

$$Y_t = b_0+b_1t+\epsilon_t$$
where $t=1,2,...T$ in fixed-time periods

### Least squares method
**Least squares method** used to estimate the line of best fit
- $min(\sum{\epsilon_t{^2}})$: The least squares criterion defines the best-fitting linear relationship as the one that minimises the sum of squared errors, the squared vertical distances between the predicted and actual values of the dependent variable.
- all of the linear regression would work in time series regression as well

$$\hat{Y_t} = \hat{b_0}+\hat{b_1}t$$
where $(t=1,2,...,T)$

![[Screenshot 2022-10-03 at 15.50.35.png]]

The **slope coefficient** formula:
$$\hat{b_1} = \frac{Cov_{ty}}{\sigma^2{_t}}$$
where $cov$: covariance of x and y; $\sigma^2_{x}$: variance of x
- Y is the dependent variable and X is the independent variable.  
- The estimated slope coefficient is interpreted as the change in the _dependent_ variable, given a one-unit change in the _independent_ variable. 
- The predicted value of the dependent variable must consider the estimated intercept term along with the estimated slope coefficient.

and the **intercept $b_0$** can be estimated with this formula:

$$\hat{b_0} = \bar{Y} - \hat{b_1}t$$
it is the estimate of Y when t=0.

### Limitations of linear regression model
- cannot model all kinds of relationship
- financial time series data often exhibit exponential relationships (e.g. growth/interest compounding)

## Log-lin model
**Log-lin model** is used when:
- when the data points, dependent (what you expect/predict) variable vs independent variable share a logarithmic relationship
- where the dependent variable (Y) increases at a faster rate over then independent variable (X or t, depending on the context)
$$\hat{Y_t} = e^{\hat{b_0}+\hat{b_1}t}$$
- We can apply ln() to convert the logarithmic relationship to linear and apply the linear model to the equation and allow the usage of linear regression technique:
$$ln(\hat{Y_t}) = \hat{b_0}+\hat{b_1}t$$
and this is the **log-linear trend model**.

![[Screenshot 2022-10-04 at 16.17.52.png]]

The slope, $b_1$, is the relative change in Y for an absolute change in X.
A regression of the form $ln(Y) = b_0 + b_1X$ is appropriate when the relative change in the dependent variable is a linear function of the independent variable.

## Lin-log model
**Lin-log model** is used when:
- the dependent variable increases at a slower rate over the independent variable
- where the dependent variable (Y) is linear, and the independent variable is ln(X)
- therefore, the overall formula would be:

$$Y_i = b_0+b_1lnX_i$$

The slope, $b_1$, is the absolute change in Y for a relative change in X.

![[Screenshot 2022-10-04 at 16.18.12.png]]

## Log-log model
Sometimes, the data might appear to be random, however, if we apply log to both Y and X, sometimes, there might be an linear relationship.

$$ln(Y_i)=b_0+b_1lnX_i$$

The slope, $b_1$, is the relative change in Y for a relative change in X.

![[Screenshot 2023-06-23 at 17.58.49.png]]
![[Screenshot 2023-06-23 at 18.12.35.png]]
![[Screenshot 2023-06-23 at 18.16.24.png]]

---
## Questions before starting this section:
- [ ] When to model through linear regression?
- [ ] How to do more than two parameters modelling?
- [ ] How to model a with different types of data?


## Codes to test understanding of objectives




