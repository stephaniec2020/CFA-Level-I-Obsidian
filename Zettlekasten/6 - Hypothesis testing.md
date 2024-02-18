# 6 - Hypothesis testing
202209271159
Status: #📥 
Tags: [[CFA Level I]]

## Objectives:
- [x] define a hypothesis, describe the steps of hypothesis testing, and describe and interpret the choice of the null and alternative hypotheses.
- [x] compare and contrast one-tailed and two-tailed tests of hypotheses.
- [x] explain a test statistic, Type I and Type II errors, a significance level, how significance levels are used in hypothesis testing, and the power of a test.
- [x] explain a decision rule and the relation between confidence intervals and hypothesis tests, and determine whether a statistically significant result is also economically meaningful.
- [x] explain and interpret the p-value as it relates to hypothesis testing.
- [x] describe how to interpret the significance of a test in the context of multiple tests.
- [ ] identify the appropriate test statistic and interpret the results for a hypothesis test concerning the population mean of both large and small samples when the population is normally or approximately normally distributed and the variance is 1) known or 2) unknown.
- [ ] identify the appropriate test statistic and interpret the results for a hypothesis test concerning the equality of the population means of two at least approximately normally distributed populations based on independent random samples with equal assumed variances.
- [ ] identify the appropriate test statistic and interpret the results for a hypothesis test concerning the mean difference of two normally distributed populations.
- [ ] identify the appropriate test statistic and interpret the results for a hypothesis test concerning (1) the variance of a normally distributed population and (2) the equality of the variances of two normally distributed populations based on two independent random samples.
- [ ] compare and contrast parametric and nonparametric tests, and describe situations where each is the more appropriate type of test.
- [ ] explain parametric and nonparametric tests of the hypothesis that the population correlation coefficient equals zero, and determine whether the hypothesis is rejected at a given level of significance.
- [x] explain tests of independence based on contingency table data.

## Review:
- [ ] describe the properties of the chi-square distribution and the F-distribution, and calculate and interpret their degrees of freedom


---

## Hypothesis test
**Hypothesis Testing** is a type of statistical analysis in which you put your assumptions about a population parameter to the test. It is used to **estimate the relationship between 2 statistical variables**.

There are different types of hypothesis test which is summarised in the table:

|Test of| Statistic test to use| Degrees of freedom |
|:----:|:----:|:----:|
|Mean|t or z|n-1|
|**Difference in means (not so simple)**|t |n-1|
|Mean differences|t|n-1|
|Variance|$X^2$|n-1|
|Equal variances (of 2 samples)|F|$n_1$ -1, $n_2$ -1|
|Correlation (of 2 samples)|t|n-2|
|Independence (of 2 samples)|$X^2$|(r-1)(c-1)|
|Regression slope: significance|F|1,n-2|
|Regression slope: value|t|n-2|


## Hypothesis testing procedure
**Hypothesis testing** is broken down into 7 steps:
1. State the hypothesis
2. Identify test statistics and probability distribution
3. Specify significance level
4. State decision rule
5. Collect & calculate the statistics of test data
6. Make statistical decision
7. Make economic decision

### 1. State the hypothesis 
In stating the hypothesis, there are always two hypotheses to be made when applying statistics:
- **Null hypothesis** - $H_0$ - hypothesis to be tested (hypothesis that contains the equal sign (i.e. =, $\le$, $\ge$))
- **Alternative hypothesis** - $H_A$ - concluded hypothesis when $H_0$ is rejected (the one you suspect to be true)
- **Always set the $H_A$ first, as it is the one that you suspect to be true**

$\theta$ - population parameter
$\theta_0$ - possible value of population parameter

There are 3 types of hypothesis:

|Null hypothesis| Alternative hypothesis|
|:----:|:----:|
|$\theta = \theta_0$|$\theta \ne \theta_0$|
|$\theta \le \theta_0$|$\theta > \theta_0$|
|$\theta \ge \theta_0$|$\theta < \theta_0$|

eg. suspecting the fund return beats the benchmark
The hypothesis testing for this particular sample of **fund return beats the benchmark** is as follows:
$$\theta = R_f -R_b$$
where $H_A: \theta > 0$, therefore the $H_0: \theta \le 0$

### 2. Identify the test statistics
- **Test statistics** - the value that is the basis for rejecting $H_0$

$$\mathrm{Test\,statistics = \frac{Sample\,statistic - H_0 value}{Std\,Error\,of\,Sample\,statistics}} $$
where standard error of sample statistics - $\frac{s}{\sqrt{n}}$

