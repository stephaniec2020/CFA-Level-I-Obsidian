# 2 - Organising, visualising and describing data
202209090128
Status: #📥 
Tags: [[CFA Level I]]

## Objectives:
- [x] Identify and compare data types.
- [x] Describe how data are organised for quantitative analysis.
- [x] Interpret frequency and related distributions.
- [x] Interpret a contingency table.
- [x] Describe ways that data may be visualised and evaluate uses of specific visualisations.
- [x] Describe how to select among visualisation types.
- [x] Calculate and interpret measures of central tendency.
- [x] Evaluate alternative definitions of mean to address an investment problem.
- [x] Calculate quantiles and interpret related visualisations.
- [x] Calculate and interpret measures of dispersion.
- [x] Calculate and interpret target downside deviation.
- [x] Interpret skewness.
- [x] Interpret kurtosis.
- [x] Interpret correlation between two variables.

## Review:
- [x] Geometric, harmonic, and arithmetic mean
- [x] Calculation of coefficient of variance (reminder: it is the opposite of Sharpe ratio)
- [ ] Calculation of target downside deviation
- [ ] Interpret skewness and kurtosis
- [ ] Calculation of covariance and correlation
- [ ] Study different charts: frequency polygon, histogram,  bubble line chart, scatter plots
- [ ] Memorise the equation of mean absolute deviation (MAD) 
- [ ] Know how to calculate deciles

---

## Codes to test understanding of objectives
1. Dollar-cost averaging technique (Harmonic mean)

$$\bar{X} = \frac{N}{\sum\limits_{i=1}^n\frac{1}{X_i}}$$
Understand the reason of why the dollar-cost averaging is below the arithmetic mean; need to find out the reason of when does it fail

2. Find out the past performance of the compound annual rate return of a certain stock (Geometric mean)/ of SPX for the past return (daily, starting from the date of my birth)
$$1+R_{G}= \sqrt[n]{(1+R_1) \times (1+R_2) \times ... \times (1+R_n)}$$

3. Past performance of a stock (geometric mean) vs. expected future performance of a stock (arithmetic mean)
4. Find the Sharpe ratio of each instrument/tool (cash, bonds, stocks)
	https://medium.datadriveninvestor.com/the-sharpe-ratio-with-python-from-scratch-fbb1d5e490b9


## Data types

There are 6 different broad categories of data:
- Numerical vs categorical
- Time series vs cross-sectional
- Structured vs unstructured

### Numerical data
- or **quantitative data**, are values that can be measured
- can be discrete or continuous
	- discrete: countable
	- continuous: can have decimal places/any fractional values

#### Categorical data:
- or **qualitative data** are consist of labels and distributed within groups
- categorical data can be nominal and ordinal
	- nominal: cannot be placed in orders (eg. industry types: commercial, manufacturing, sales; or bond types: international, government)
	- ordinal: can be placed in logical order (top-1000 performing stocks, as it can be ranked (i.e. buy, hold, sell))

#### Time-series data:
- set of observation taken periodical and most often at equal intervals over time
- eg. daily closing price of a stock, earnings per share of a company

#### Cross-sectional data:
- refers to a set of comparable observation all taken at a specific time point in time
- eg. today's closing price of all 30 stocks in Dow Jones
- time series and cross-sectional data are also known as panel data, which can be put into tables 

### Structured data
- time-series, cross-sectional data, and panel data are structured data
- *market data*
- *analytical data*
- *fundamental data*
- structured data often are presented as one-dimensional array, or two-dimensional array (data table)

### Unstructured data
- which can not be in a certain structure 
- eg. financial analyst commentary, company's CEO commentary on financial statements, post of social media -> investor sentiment, business sentiment
- *generated by sensors*, eg. traffic cameras -> business activity
- unstructured data have to be transformed into structured data

