
# 4 - Common probability distributions
202209171647
Status: #📥 
Tags: [[CFA Level I]]

## Objectives:
- [x] define a probability distribution and compare and contrast discrete and continuous random variables and their probability functions.
- [x] calculate and interpret probabilities for a random variable given its cumulative distribution function
- [x] describe the properties of a discrete uniform random variable, and calculate and interpret probabilities given the discrete uniform distribution function.
- [x] describe the properties of the continuous uniform distribution, and calculate and interpret probabilities given a continuous uniform distribution.
- [x] describe the properties of a Bernoulli random variable and a binomial random variable, and calculate and interpret probabilities given the binomial distribution function.
- [x] explain the key properties of the normal distribution.
- [ ] contrast a multivariate distribution and a univariate distribution, and explain the role of correlation in the multivariate normal distribution.
- [ ] calculate the probability that a normally distributed random variable lies inside a given interval.
- [ ] explain how to standardize a random variable.
- [ ] calculate and interpret probabilities using the standard normal distribution.
- [x] define shortfall risk, calculate the safety-first ratio, and identify an optimal portfolio using Roy’s safety-first criterion.
- [ ] explain the relationship between normal and lognormal distributions and why the lognormal distribution is used to model asset prices.
- [ ] calculate and interpret a continuously compounded rate of return, given a specific holding period return.
- [ ] describe the properties of the Student’s t-distribution, and calculate and interpret its degrees of freedom.
- [ ] describe the properties of the chi-square distribution and the F-distribution, and calculate and interpret their degrees of freedom.
- [x] describe Monte Carlo simulation.

## Review:
- [ ] describe the properties of the chi-square distribution and the F-distribution, and calculate and interpret their degrees of freedom (look at chapter 6)
- [ ] calculate and interpret a continuously compounded rate of return, given a specific holding period return.
- [ ] explain the relationship between normal and lognormal distributions and why the lognormal distribution is used to model asset prices.
- [ ] Memorise 3 of those confidence intervals by heart:
	- 90%: $\bar{X} - 1.65\sigma < X < \bar{X} + 1.65\sigma$ 
	- 95%: $\bar{X} - 1.96\sigma < X < \bar{X} + 1.96\sigma$ 
	- 99%: $\bar{X} - 2.58\sigma < X < \bar{X} + 2.58\sigma$ 
- [ ] Lognormal and normal relationship 
- [ ] definition of independent and dependent relationship （look at chapter 7)
- [ ] holding period return and continuous compounding rate
- [ ] memorise the formula for effective annual rate of continuous compounding
- [ ] Roy’s safety-first criterion


---

## Random variable (Discrete vs Continuous)
Random variable is uncertain quantities or number:
- **Discrete** - number of possible outcomes can be **counted**
- **Continuous** - number of possible outcomes can be divided **infinitely** (with decimal places) (eg. time)

## Properties of a probability function
A probability function is denoted as $p(x)$, specifies a probability that a random variable is equal to a specific value. More formally, $p(x)$ is the probability that random variable $X$ takes on the value of $x$, which is $p(x) = P(X=x)$
The two key properties of a probability function are:
- $\sum p(x)= 1$, the sum of the probabilities for *all* possible outcomes, $x$, for a random variable, must be equal to 1 in probability distribution function
- Cumulative distribution function must start from 0 to 1, (i.e. $0 \le p(x) \le 1$)

## Data visualisation
For different types of random variable, there are different ways of visualisation:
- **Discrete random variable** - Probability distribution function, cumulative distribution function
- **Continuous random variable** - Probability density function, cumulative distribution function

$P(X=1)=p(1)=0.2$ where discrete probability distribution function is denoted with the p.

$P(X=1)=f(1)=0.2$ where the continuous probability density function is denoted with f.

$P(X \le 1)=F(1)=0.2$ where the probability of discrete/continuous probability density function is denoted with F.