where one of the test could potentially be used: z-statistics, t-statistics, chi-square test, f-distribution.

### 3. Specify the significance level
Since it is inferential statistics from sample to population, there might be times that one may encounter one of the **two types of errors**: 
- **Type I Error** - rejection of the null hypothesis when it is actually true (i.e. false positive)
- **Type II Error** - failure to reject the null hypothesis when it is actually false (i.e. false negative)

$H_0$: Not Pregnant 
$H_A$: Pregnant
![[Pasted image 20221024143153.png]]

![[Screenshot 2022-09-28 at 13.38.56.png]]

**Hypothesis error reduction**: 
- **Type I Error** is defined as rejecting the null hypothesis when it is actually true. The probability of committing a Type I error is the **significance level or alpha risk**.
- Type II error is difficult to quantify.
- In reduction of type I error by **lowering the $\alpha \%$ is not the best way as type II error will increase**
- The only way to reduce both types of errors is to **increase in sample size $n$**.
- Significance level has to be set at this stage, otherwise, it is also known as p-hacking
- Significance level ($\alpha$) is commonly set as 5% (moderately significant)
- Power of the test is correctly to reject the null hypothesis

![[Screenshot 2022-10-24 at 14.34.24.png]]
https://www.scribbr.com/statistics/type-i-and-type-ii-errors/

### 4. State the decision rule
The decision rule can either be:
- **One-tailed test**
- **Two-tailed test**

The decision rule depends on the null hypothesis set ($\theta = \theta_0$ , $\theta \le \theta_0$ , $\theta \ge \theta_0$).

**One-tailed test** - whether the critical value lies beyond one-sided of the distribution (i.e. $\theta \le \theta_0$ OR $\theta \ge \theta_0$)

![[Screenshot 2022-09-29 at 14.29.08.png]]

**Two-tailed test** - whether the critical value lie beyond two-tailed of the distribution (i.e. $\theta = \theta_0$)

![[Screenshot 2022-09-29 at 14.33.43.png]]

### 5. Collect and test data
Once the data is collected, one should **ensure the quality of the sample**:
- Check for measurement errors
- Avoid sample selection bias - e.g. survivorship bias, time period bias