### Frequency table/ distribution
#### Generating frequency table notes:
1. Define the intervals
	- must have a lower and upper limit
	- intervals must be mutually exclusive
	- number of intervals must be considered properly - not too many that does not provide constructive information, and not too little that it does not capture the difference between intervals
2. Tally the observations.
3. Count the observations. (Absolute frequency)

Other important concepts:
- absolute frequency
- relative frequency
- cumulative absolute/relative frequency

## Contingency table
- two-dimensional array which can analyse two variables at the same time
- important for chi-square table
- joint frequency: observed frequency of two attributes
- marginal frequency: total frequencies of a row or column 
- confusion matrix: 2-by-2 matrix -< evaluate performance of a classification model (false positive and false negative)


## Visualising data
#### Types of graphs and table to present structured data
- histogram
- frequency polygon
- cumulative frequency distribution chart
- bar chart
- grouped bar chart (women and men)
- clustered bar chart 
- stacked bar chart (women and men in total)
- tree map (visualising the relative sizes of categories, reflect frequency)
- word cloud (analysing text, continue uses of specific words in text data, the higher the frequency, the larger the text)
- line chart (eg illustrating time-series data)
- bubble line chart (eg. revenue per salesperson, add another dimension)
- scatter plot (eg. identify the relationship between 2 variables, continuous data) (identify linear and non-linear relationship) (linear regression)
- scatter plot matrix (analyse relationship between 3 or more variables)
- heat map (colour and shape indicate frequency, more appropriate for discrete categories)


## Flow chart for selecting the right visualisation tool 
![[Screenshot 2022-09-10 at 20.45.45.png]]

## Measure of central tendency
**Measure of central tendency** identifies the centre, or average of a dataset. This central point can then be used to represent the typical, or expected value in the data set.

There are several ways of identifying the centre of the dataset, choose accordingly depending on the usage:
- mean
- mode
- median
- harmonic mean - 
- geometric mean
- quantiles

## Mean
### Population mean
- population: parameter - measure used to describe a characteristic of the population
- all the observed values in the population in the group of interest 

$$\mu = \frac{\sum\limits_{i = 1}^n X_{i}}{N}$$


### Sample mean
- subset of a population 
- sum of all the values in a sample of a population
- it is used to make *inferences* about population mean
$$\bar{X} = \frac{\sum\limits_{i = 1}^n X_{i}}{n}$$

**Arithmetic means**  - sum of the observations / number of observations
few characteristics and assumptions were made for the arithmetic mean:
- all interval and ratio data sets have an arithmetic mean
- all data values are considered and included in the arithmetic mean computation
- a data set has only one arithmetic mean (i.e. the arithmetic mean is unique)
- the sum of the deviations of each observations in the data set from the mean is always zero
- all of the values hold equal weight
- <font color="purple">estimate the next observation, expected value of a distribution</font>


The **sum of mean deviations** equation is as follows:  $${\sum\limits_{i = 1}^n (X_{i}-}{\bar{X}}) = 0$$

Other ways to calculate the mean to overcome certain outliers of the data set:
- **Trimmed mean** - exclude a stated percentage (%) of the most extreme observation  (eg. 1% trimmed mean ⇒ exclude 0.5% of the highest observation and the lowest 0.5% of observation); **estimate the mean without the effects of a given percentage of outliers**

- **Winsorised mean** - substitute the highest and lowest value with the desired percentile's value, eg. to calculate 90% winsorised mean ⇒ 5th and 95th percentile of the whole data set, substitute the value above 95th percentile and lower than 5th percentile and calculate the mean of the revised data and **decrease the effect of outliers on the mean**

**Weighted mean**
- Weighted mean takes into account of each observation carry a disproportionate influence to the mean 
-  <font color="purple">It is useful for calculating portfolio returns in a single cross-sectional data (snapshot of a certain timeframe)</font>