## Properties of random variable
- **Binomial random variable** -  the number of "successes" in a **given number of trials (more than 1, if 1 trial has been conducted, it's Bernoulli random variable)**, whereby the outcome and either be ("success" or "failure"/"up" or "down"); the probability of success, $p$, is constant for each trial, and the trials are independent
- **Bernoulli random variable** - a binomial random variable for which the number of trials is 1 (i.e. mini-experiment of a trial)

## Types of distribution in random variable
There are several types of distributions in random variable:
- **Discrete uniform random variable** - all outcomes are equally likely
- **Bernoulli random variable** - is the simplest kind of random variable. It can take on two values, 1 and 0. It takes on a 1 if an experiment with probability p resulted in success and a 0 otherwise. Denoted the probability of success and failure, therefore $\sum P=1$
- **Binomial distribution** - i.e. is random variable that represents the number of successes in n successive independent trials of a Bernoulli experiment. (drawing tree diagrams would help)
	- n: number of trials
	- p: Probability of success
	- x: number of successes

![[Screenshot 2022-09-18 at 13.56.46.png]]

The final outcome is the number of successes in a series of $n$ trials. Under these conditions, the binomial probability function defines the probability of $x$ successes in $n$ trials.
It can be expressed using the following formula: $$P(X=x) = \mathrm{Num\,of\,ways} \times p^x(1-p)^{n-x}$$
or, through calculator, you can use the $nCr$ function
$$P(X=x) = \mathrm{nCr} \times p^x(1-p)^{n-x}$$
where nCr: 'n choose r'

> EXAMPLE: Binomial probability
> Assuming a binomial distribution, compute the probability of drawing three black beans from a bowl of black and white beans if the probability of selecting a black bean in any given attempt is 0.6. You will draw five beans from the bowl.
>
>Answer:
> Probability of success = Number of trials C Number of success x probability of success^n times of success x probability of failure^number of failures
> $$P(X=x) = \mathrm{nCr} \times p^x(1-p)^{n-x}$$
>$$P(X = 3) = p(3) = 5C3 \times 0.6^3 \times0.4^2$$$$ = (120 / 12)(0.216)(0.160) = 0.3456$$


![[Screenshot 2023-06-24 at 14.23.19.png]]

![[Screenshot 2022-09-18 at 13.55.01.png]]

For a given series of $n$ trials, the expected number of successes, or $E(X)$ is given by the following formula:
$$E(X) = np$$
If we perform $n$ trials, and the probability of success of each trial is $p$, we can expect $np$ successes.

Variance of a binomial random variable:
$$\sigma(X) = np(1-p)$$
![[Screenshot 2022-09-18 at 13.55.54.png]]
Eg. it can be used as stock price movement
![[Screenshot 2022-09-18 at 13.53.01.png]]

### Tracking error
Tracking error = Total return of the portfolio - total return of the index

![[Screenshot 2022-09-18 at 13.56.11.png]]

## Common probability distributions - continuous random variables
### Continuous uniform distribution (probability density function)
- equally likely outcome
- $\sum f(x) = 1$, area under the line = 1
- For $f(x) = \frac{1}{b-a}$, for $a \lt x \lt b$
	- and otherwise, outside of the probability = 0.

### Continuous uniform cumulative distribution 
- $F(x) = 0$ for $x<a$
- $F(x) = \frac{x-a}{b-a}$ for $a \lt x \lt b$
- $F(x) = 1$ for $x \gt b$

## Normal distributions
- $N (\mu, \sigma^2)$
- Symmetrical
- Mean = median = mode
- 68%, 95%, and 99% with 1, 2, and 3 $\sigma$ respectively
- Skewness = 0 
- Kurtosis = 3; excess kurtosis = 0 (peakedness)

### Types of normal distribution
- **Univariate distribution** - distribution of a single random variable
- **Multivariate distribution** - specifies the probabilities for a group of related random variables, it is only meaningful when the behaviour of each random variable in the group is in some way dependent on the behaviour of the other
- If the normal distribution of variable are added together with others, multivariate distributed data will also have a normal random distribution
- Correlation is the feature that distinguishes a multivariate distribution from a univariate normal distribution
- eg. 3 stocks have a normal distribution of return ⇒ the portfolio return must also be normal

Stock X return: $X \sim N(\mu_x,\sigma_x^2)$,
Stock Y return: $Y \sim N(\mu_y,\sigma_y^2)$
Stock Z return: $Z \sim N(\mu_z,\sigma_z^2)$

Portfolio return: P = 0.3X + 0.2Y + 0.5Z; portfolio return must be normal as well


$$
P \sim Normal
\begin{cases}
\mathrm{means}\,(\mu_x,\mu_y,\mu_z)
\\\mathrm{variances}\,(\sigma^2_x,\sigma^2_y,\sigma^2_z)\\
\mathrm{correlations}\,(r_{xy},r_{yz},r_{xz})
\end{cases}$$

$$
P \sim Normal\,(\mathrm{N\,variables})
\begin{cases}
\mathrm{N\,means}
\\\mathrm{N\,variances}\\
0.5N(N-1)\mathrm{\,pairwise\,correlation}
\end{cases}$$

### Confidence intervals
**Confidence interval** is a range of values around the expected outcome within which we expect the actual outcome to be some specified percentage of the time

3 of those **confidence intervals** must remember by heart:
- 90%: $\bar{X} - 1.65\sigma < X < \bar{X} + 1.65\sigma$ 
- 95%: $\bar{X} - 1.96\sigma < X < \bar{X} + 1.96\sigma$ 
- 99%: $\bar{X} - 2.58\sigma < X < \bar{X} + 2.58\sigma$ 

### Z-Table
eg. $P(X < 1.65) = 0.9505$, it means ~95% of the observations lie below 1.65 
or expect X to be < 1.65 with 95% confidence (if one tailed)

as normal distribution is symmetrical 
90%:
$P(X<1.65) = 0.9505$
$P(X<-1.65) = 1-0.9505 = 0.0495$
Therefore, $P(-1.65<X<1.65) = 0.9505-0.0495 = \approx 0.9$

## Z-transformation
Although in reality, there are normally distributed random variable, the case is their mean is rarely 0, which is the standard normal distribution. Therefore, to "standardises" the observation from normal distribution.
 
eg. earnings per share ~ $(2,0.5^2)$
that means the earnings per share has a mean of 2 and a variance of 0.25, and a standard deviation of 0.5

The **Z-transformation** transforms the normal distribution of a curve to standard normal distribution (i.e. **z-score**), the equation is as follows:

$$z= \mathrm{\frac{Observation - Population\,mean}{Standard\, deviation}}= \frac{x-\mu}{\sigma}$$
where $\mu$ is for the horizontal transformation, and the $\sigma$ is for the scaling to the standard normal distribution, z is the value that have to look up on the table.

If $z$ is negative, the percentage have to be $1-F(z)$.

## T-distribution
The **T-distribution's** characteristic:
- As the number of degrees of freedom grows, the t-distribution approaches the shape of the standard normal distribution.
- Compared to the normal distribution, the t-distribution has fatter tails.
- The t-distribution is symmetric about the mean and so it has skewness of zero.

## Evaluation of portfolio performance
There are several methods to evaluate the portfolio's performance, especially risk and return:
- Shortfall risk
- Roy's safety first ratio
- Holding period return
- TWRR
- MWRR

### Shortfall risk
- probability of return falling below threshold return
eg. Portfolio A return: N (10,5)
If the analyst decide that the threshold return less than 5% is unacceptable, (i.e. $R_L = 5\%$), that is known as the shortfall risk

$$Z_a = \frac{(5-10)}{5} = -1$$

and by looking at the cumulative z-table, we get the probability of: 0.8413
 
$$1 - (0.8413) = 0.1587 = 15.8\%$$
The shortfall risk of portfolio A is 15.87%

eg 2. Portfolio B return: N (15,7.5)
$$Z_b=\frac{(5-15)}{7.5} = -1.33$$
and by looking at the z-table, we get the value of: 0.9082

$$1-0.9082 = 0.0918 = 9.18\%$$

The shortfall risk of portfolio B is 9.18%.

**Note:** lower Z value ⇒ lower shortfall risk

![[Screenshot 2022-09-18 at 18.31.57.png]]

### Roy's safety first ratio

$$\mathrm{SFR} = \frac{E(R_p)-R_L}{\sigma p}$$
where SFR is the safety first ratio; $E(R_p)$ is the expected return portfolio percentage; $R_L$ is the minimum required threshold value of return; and $\sigma p$ is the standard deviation of portfolio

eg. $SFR_A = \frac{(10-5)}{5} = 1$; $SFR_A = \frac{(15-7.5)}{7.5} = 1.33$
where the higher SFR value ⇒ lower shortfall risk

![[Screenshot 2022-09-18 at 18.53.18.png]]

#### What is the shortfall risk of portfolio C?
Since the SFR is 1.25, the z-value of SFR is $-1.25 = 1-(0.8944) = 0.01056 = 10.56\%$


### Lognormal distribution
- Lognormal distribution is generated by the function $e^x$, where $x$ is normally distributed
- Since the natural logarithm, ln, of $e^x$ is $x$, the logarithms of lognormally distributed randome variables are normally distributed 
- Skew towards the right, positively skewed distribution
- It can never take on values below 0
- It is useful for modelling **asset prices**, whereas normal distribution is good at modelling portfolio returns.
- Using a lognormal distribution to model price relatives avoids this problem.

#### Price relatives
- A price relative is just the end-of-period price of the asset divided by the beginning price 
  ($\frac{S1}{S0}$) and is equal to (1 + the holding period return). 
- To get the end-of-period asset price, we can simply multiply the price relative times the beginning-of-period asset price. 
- Since a lognormal distribution takes a minimum value of zero, end-of-period asset prices cannot be less than zero. 
- A price relative of zero corresponds to a holding period return of –100% (i.e., the asset price has gone to zero). Recall that we used price relatives as the up-move and down-move (multiplier) terms in constructing a binomial tree for stock price changes over a number of periods.

### Holding period return
- For a holding period return (HPR) over any period, the equivalent continuously
compounded rate over the period is ln(1 + HPR).

ln (FV/PV) = ln(1+HPR) = Rcc
HPR

If Rcc = 10%, the
(effective) holding period return over two years is e(0.10)2 – 1 = 22.14%. In general, the
holding period return after T years, when the annual continuously compounded rate is
Rcc, is given by:
HPRT = eRcc×T – 1


### Normal and lognormal distribution

**Continuous compounding** equation is as follows:
$$EAR_{cont} = e^{r}-1$$
where EAR = effective annual rate; e: mathematical constant; r: continuous rate

$$FV = PV \times e^{rN}$$
where FV: future value; PV: present value; r: continuous rate

Price relatives or 1+HPR:
$$\frac{FV}{PV} = e^{rN}$$
$$ln(\frac{FV}{PV})=rN$$

> A stock was purchased for $100 and sold one year later for $120. Calculate the investor’s annual rate of return on a continuously compounded basis.
>
>Answer: $$ln(\frac{120}{100}) =18.232\%$$
>If we had been given the return (20%) instead, the calculation is: $$ln(1 + 0.20) = 18.232\%$$

As asset never comes down below 0, the price relative can never be below 0.

If natural log of Y is normal, Y is a lognormal distribution.

> The continuously compounded rate of return that will generate a one-year holding period return of -6.5% is _closest_ to -6.7%.
> Continuously compounded rate of return = ln(1 – 0.065) = -6.72%.

> Over a period of one year, an investor's portfolio has declined in value from 127,350 to 108,427. What is the continuously compounded rate of return? 
> The continuously compounded rate of return = ln(S1 / S0) = ln(108,427 / 127,350) = –16.09%.


## Monte Carlo Simulation
### What is monte carlo simulation?
- **Monte Carlo Simulation** is a technique based on the repeated generation of one or more risk factors that affect security values, in order to generate a distribution of security values.
- For each of the risk factors, the analyst must specify the parameters of the probability distribution that the risk factor is assumed to follow. 
- A computer is then used to generate random values for each risk factor based on its assumed probability distributions. 
- Each set of randomly generated risk factors is used with a pricing model to value the security
- This procedure is repeated many times (100x, 1,000x, or 10,000x), and the distribution of simulated asset values is used to draw inferences about the expected (mean) value of the security and possibly the variance of security values about the mean as well.

### Example of monte carlo simulation
As an example, consider the valuation of stock options that can only be exercised on a
particular date. The main risk factor is the value of the stock itself, but interest rates
could affect the valuation as well. The simulation procedure would be to:
1. Specify the probability distributions of stock prices and of the relevant interest
rate, as well as the parameters (mean, variance, possibly skewness) of the
distributions.
2. Randomly generate values for both stock prices and interest rates.
3. Value the options for each pair of risk factor values.
4. After many iterations, calculate the mean option value and use that as your
estimate of the option’s value.

### Usage of monte carlo simulation
- Value complex securities.
- Simulate the profits/losses from a trading strategy.
- Calculate estimates of value at risk (VaR) to determine the riskiness of a portfolio of assets and liabilities.
- Simulate pension fund assets and liabilities over time to examine the variability of the difference between the two. 
- Value portfolios of assets that have nonnormal returns distributions.

---
## Questions before starting this section:
- [ ] what is shortfall risk?
- [ ] what is safety-first ratio?
- [ ] why asset prices are lognormal and when should we use normal? (how to identify the phases?)
- [ ] how to do monte carlo stimulation?

## Codes to test understanding of objectives
1. Do Monte-Carlo stimulation of a portfolio
2. Understand the confidence interval and understand the z-values
3. Calculate the shortfall risk of 2 funds from money box.
4. https://www.scribbr.com/frequently-asked-questions/what-is-a-normal-distribution/