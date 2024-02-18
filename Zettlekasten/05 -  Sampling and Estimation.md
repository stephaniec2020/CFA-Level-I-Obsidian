# 5 -  Sampling and Estimation
202209201815
Status: #📥 
Tags: [[CFA Level I]]

## Objectives:
- [x] Compare and contrast probability samples with non-probability samples and discuss applications of each to an investment problem.
- [x] Explain sampling error.
- [x] Compare and contrast simple random, stratified random, cluster, convenience, and judgmental sampling.
- [x] Explain the central limit theorem and its importance.
- [x] Calculate and interpret the standard error of the sample mean.
- [x] Identify and describe desirable properties of an estimator.
- [x] Contrast a point estimate and a confidence interval estimate of a population parameter.
- [x] Calculate and interpret a confidence interval for a population mean, given a normal distribution with 1) a known population variance, 2) an unknown population variance, or 3) an unknown population variance and a large sample size.
- [x] Describe the use of resampling (bootstrap, jackknife) to estimate the sampling distribution of a statistic.
- [x] Describe the issues regarding selection of the appropriate sample size, data snooping bias, sample selection bias, survivorship bias, look-ahead bias, and time-period bias.

## Review:
- This chapter is more theoretical basis, there is only one formula to remember, which is SEM, otherwise, all others are theories which have to be memorised
- [ ] Central limit theorem's assumption and characteristics
- [ ] learn what is point estimate and confidence interval estimate of a population parameter
- [ ] types of biases
- [ ] explain sampling error
- [ ] compare and contrast different sampling methods
- [ ] describe the properties of an estimator
- [ ] memorise the formula for confidence interval

---

## Sampling
In the real world scenario, there are 2 important concepts:
- **Population** - Descriptive statistics ⇒ Parameter; Population is often unrealistic to measure as it's not possible to have all the information
- **Sample** - used inferential statistics to infer to the population mean and standard deviation, where it provides as an estimate to the true population parameter

#### What is the best way to do sampling?
##### Probability sampling methods
It gives every member of population having the equal change of being selected
- **Simple random sampling** ⇒ every element has equal probability to be selected (i.e. random number generator to generate the numbers to sample from
- **Systematic sampling** ⇒ using the last digit of account number, sampling every nth observation is an example of systematic sampling)
- **Stratified random sampling** ⇒ random selection from subgroups with distinctive characteristics (e.g. from low, medium, and high risk accounts)
- **Cluster sampling** ⇒ assume each cluster is representative of a population, each cluster is then used as a sampling unit (e.g. cluster - branch of firm/geographical location)
	- **One-stage cluster sampling** - ALL observations in selected clusters comprise the sample
	- **Two-stage cluster sampling** - Randomly-selected subset of observations from the selected clusters (it is less representative compared to one-stage cluster sampling)

##### Non-probability sampling methods
- **Convenience sampling** - samples are selected based on whether or not the data is easily accessible to the researcher (i.e. cost/ease of access)
- **Judgemental sampling** - handpicking samples based on a researcher's knowledge and professional judgement (i.e. researcher's subjective judgment)

#### Sampling Error
- Population mean: $\mu$; population standard deviation: $\sigma$
- Sample population mean: $\bar{X}$; sample standard deviation: s

**Population distribution** 
**Sampling distribution** - the probability distribution of all possible sample statistics computed from a set of equal-size samples randomly drawn from the same population. As there are more samples, there would be a distribution of its own, which differs from the population distribution

## Central Limit Theorem
**Definition**: "For simple random sample of size $n$ from a population with mean $\mu$ and variance $\sigma^2$, the sample mean approaches a normal distribution with a mean of $\mu$ and variance $\frac{\sigma^2}{n}$ and standard deviation of $\frac{\sigma}{\sqrt{n}}$"

- Population mean: $\mu$; population standard deviation: $\sigma$
- Sample population mean: $\bar{X}$; sample standard deviation: s

**Population distribution** - true population distribution, which does not have to be normal distribution
**Sampling distribution** - 
- the mean of the sample: $\bar{X}$ is an estimate of population mean: $\mu$
- as there are more samples, there would be a distribution of its own, which differs from the population distribution; however, with the sample size $n$ increase, the variance is smaller as it is $\frac{\sigma^2}{n}$
- it approximates to be normal when the sample size $n \ge 30$

## Point and interval estimates
### Properties of Estimators
- **Consistent** - accuracy of the estimate increases as the sample size increase 
  (i.e. accuracy ↑ as $n$ ↑)