The equation of weighted mean is as follows:
$$\bar{X}_w = \sum\limits_{i = 1}^n{w_iX_i} = (w_1X_1+w_2X_2+...+w_nX_n)$$
where $X_{1}$,$X_{2}$,...,$X_{n}$: observed values;
 $w_{1}$,$w_{2}$,...,$w_{n}$: corresponding weights associated with each of the observed value so that the Σ$w_{i}$ = 1.

**Geometric means** 
- <font color="purple">Compound rate of returns over multiple periods</font>
- it is used when calculating investment returns over multiple periods or when measuring compound growth rates

Geometric mean (G) = 
$$G = \sqrt[n]{(X_1 \times X_2 \times ... \times X_n)}$$
where 

**Note**: it can only be calculated if the products are non-negative

Geometric mean of return/growth, $R_{G}$

$$1+R_{G} = \sqrt[n]{[(1+R_{1})\times(1+R_{2})\times...\times(1+R_{n})]}$$

or you can present it as 
$$1+R_{G} = {[(1+R_{1})\times(1+R_{2})\times...\times(1+R_{n})]}^\frac{1}{n}$$
where $R_{G}$: rate period geometric mean of return/growth; $R_{t}$: the return period of $t$; n: is the number of period
**Note**: for $\sqrt[3]{(1+R_1)(1+R_2)(1+R_3)}$  input this $y^x$ $\frac{1}{3}$ in the calculator

> Example
> For the last three years, the returns for Acme Corporation common stock have been -9.34%, 23.45%, and 8.92%. Compute the compound annual rate of return over the three-year period.
> 
> Answer: 
> $$1+R_{G} = \sqrt[3]{(1-0.0934) \times (1+0.2345) \times (1+0.0892)}$$
> $$1+R_{G} = \sqrt[3]{1.21903}$$
> $$R_{G} = 1.06825 - 1 = 6.825\%$$
> The compound annual rate of growth is 6.825% **(time-weight rate of return)**

**Note**: geometric mean is always less than or equal to arithmetic mean, and the difference increases as the dispersion of the observation increases.
The only time of the arithmetic and geometric means are equal is when there is no variability in the observations (ie all observations are equal)

### Geometric mean vs arithmetic mean for returns calculation
> **Geometric mean vs arithmetic mean for returns calculation**
>
> Which is the better estimator of future performance?
> In a scenario of an investor placing $1000 in a stock and the 1st year of return is 100% and the 2nd year of return is -50%. The account final value is $1000.
> By using the geometric mean:
> $$1+R_{G}=[(1+1)\times(1-0.5)]^\frac{1}{2}$$
$$R_{G}= 1-1=0\%$$
> So the past performance is 0%, which is correct because the final value is $1000.
>
> However, if you calculate by using the arithmetic mean for past performance, you'll get 25% because 
> $$\frac{(100+50)}{2} = 25\%$$ which is wrong. 
> 
> It is illustrated in the diagram below:
![[Screenshot 2022-09-11 at 15.54.00.png]]

**However, if you want to calculate the future performance, arithmetic mean would be more suitable**

Arithmetic mean is the better estimator of future returns, although it may not be the mathematically correct calculation of the past returns.

![[Screenshot 2022-09-11 at 15.57.20.png]]

![[Screenshot 2022-09-11 at 15.57.48.png]]

**Harmonic means**
- dollar cost-averaging technique (mathematical base of why dollar-cost averaging is beneficial)
- average cost of shares purchased over time
- <font color="purple">to calculate the average share cost from periodic purchases in a <b>fixed dollar amount</b></font>

Equation:
Average cost per share = 
$$\bar{X}=\frac{N}{\sum\limits_{i=1}^n\frac{1}{X_i}}$$
where average of X: average cost per share; N: number of times buying into the share; Xi: price of the share when acquired