### 6. Make statistical decision
- Calculate the t-statistics/z-statistics score and see whether the t-statistics/z-statistic score above the critical value (which is decided by the degree's of freedom and the significance level $\alpha$)
- Either reject the null hypothesis or fail to reject the null hypothesis.

![[Screenshot 2022-09-29 at 14.45.00.png]]

![[Screenshot 2022-09-29 at 14.45.39.png]]

There is another approach, which is the p-value approach:
![[Screenshot 2022-09-29 at 14.48.24.png]]
Just the p-value is reported without selecting a significance level, it allows the reader to make their own conclusions on the significance of the results


### 7. Make the economic decision
**Note:** Statistical significance $\ne$ economic significance
In the example of mutual fund outperforms the benchmark at 5% significance level.
There should also be other concerns, such as:
- **cost** (e.g. manager fees, advisory fees, transaction fees, brokerage fees)
- **taxes** - additional taxes?
- **risk** - is the risk level appropriate for the client?

## Hypothesis testing of a single mean
**Hypothesis testing of a single mean** is:
- a statistical technique used to make inferences about a population mean based on sample data
- the goal is to determine whether there is sufficient evidence to support or reject a particular claim or hypothesis about the population mean.

The null hypothesis represents the claim being tested, assuming no significant difference or effect, while the alternative hypothesis represents the claim that contradicts the null hypothesis and suggests a significant difference or effect.

|Null hypothesis ($H_0$)| Alternative hypothesis ($H_A$)|
|:----:|:----:|
|$\theta = \theta_0$|$\theta \ne \theta_0$|
|$\theta \le \theta_0$|$\theta > \theta_0$|
|$\theta \ge \theta_0$|$\theta < \theta_0$|

**Z-statistic** is calculated by subtracting the hypothesised parameter from the parameter that has been estimated and dividing the difference by the standard error of the sample statistic. 

Here, the **test statistic (z-statistics)** equation is as follows:
$$z\,statistics = \frac{(\bar{X} − \mu)}{\frac{s}{\sqrt{n}}}$$

##### Criteria for selecting test statistics in testing single mean
![[Screenshot 2022-09-29 at 15.23.28.png]]

![[Screenshot 2022-09-29 at 15.34.17.png]]

![[Screenshot 2022-09-29 at 15.35.00.png]]

![[Screenshot 2022-09-29 at 15.35.11.png]]

## Hypothesis testing of differences between two means
**Hypothesis testing of differences between two means** is:
- a statistical technique used to compare the means of two independent groups or populations
- It helps determine whether there is sufficient evidence to support or reject the claim that the means of the two groups are significantly different from each other
- where **sample 1 and sample 2 has to be both from normal distribution**

![[Screenshot 2022-09-29 at 15.36.35.png]]

#### After that, we have to determine:
1. Whether the two population are **independent**? Chi-square test of independence
2. Whether two population have **equal variance**? F-test of equal variance

Answer of 1. Whether the two population are **independent** from each other, if so, you can proceed to question 2.
Answer of 2. If so, whether the **variance** are equal (i.e. $\sigma_1{^2} = \sigma_2{^2}$) or not. 

2a. If the **population variance are equal**, we can use the **t-test of pooled variance**:
$$t = \frac{\bar{X_1}-\bar{X_2}}{\sqrt{(\frac{s^2p}{n_1}+\frac{s^2p}{n_2})}}$$
where $S_p{^2}$ : pooled variance; $\bar{X}$: respective mean of each sample; $n$: number of samples from each population

The degrees of freedom of **equal population variance** is:
$$d.f. = n_1 + n_2 - 2$$

2b. When the **population variance are not equal, (i.e. $\sigma_1{^2} \ne \sigma_2{^2}$),** we have to use **individual sample variance**:
$$t = \frac{\bar{X_1}-\bar{X_2}}{\sqrt{(\frac{s_1{^2}}{n_1}+\frac{s_2{^2}}{n_2})}}$$
where $s_1{^2}$ is the variance of sample 1 and $s_2{^2}$ is the variance of sample 2
**Note:** we can always make the deduction of outcome from 2 unrelated events have unequal population variance

and the **degrees of freedom of unequal population variance** is:
$$d.f. = \frac{(n_1-1)s_1{^2}+(n_2-1)s_2{^2}}{n_1+n_2-2}$$
it is also known as the non-pooled variance.

1. If the **populations are not independent** to each other, we have to used **paired sample test** and the equation is as follows:
 $$d=x_1-x_2$$
where d: a single random variable and perform hypothesis testing on it as in the case of a single mean

Then we perform the t-test:
$$\mathrm{Test\,statistics = \frac{d - H_0 value}{Std\,error\,of\,sample\,statistics}} $$
where **standard error of sample statistics** is as follows:
$$\mathrm{Std\,error\, of\,sample\,statistics = \frac{s}{\sqrt{n}}}$$
where one of the test could potentially be used: z-statistics, t-statistics, chi-square test, f-distribution

## Summary for single and difference between two means statistical analysis

![[Screenshot 2022-09-29 at 19.45.36.png]]

## Chi-square test
**Chi-square test ($X^2$)** is used for:
- concerning the **variance** of a **normally distributed population** -  $\sigma_0{^2}$: hypothesised value of the variance, and $s^2$ is the sample variance (i.e. $H_0$: $s^2 = \sigma_0{^2}$, $H_A$: $s^2 \ne \sigma_0{^2}$)
- **independence** - determine whether there is a significant association between two categorical variables; ($H_0$: variables are independent, $H_A$: variables are related)
- **goodness-of-fit** - assess how well an observed data set fits a particular theoretical distribution; ($H_0$: observed data follows a theoretical distribution, $H_A$: observed data does not follow the specified distribution)

In the **test of variance,** the null and alternative hypothesis can also be:

|Null hypothesis $H_0$| Alternative hypothesis $H_A$|
|:----:|:----:|
|$s^2 = \sigma_0{^2}$|$s^2 \ne \sigma_0{^2}$|
|$s^2 \le \sigma_0{^2}$|$s^2 > \sigma_0{^2}$|
|$s^2 \ge \sigma_0{^2}$|$s^2 < \sigma_0{^2}$|
**Note:** If the question provide standard deviation, it is essential to convert to variance
- degrees of freedom (d.f.) = $n - 1$

### Test statistics for test of variance using chi-square test
The test statistics for test of variance using chi-square test equation is as follows:
$$X^2{_{n-1}}= \frac{(n-1)s^2}{\sigma_0{^2}}$$
where $\sigma_0{^2}$: hypothesised value of the variance, and $s^2$ is the sample variance, and chi-square table is used.

### Chi-square distribution
**Chi-square distribution** is:
- A chi-square ($Χ^2$) distribution is a continuous probability distribution that is used in many hypothesis tests.
- The shape of a chi-square distribution is determined by the parameter k. The graph below shows examples of chi-square distributions with different values of k.
- The chi-square distribution is a continuous probability distribution with the values ranging from 0 to ∞ (infinity) in the positive direction. 
- The $Χ^2$ can never assume negative values.

#### Shape of Chi-square distribution
- The shape of the chi-square distribution depends on the number of degrees of freedom ‘k’. When ‘k’ is small, the shape of the curve tends to be skewed to the right, and as the ‘k’ gets larger, the shape becomes more symmetrical and can be approximated by the normal distribution.
- As k increases, the distribution looks more and more similar to a normal distribution. In fact, when k is 90 or greater, a normal distribution is a good approximation of the chi-square distribution.
Reference: https://www.scribbr.com/statistics/chi-square-distributions/

![[Screenshot 2022-10-16 at 19.35.06.png]]
![[Screenshot 2022-10-16 at 19.37.20.png]]

#### The non-central chi-square distribution
- The non-central chi-square distribution is a more general version of the chi-square distribution. It’s used in some types of power analyses.
- The non-central chi-square distribution has an extra parameter called λ (lambda) or the non-central parameter. This parameter changes the shape of the distribution, shifting the peak to the right and increasing the variance as λ increases.

![[Screenshot 2022-10-16 at 19.46.06.png]]

## F-test
**F-test** is:
- used for hypothesis test concerning the **equal variances** between two **normally distributed populations** and **independent samples** (i.e. the need for using chi-square test for both whether they are normally distributed or two variables are independent or related) - since they are independent samples, so they may have different degrees of freedom (d.f.)
- **regression slope significance** 

For the **equal variance** test of two assumed normally distributed population: 

|Null hypothesis $H_0$| Alternative hypothesis $H_A$|
|:----:|:----:|
|$\sigma_1{^2} = \sigma_0{^2}$|$\sigma_1{^2} \ne \sigma_0{^2}$|
|$\sigma_1{^2} \le \sigma_0{^2}$|$\sigma_1{^2} > \sigma_0{^2}$|
|$\sigma_1{^2} \ge \sigma_0{^2}$|$\sigma_1{^2} < \sigma_0{^2}$|

that's why the **f-table** is designed for different significant values (i.e. 2.5% or 5%) and look at the two different d.f. to find the critical value 

### Test statistics for equal variance using F-test
The **test statistics for equal variance using F-test** is as follows:
$$F = \frac{s_1{^2}}{s_2{^2}}$$
where it has to force the test as a right tailed test, therefore $s_1{^2}$ has to be greater than $s_2{^2}$.
 $s_1{^2}$: variance of sample 1;  $s_2{^2}$: variance of sample 2;
**Note:** variance is being used to calculate F-score, therefore, if given standard deviation, it requires "s-squared"(i.e. $s^2$) and the F-table is being used.

### F-distribution
#### Origin of F-distribution
- Chi-square distributions are important in defining the F distribution, which is used in ANOVAs.
- Imagine you take random samples from a chi-square distribution, and then divide the sample by the k of the distribution. Next, you repeat the process with a different chi-square distribution. If you take the ratios of the values from the two distributions, you will have an F-distribution.

#### Properties of F-distribution
- The F-distribution is positively skewed and with the increase in the degrees of freedom k1 and k2, its skewness decreases. 
- The value of the F-distribution is always positive, or zero since the variances are the square of the deviations and hence cannot assume negative values. Its value lies between 0 and ∞
- The shape of the F-distribution depends on its parameters k1 and k2 degrees of freedom.
![[Screenshot 2022-10-16 at 19.39.41.png]]

## Pearson correlation
**Pearson's correlation** is:
- To **assess the linear relationship between two variables** (assumed both variables are normal)
- Correlation coefficient is a standardised measure of which whether two products move together.
where correlation:

$\mathrm{Corr}(X,Y) = \rho_{XY} = -1$ means negative linear relationship
$\mathrm{Corr}(X,Y) = \rho_{XY} = 0$ means no linear relationship
$\mathrm{Corr}(X,Y) = \rho_{XY} = 1$ means positive linear relationship

$$\mathrm{Corr}(Y,X) =\mathrm{Corr}(X,Y) = \frac{\mathrm{Cov}(X,Y)}{\sqrt{\sigma^2(X)}\sqrt{\sigma^2(Y)}}=\frac{\mathrm{Cov}(X,Y)}{\sigma(X)\sigma(Y)}$$

### Hypothesis test of Pearson correlation
Is there a significant relation between variable X and Y?
$H_0$: $\rho_{XY} = 0$
$H_A$: $\rho_{XY} \ne 0$

### Sample/data collection for Pearson correlation
Collect a sample size of $n$ and calculate the correlation coefficient from them
**Pearson correlation coefficient** equation is as follows:
$$r_{XY} = \frac{Cov(X,Y)}{s_Xs_Y}$$

### Test statistics for Pearson correlation coefficient
The **test statistics for Pearson correlation coefficient** is as follows:
$$t = \frac{r\sqrt{(n-2)}}{\sqrt{1-r^2}}$$
where **Pearson's correlation coefficient** is used, the degree of freedom is as follows: $$d.f. = n-2$$
**Note**: As the sample size increases, there's higher probability of rejection of $H_0$ for Pearson correlation coefficient
![[Screenshot 2022-09-30 at 15.32.25.png]]

## Parametric and non-parametric test
**Parametric statistics** are based on **assumptions about the distribution of population** from which the sample was taken. **Nonparametric statistics** are not based on assumptions, that is, the data can be collected from a sample that **does not follow a specific distribution**.

![[Screenshot 2023-06-24 at 11.18.55.png]]

### Parametric
Some of the parametric tests are:
- independent t-test
- paired t-test
- one-way ANOVA
- repeated measures ANOVA
- Pearson's correlation

It involves in both:
1. **Parameters** - eg. mean, variance
2. **Assumptions about the population distribution** - i.e. population distribution is normal

### Non-parametric
Analyst might use non-parametric test under these conditions:
- Distributional assumption are not met (i.e. the population distribution is not normal and the sample size is less than 30)
- Using ranked data - as ranked data are not normally distributed, parametric tests require strong scale than rank
- Not concerned with the parameter - e.g. the sample is random, is the sample from a population following a normal distribution?

## Spearman rank correlation coefficient
**Spearman rank correlation coefficient** is:
- non-parametric, cared about the ranked data

### Steps of calculating Spearman rank correlation coefficient:
1. Convert the data to pairwise ranked data
2. Rank them within the dataset, basically to counteract that the data is not normally distributed.
3. Calculate the difference between the ranked data
4. Square the differences
5. Calculate the sum of the squared differences

![[Screenshot 2022-09-30 at 15.57.53.png]]

The **Spearman Rank correlation coefficient** equation is as follows:
$$r_{XY} = 1 - \frac{6\sum{D_i{^2}}}{n(n^2-1)}$$
where $n$ is the number of paired samples.

Then it's similar to the Pearson correlation coefficient test-statistics:, input the $r$ of **Spearman Rank correlation coefficient** in this formula,
$$t = \frac{r\sqrt{(n-2)}}{\sqrt{1-r^2}}$$
and degrees of freedom is $n-2$
and use the t-distribution table to test whether to reject or not to reject the $H_0$

## Hypothesis test of independence using contingency table
The hypothesis **test of independence** using contingency table:
$H_0$: variables are independent
$H_A$: variables are related

**Contingency table** is used for:
- testing of independence of categorical/discrete data
- it is **NOT** for quantitative data. which was discussed extensively before (i.e. z-test, t-test, F-test, chi-square test)

Observed frequency - $O_{ij}$
Expected frequency - $E_{ij}$, expected based on the proportion

The **expected frequency** is as follows: 
$$E_{ij} = \mathrm{\frac{Total\,row\,i\times Total\,col\, j}{Overall\, Total}}$$

![[Screenshot 2022-09-30 at 16.07.56.png]]

### Test statistic for contingency table
To test the **independence of two data**, **chi-square statistics** is used:
$$\chi^2 = \sum{\frac{(O_{ij}-E_{ij})^2}{E_{ij}}}$$
where the numerator is the squared difference between the observed and expected

If the two variables are independent, ⇒ $\chi^2$ is close to 0
If the two variables have a relation, ⇒ $\chi^2$ is large

For **test of independence**, **one-tailed chi-square test** is used, with the **rejection region on the right**.

The equation for **degrees of freedom (d.f.) for independence** is as follows:
$$d.f. = (r-1)(c-1)$$
where $r$: number of rows and $c$: number of columns

![[Screenshot 2022-09-30 at 16.16.10.png]]

### Summary of how to perform a test of independence
![[Screenshot 2022-09-30 at 16.16.24.png]]

---
## Questions before starting this section:
- [ ] why do we only reject null hypothesis
- [ ] how do we assume the population is normal or not
- [ ] what are the criteria for
- [ ] what if $s_1{^2}$ is smaller than  $s_2{^2}$ and F-table  does not support


## Codes to test understanding of objectives
- [ ]