- **Unbiased** - expected value of the estimator is equal to the parameter to be estimated 
  (i.e. $E(\bar{X}) = \mu$)
- **Efficient** - no other unbiased estimator has a sampling distribution with a smaller variance

The sample mean: $\bar{X}$ is a good example of consistent, unbiased and efficient estimator of the population mean: $\mu$.

**Point estimate** - single value used to estimate population parameters
**Confidence Interval** - range of values in which the population parameter is expected to fall within (i.e. range with a prescribed level of confidence that the sample fall within that range)
- it is presented as **Point estimate ± (reliability factor ⨉ standard error)**
	- where the reliability factor is read from the t-table (i.e. d.f. = n-1 and from the 1-tailed test; d.f. = 60, 99% confidence, reliability factor is 2.660) or memorised (i.e. 95% confidence reliability factor is 1.96)
	- sometimes the standard error has to use the **standard error of the mean (SEM)**, which is the standard deviation of the distribution of sample means.

**Note**: When both the population standard deviation and sample standard deviation are given, use the population standard deviation, as it represents "the ground truth"

- Apply the $\frac{\sigma}{\sqrt{n}}$ to find the standard deviation from sample

The formula for **standard deviation of a sample mean (SEM)**, is as follows:
$$SEM = \sqrt{\frac{s^2}{n}}=\frac{s}{\sqrt{n}}$$
where $s^2$: sample variance; $n$: the number of samples from the sampling population

> For **population to standard deviation of the sample mean**: 
> A population has a mean of 8 and variance of 16. A random sample of 100 observations was taken. What is the standard deviation of the sample mean?
> (16/100)^0.5 = 0.4



## Confidence Intervals
3 of those **confidence intervals** must remember by heart:
- 90%: $\bar{X} - 1.65\sigma < X < \bar{X} + 1.65\sigma$ 
- 95%: $\bar{X} - 1.96\sigma < X < \bar{X} + 1.96\sigma$ 
- 99%: $\bar{X} - 2.58\sigma < X < \bar{X} + 2.58\sigma$ 
where it can only be applied to normal distributions, since the CLT stated the sampling statistics if $n \ge 30$ approximates to be a normal distribution, the confidence interval can be applied to sample
- The **degree of confidence** is the confidence level associated with a confidence interval and is computed as 1 − α.
- other confidence intervals calculation (z-distribution): 
$$\bar{X} \pm Z_{\frac{\alpha}{2}}\sigma_{\bar{X}}$$
where $\alpha$: level of significance; $1-\alpha$: degree of confidence; $\frac{\alpha}{2}$: as it is two-tailed; $Z$: the Z-value from the z-distribution table, $\sigma_{\bar{X}}$: standard deviation of $x$ sample population (which is $\frac{\sigma}{\sqrt{n}}$)

Confidence intervals are narrower when the samples are larger and the standard errors of the point estimates of population parameters are less.

![[Screenshot 2022-09-27 at 18.34.26.png]]

eg. how to calculate the confidence interval from Z-table
![[Screenshot 2022-09-26 at 16.43.50.png]]

## T-distribution (For sampling $n$ > 30) 
- The sampling distribution can't be assumed to be normal if the sample size $n$ < 30
- However, if the population distribution is normal, then we can use student's t-distribution
- The t-distribution is used when the normal distribution (z-table) is not being used, as it does not fully satisfy the condition of using z-distribution (i.e. normal distribution)
- The t-distribution is less peaked and have fatter tails than the normal distribution.
- Although the _t_-distribution begins to approach the shape of a normal distribution for large sample sizes, at a sample size of 30 a _t_-statistic produces a wider confidence interval than a _z_-statistic.
- **Degrees of freedom (d.f.)** - defined as the degree to which the distribution deviates from normal distribution (i.e. $n-1$); as the d.f. approaches to normal, it is closer to normal distribution
- **If the population variance is not known, it has to be t-distribution**; providing that the sample size > 30 or the population is assumed to be normal

other confidence intervals calculation (t-distribution): 
$$\bar{X} \pm t_{\frac{\alpha}{2}}s_{\bar{X}}$$
where $\alpha$: level of significance; $1-\alpha$: degree of confidence; $\frac{\alpha}{2}$: as it is two-tailed; $t$: the t-value from the t-distribution table

### Criteria for selecting test statistics (When to use z or t-table)?
- z-table - use $z$ to find probability
- t-table - use probability to find $t$