> Example
> An investor purchases $1,000 of mutual fund shares each month, and over the last three months, the prices paid per share were $8, $9, and $10. a) What is the number of units acquired. b) What is the average cost per share?
> 
> Answer:
> a) Number of units acquired: $$\frac{1000}{8}+\frac{1000}{9}+\frac{1000}{10} = 336.1$$
> b) The average price per share is:
>  Total amount paid/ number of units acquired: 
>  $$\frac{3(1000)}{336.1} = \$8.926$$
> The other shortcut to comes to the same answer is through **harmonic mean**
> $$\frac{3}{\frac{1}{8}+\frac{1}{9}+\frac{1}{10}} = \$8.926$$
> Also, the value $8.926 is slightly lower than the arithmetic mean $9; that is the mathematical basis of dollar-cost averaging

**Note**: For all values that are not equal, the harmonic mean < geometric mean < arithmetic mean. This mathematical fact is the basis for the claimed benefit of purchasing the same dollar amount of mutual fund shares each month/each week.

## Mode
- mode is the most frequently observed value in the dataset 
- it is not useful in small and values missing in dataset 
- it is best used in a large sample size and to quickly identify the most prevalent value

Unimodal - 1 mode within the dataset
Bimodal - 2 modes within the dataset
Trimodal - 3 modes within the dataset

## Median
- is the midpoint of a dataset when arranged in ascending or descending order
- median is important as the arithmetic mean is affected by the highest observation and lowest observation (outliers)
- it is a better measure of central tendency with cases that have outliers

## Quantiles
Median - the distribution is divided into 2
Quartile - the distribution is divided into 4
Quintile - the distribution is divided into 5
Decile - the distribution is divided into 10
Percentile - the distribution is divided into 100(%)
interquartile range - Q2 to Q3 (2nd quartile to 3rd quartile/ 25th percentile to 75th percentile)

$$L_{y} = (n+1) \times (\frac{y}{100})$$ where $L_{y}$ : location of data points that sits at the boundary of the quantile; n: number of observations; y: percentile

>What is the third quartile for the following distribution of returns?
>
> 8%, 10%, 12%, 13%, 15%, 17%, 17%, 18%, 19%, 23%
> 
>Answer:
> The third quartile is the point below which 75% of the observations lie. Recognising that there are 10 observations in the data set, the third quartile can be identified as:
> $$L_{75} = (10+1) \times (\frac{75}{100}) = 8.25$$
> When the data are arranged in ascending order, the third quartile is a fourth (0.25) of the way from the eighth data point (18%) to the ninth data point (19%), 
> $$18 + (19-18)\times0.25 = 18.25\%$$
> or 18.25%. 
> 
> This means that 75% of all observations lie below 18.25%.

## Box-and-whisker plot

![[Screenshot 2022-09-11 at 16.18.05.png]]

## Measure of dispersion
Low variability ⇒ less risk 
High variability ⇒ high risk

#### Range and Mean Absolute Deviation
- mean absolute deviation (MAD) can describe the distribution better compare to the mean than the range
$$\mathrm{Mean\,Absolute\,Deviation} = \frac{\sum|X-\bar{X}|}{N}$$

#### Population Variance & standard deviation
- population has to include every member of the population; what if we don't have the whole population's data or the population is too big??

**Population variance** =
 $$\sigma^2 = \frac{\sum(X-\mu)^2}{N}$$

**Population standard deviation** equation is as follows: $$\sigma = \sqrt\frac{\sum(X-\mu)^2}{N}$$
Standard deviation is always greater or equal to mean absolute deviation, i.e. $\sigma \ge MAD$
**Note**: Standard deviation gives more weight to the larger deviation when it's being squared

Since population is too big ⇒ often we use inferential statistics (sample population)
From the sample variance and sample deviation ⇒ we inferred from it and to estimate the parameter (population parameter)

**Sample variance** = $$s^2 = \frac{\sum(X-\bar{X})^2}{n-1}$$and the unit would be unit$^2$.