- Is the population distribution normal?
- Is the population variance known?
- Is the sample size $n \ge$ 30?

![[Screenshot 2022-09-26 at 16.59.41.png]]

The monthly returns of a stock has a population mean of 1.9% and standard deviation of 8.2%. The distribution of the returns in non-normal. What is the 80% confidence interval on the mean monthly return over a 3-year period?

We are calculating the mean monthly return over a 3-year (36 mths) period. The sample size is therefore 36.

Non-normal -> n>30 -> Population variance known -> z-statistic

From z table, z=1.28 for 80% confidence interval. (Find corresponding z value for probability closest to 0.9)

Standard error = 8.2 / 36^0.5 = 1.37

Confidence interval = 1.9 +/- 1.28 x 1.37 = 0.15% to 3.65%

![[Screenshot 2023-06-24 at 14.50.50.png]]

## Flowchart to calculate confidence interval
![[Screenshot 2022-09-26 at 17.07.38.png]]


## Resampling methods
There are two alternative method of estimating the standard error of the sample mean **(S.E.M./SEM)** involve in resampling of the data: 
- Bootstrap 
- Jackknife

### Jackknife  🔪
- calculates multiple sample means
- each with one of the observations removes from the sample
- standard deviation of these sample means can then be used as an estimate of the standard error of sample means
- it is computationally simple when the number of observation is relatively small
- low-cost
- it can remove bias from statistical estimates

### Bootstrap  🥾
 - more computationally demanding
 - drawing the repeated samples of size $n$ from the full data set (replacing the sampled observations each time), then calculate the standard deviations of these samples means to give an estimate of S.E.M
 - improve accuracy 
 - can be used to construct confidence intervals for a variety of statistics in addition to the mean, such as median
 - estimate the distributions of complex statistics 

## Sample size consideration
- Larger sample reduces the sampling error and the standard deviation of the sample statistics is around its true (population) value.
- However, this does not imply that the sample should be as large as possible, or that the sampling error must be as small as can be achieved. Larger samples might contain observations that come from a different population, in which case they would not necessarily improve the estimates of the population parameters.
- Confidence intervals are narrower when the samples are larger and the standard errors of the point estimates of population parameters are less.
- Two limitations of large sample size:
	- may contain observation from another distribution (from another population), which might decrease the precision of parameter estimates
	- cost, when the cost of increasing the sample size is greater than the value of the extra precision gained, increasing the sample size is not appropriate.

## Types of biases
There are 5 major types of biases:
- Data-snooping bias
- Sample selection
- Survivorship bias
- Look ahead bias
- Time-series bias

### Data-snooping bias
- Occurs when analyst repeatedly use the same database to search for pattern or trading rules until one that works
- refers to the results where statistical significance of the pattern is overestimated because the results were found through data-snooping
- understand that whether the evidence of many different variables were tested, most of which were unreported until significant ones are found
- the lack of any economy theory that is consistent with the empirical results
- to avoid data-snooping, test a potentially profitable trading rule on a data set different from the ones you used to develop the rule (80 training + 20 testing dataset)

### Sample selection
- systematically excluded from the analysis mostly due to data unavailability
- cannot draw the conclusion from the sample to population as part of the data were excluded

### Survivorship bias
- most common form of sample selection bias
- only includes the existing ones, or readily accessible
- eg. mutual funds database, which survived as it's performing well, they do not include funds that have ceased to exist due to closure
- it might leads to overestimation of performance

### Look ahead bias
- when a study test a relationship using sample data that was not available on the test date
- occurs when a study tests a relationship using sample data that was not available on the test date

### Time-series bias
- can result if the time period over which the data is gathered is either too short or too long
- It’s not clear whether this relationship will continue in the future or if it is just an isolated occurrence
- the data with too long of a time period should be divided into two subsamples that span the period before and after the change











---
## Questions before starting this section:
- [ ] Potential problems of biases
- [ ] Where do you get the right sample 
- [ ] How representative sample is to the population
- [ ] when to use z-/t-statistics?



## Codes to test understanding of objectives





>Although the _t_-distribution begins to approach the shape of a normal distribution for large sample sizes, at a sample size of 30 a _t_-statistic produces a wider confidence interval than a _z_-statistic. A confidence interval for the population mean is the sample mean plus-or-minus the appropriate critical value times the _standard error_, which is the standard deviation divided by the square root of the sample size. If a population is normally distributed, we can use a _t_-statistic to construct a confidence interval for the population mean from a small sample, even if the population variance is unknown.