**Sample standard deviation** = $$s = \sqrt\frac{\sum(X-\bar{X})^2}{n-1}$$
where $\bar{X}$ is the sample mean, and $n$ is the sample population.
The denominator is $n-1$, and it allows us to have unbiased estimate
The sample standard deviation can be interpreted as the unbiased estimator of the population standard deviation, $\sigma$.

Standard deviation is often used as a measure of risk, and the mean is the estimate of expected return.

#### Downside risk
As an investor, the positive portion of the standard deviation is not taken as risk, instead it's an unexpected reward; only the **downside (negative side) would be taken as a risk**.
The target downside deviation is also known as 'target semideviation'.

The **measure of downside risk** equation is as follows:
$$s_{target} = \sqrt{\frac{\sum(X-B)^2}{n-1}}$$
where $B$ is the proclaimed benchmark (expected return).
**Note**: $\sum$ only uses the negative deviations (less than benchmark deviation); $n$ is equal to the sample size (which include all positive and negative deviations)

![[Screenshot 2022-10-07 at 13.34.50.png]]

With investments and portfolios, a very common downside risk measure is downside deviation, which is also known as [semi-deviation](https://www.investopedia.com/terms/s/semideviation.asp). This measurement is a variation of standard deviation in that it measures the deviation of only bad [volatility](https://www.investopedia.com/terms/v/volatility.asp). It measures how large the deviation in losses is.

### Coefficient of Variation
**Coefficient of variation**:
- addresses how much dispersion exists relative to mean of a distribution
- allows for direct comparison of dispersion across different datasets

**Coefficient of Variation** equation is as follows:
$$\mathrm{Coefficient\,of\,Variation = \frac{s}{\bar{X}}}$$
since in the application of portfolio return/ financial analysis, the $s$ = risk and $\bar{X}$ = return or expected value of the distribution, so it can be also written as:

$$\mathrm{Coefficient\,of\,Variation = \frac{Std\,Dev}{Avg\,Return} = \frac{Risk}{Return}}$$
which means risk per unit of return, the lower means lower risk per unit of return.

**Sharpe Ratio** is the inverse of the coefficient of variation, it measures the return per unit of risk; it is the excess return per unit of risk (risk-adjusted return):

To understand the Sharpe ratio of an investment:
$$\frac{r-r_f}{s} = \mathrm{\frac{Excess\,return}{Risk}}$$
where $r$: return from investment; $r_f$: risk-free rate; therefore the return is excess return.


In investment terms, investors are looking for more return and less risk; therefore, the coefficient of variation: the lower the value, it's more desirable; as for Sharpe Ratio (risk-adjusted return): the higher the value is the better.

### Sortino ratio
**Sortino ratio** is a variation of the Sharpe ratio that differentiates harmful volatility from total overall volatility by using the asset's standard deviation of negative portfolio returns—downside deviation.

$$\mathrm{Sortino\,ratio = \frac{R_{p}- R_f}{\sigma_{d}}}$$

where $R_p$​: Actual or expected portfolio return; $R_f​$=Risk-free rate; $\sigma_{d}$: Standard deviation of the downside​ (i.e. only losses occur on the left side of return distribution, lower than the mean expected return).

### Normal distribution
There are a few characteristics which define the **normal distribution**:
- mean = median = mode
- $X(\mu,\sigma)$ ~ (0,1)
- 68% of values are $\pm$ 1 s.d.; 95% of values are $\pm$ 2 s.d.; 99% of values are $\pm$ 3 s.d.
- symmetrical

### Other types of distribution
Skewness:
- Positively skewed distribution - longer right tail (mean > median > mode)
- Negatively skewed distribution - longer left tail (mean < median < mode)


sample skewness = $$S_{skewness} = \frac{1}{n} \frac{\sum\limits_{i=l}^n(X_i-\bar{X})^3}{s^3}$$
where $n$: number of observations; $s$:
and $n>0$ and $s\ge0$ and the nominator is positive or negative depending on the dominant high magnitude observations
positively skewed distribution ⇒ positive skewness value
negatively skewed distribution ⇒ negative skewness value
skewness level of $|S_k| > 0.5$ is significant level of skewness

![[Screenshot 2022-10-07 at 13.18.28.png]]

### Kurtosis
**Kurtosis** a measure of whether it is more or less peaked than the normal distribution

There are 3 descriptions of kurtosis:
- **Mesokurtic** - same peakedness of normal distribution
- **Leptokurtic** - more peaked than that of normal distribution
- **Platykurtic** - fatter, less peaked, (flat) than that of normal distribution

In investment terms, leptokurtic distribution is more risky than normal distribution as there are outliers and longer tails on both ends

The **sample kurtosis** equation is as follows: $$s_{kurtosis}=\frac{1}{n}\frac{\sum\limits_{i=l}^n(X_i-\bar{X})^4}{s^4}$$
**Note**: It is very similar to the calculation of sample skewness, except to the power of 4 instead of 3.
when $s_{kurtosis} > 3$ = leptokurtic; when $s_{kurtosis} < 3$ = platykurtic

Besides, there are differences between sample and excess kurtosis.

$$\mathrm{Excess\,kurtosis = Sample\,kurtosis -3}$$


Excess kurtosis = $s_{kurtosis} -3$; so the base value of 0 indicate mesokurtic (normal distribution)

![[Screenshot 2022-10-07 at 13.19.58.png]]

![[Screenshot 2022-10-07 at 13.20.26.png]]

### The relationship between skewness, kurtosis and investment risk and return
![[Screenshot 2022-09-12 at 14.39.54.png]]

## Covariance and correlation
### Correlation 
**Correlation** is:
- a measure of the strengths of the *linear* relationship of two random variables
- has no units
- ranges from -1 to +1, that is $-1 \le \rho_{x,y} \le +1$

In order to calculate correlation, one must calculate the covariance first.

### Covariance
**Covariance**:
- between two variables is a measure of the degree to which the two variables tend to move together
- A positive covariance indicates that the variables tend to move together; a negative covariance indicates that the variables tend to move in opposite directions relative to their means.

The formula of **covariance** is as follows: $$\mathrm{covariance}=Cov_{x,y} = \frac{\sum|(X-\bar{X})(Y-\bar{Y})|}{n-1}$$
where $n$: number of periods.
**Note:** variance of one variable - the covariance is with itself
it is difficult to interpret as the covariance is not normalised

Negative covariance means rates of return for one security will tend to be above its mean return in periods when the other is below its mean return, and vice versa. Positive covariance means that returns on both securities will tend to be above (or below) their mean returns in the same time periods. For the returns to always move in opposite directions, they would have to be perfectly negatively correlated. Negative covariance by itself does not imply anything about the strength of the negative correlation, it must be standardised by dividing by the product of the securities' standard deviations of return.

The formula of **correlation coefficient** is as follows:
$$\mathrm{correlation} = \rho_{x,y} = \frac{Cov_{x,y}}{(\sigma_x\sigma_y)} = \mathrm{\frac{covariance}{products\,of\,std.dev.}}$$
correlation is a standardised measure of which whether two products move together.
where correlation:

$\rho_{x,y} = -1$ means negative linear relationship
$\rho_{x,y} = 0$ means no linear relationship
$\rho_{x,y} = 1$ means positive linear relationship

### Limitations to correlation analysis
1. Sensitive to outliners (it can be dealt with using trimming and windsorisation) ⤍ however, analyst should always inspect whether that outlier was merely just the noise or it can provide useful information
2. Spurious correlation (could be completely irrelevant and could have confounding variable) (https://www.tylervigen.com/spurious-correlations)
3. Correlation does not imply causation

---
# Questions before starting this section:
- [ ] What are the different data types
- [ ] Which are the most commonly used data presentation/graphs
- [ ] What is a contingency table
- [x] What is downside deviation
- [x] What is the need of calculating skewness and kurtosis?
