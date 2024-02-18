# 3 - Probability concepts
202209141330
Status: #📥 
Tags: [[CFA Level I]]

## Objectives:
- [x] define a random variable, an outcome, and an event.
- [x] identify the two defining properties of probability, including mutually exclusive and exhaustive events, and compare and contrast empirical, subjective, and a priori probabilities.
- [x] describe the probability of an event in terms of odds for and against the event.
- [x] calculate and interpret conditional probabilities.
- [x] demonstrate the application of the multiplication and addition rules for probability.
- [x] compare and contrast dependent and independent events.
- [x] calculate and interpret an unconditional probability using the total probability rule.
- [x] calculate and interpret the expected value, variance, and standard deviation of random variables.
- [ ] explain the use of conditional expectation in investment applications.
- [x] interpret a probability tree and demonstrate its application to investment problems.
- [x] calculate and interpret the expected value, variance, standard deviation, covariances, and correlations of portfolio returns.
- [x] calculate and interpret the covariances of portfolio returns using the joint probability function.
- [x] calculate and interpret an updated probability using Bayes’ formula.
- [x] identify the most appropriate method to solve a particular counting problem and analyse counting problems using factorial, combination, and permutation concepts.

## Review:
- [ ] calculate and interpret an updated probability using Bayes’ formula.
- [ ] identify the most appropriate method to solve a particular counting problem and analyse counting problems using factorial, combination, and permutation concepts.
- [ ] define a random variable, an outcome, and an event.
- [x] describe the probability of an event in terms of odds for and against the event.
- [ ] demonstrate the application of the multiplication and addition rules for probability.
- [ ] calculate and interpret an unconditional probability using the total probability rule.
- [ ] calculate and interpret the variance and standard deviation of random variables.
- [ ]  calculate and interpret the expected value, variance, standard deviation, covariances, and correlations of portfolio returns (weighting problems) and 
- [ ] calculate expected returns of portfolio - (reminder: weightings) 
- [ ] covariance of probability calculation
- [ ] Odds for

---

## Codes to test understanding of objectives
1. Understand the correlation between two stocks
2. Understand the expected portfolio return with stock, bonds, properties and commodities in an economic upturn vs downturn.
3. Calculate something from Bayesian formula, 

## From past statistics to predict the future  
- From the past parameter to make inferences of probability of success or failure, to make decisions base on logic, probability and statistics
- **Random variable** - uncertain quantity or number (eg. monthly return of asset A)
- **Outcome** - observed value of a **random variable**
- **Event** - a single or a set of **outcomes**
- **Mutually exclusive events** - can't happen at the same time
- **Exhaustive events** - include all possible outcomes ($\sum$all possible outcome = 1)

## Defining properties of probability
1. If a set of events are **mutually exclusive** and **exhaustive**, the sum of their probabilities is equal to 1 (i.e. $P(E_1)+P(E_2)+...+P(E_n) = 1$)
2. The probability of any event is between **0** and **1**. (i.e. $0 \le P(E_i)\le1$), where 0 means event E will never happen, and 1 means even E will surely happen; outcome is not random.

### How do we determine probability?
There are 3 major ways of determining probability:
- **Subjective** - Personal judgement, it is the least formal method
- **Empirical** - analyse past data (objective)
- **A priori** - formal reasoning and inspection process (not through data) (objective)

### Odds
**Odds for** are the number of occurrence for every non-occurrence

**Odds for** are the number of successful possibilities to the number of unsuccessful possibilities:
$$\mathrm {Odds\,For} = \frac{P(E)}{1-P(E)}$$

**Odds against** is the reciprocal of 'odds for'
$$\mathrm{Odds\,Against} = \frac{1-P(E)}{P(E)}$$
eg. The probability of occurrence of the odds for an event is 1-to-6 

$$\frac{1}{1+6}=0.1429=14.29\%$$


### Conditional probability
There are two types of probability:
- **unconditional probability** - 'marginal probability', probability of an event regardless of past or future occurrences of other events. (i.e. $P(A)$, $P(B)$)
- **conditional probability** - where the occurrence of one event affects the probability of another event (i.e. $P(A|B)$) (i.e. one thing happens then another thing would happen)
	- the probability of A occurring given that B has occurred is $P(A|B)$

### Dependent and independent events
**Independent** events refers to events for which the occurrence of one has no influence on the occurrence of the others (i.e. If A and B are independent, the occurrence of B will not affect A)
- it can be expressed in terms of conditional probability 
- eg. $P(A|B)=P(A)$ or equivalently $P(B|A) = P(B)$


### Joint probability
**Joint probability** is the probability of two events that they will both occur
- it is also known as the **multiplication rule of probability** **('and')**
$P(AB)= P(A\cap B)=P(A\,and\,B)=P(A|B) \times P(B)$ if the events are not independent to each other; 
if the events are independent, you should use $P(AB)= P(A\cap B)=P(A\,and\,B)=P(A) \times P(B)$ 

- **addition rule of probability** is used to determine the probability that **at least** one of the two events will occur **('or')**
$P(A\,or\,B) = P(A)+P(B)-P(A\,and\,B)$
or it's the same as $P(A \cup B) = P(A) + P(B) - P(A \cap B)$

If the two events are mutually exclusive, $P(A \cup B) = P(A) + P(B) - 0$, as $P(A\,and\,B)$ will be 0.

### Total probability
The **total probability rule** is used to determine the unconditional probability of an event given conditional probabilities
$P(A) = P(A|B_1)P(B_1) + P(A|B_2)P(B_2) + ... + P(A|B_n)P(B_n)$,
where the sets of events are mutually exclusive and exhaustive

### Probability rules must remember:
- If A and B are independent, the occurrence of B will not affect A. Hence P(A|B) = P(A).
- Since P(A|B) = P(A), substitute this into the multiplication rule and we get joint probability P(AB) = P(A) x P(B).
- The simplified addition rule P(A or B) = P(A) + P(B) is only valid for mutually exclusive pairs.
- P(A) + P(B) is only valid for mutually exclusive and exhaustive pairs.

## Expected values and variance
**Expected values** are forecast based on historical statistics value inference. Expected outcomes weighted by the probability of outcome.

The **expected value** equation is as follows:
$$E(X) = \sum{P(X_i)X_n} = P(X_1)X_1 + P(X_2)X_2 + ... +P(X_n)X_n$$
where $X_i$ can be in $ or percentage %.

The **probabilistic variance** is as follows:
$$\sigma^2E(X) = \sum{P(X_i)}[X_i-E(X)]^2$$
when it's weighted there's no need to divide by $n-1$ or $n$ as it's already weighted

![[Screenshot 2022-09-15 at 16.44.33.png]]
where both *variance* and *standard deviation* is used to measure the dispersion of a random variable around its expected value, sometimes, it's referred as **volatility**.


Expected value can also be made under an assumption:
$$E(X|S) = \sum{P(X|S)}X_i$$
- given that the probability is exhaustive and mutually exclusive

![[Screenshot 2022-09-15 at 17.29.07.png]]

Unconditional expected value of EPS:
$$E(X)=E(X|R)P(R)+E(X|R^C)P(R^C)$$

![[Screenshot 2022-09-16 at 15.13.28.png]]

## Portfolio return and variance
There are some of the metrics to calculate for the portfolio:
- portfolio return
- portfolio variance

Understand the **expected return** of multiple variables with multiple weights.
$$E(w_xX+w_yY) = w_xE(X)+w_yE(Y)$$

eg. 2-asset investment portfolio

| Asset | Weight | Expected Return|
|----|----|----|
| X | $w_x$ | $E(X)$ |
| Y | $w_y$ | $E(Y)$ |

where $w_x + w_y = 1$, and the return are often not independent as it's in the financial market and is expected to have some degree of influence on each other.

### Joint Probability Table

![[Screenshot 2023-06-24 at 13.37.13.png]]

Since they are not independent, we have to consider the covariance.

### Covariance
Properties of **covariance**:
1. General representation of variance
2. The covariance of a random variable with itself is the variance of the variable ( i.e. $Cov(X,X) = Var(X)$)
3. Covariance can range from $-\infty$ to $+\infty$
4. If there is a positive covariance between the random variables, when one of the random variable is above its mean, the other random variable *tends to be* above its mean, and *vice versa*.

$$Cov(X,Y) = \sum{E{[X-E(X)][Y-E(Y)]}}$$
where E: expectation/probability of the event happening

### Correlation
**Correlation** is a standardised measure of which whether two products move together.

Interpretation of correlation:
$\mathrm{Corr}(X,Y) = -1$ means negative linear relationship
$\mathrm{Corr}(X,Y) = 0$ means no linear relationship
$\mathrm{Corr}(X,Y) = 1$ means positive linear relationship

**Correlation** is the covariance divided by the product of the 2 standard deviations, the equation is as follows:
$$\mathrm{Corr}(Y,X) =\mathrm{Corr}(X,Y) = \frac{\mathrm{Cov}(X,Y)}{\sqrt{\sigma^2(X)}\sqrt{\sigma^2(Y)}}=\frac{\mathrm{Cov}(X,Y)}{\sigma(X)\sigma(Y)}$$
where $\sigma^2$ is the variance of asset X or Y respectively.

## Variance of the portfolio
Variance of the portfolio is the sum of the average squared deviation of the mean of asset X and asset Y with their respective weight and the covariance for each asset.

Variance of the 2-assets portfolio of X and Y:
$$\sigma^2(w_xX+w_yY) = {w_x}^2\sigma_x{^2} + {w_y}^2\sigma_y{^2}  + 2 {w_x}{w_y}Cov_{x,y}$$
where **Note**: $Cov(X,Y)$ = $ρ_{x,y} \times σ_x \times σ_y$; where ρ = correlation between assets 1 and 2
The sum of the weighted variance of each asset plus the covariance of two assets (1 covariance for each asset, so in total of **2** in $2 {w_x}{w_y}Cov(X,Y)$, as they are not independent from each other.  

Variance of 3-assets portfolio of X, Y and Z:
$$
\displaylines{\sigma^2(X,Y,Z)= {w_x}^2\sigma_x{^2}+{w_y}^2\sigma_y{^2}+
{w_z}^2\sigma_z{^2}\\+2w_xw_yCov_{x,y}+2w_xw_zCov_{x,z}+2w_yw_zCov_{y,z}}$$

At last, **to convert into standard deviation**:
$$\sigma=\sqrt{\sigma^2}$$
where $\sigma$: standard deviation; $\sigma^2$: variance.

![[Screenshot 2023-06-24 at 13.43.12.png]]

### Covariance matrix
The **covariance matrix**:
- shows the covariances between returns on a group of assets

![[Screenshot 2022-09-16 at 19.01.54.png]]


## Bayes' formula
**Bayes' formula** is used to update a given set of prior probabilities for a given event in response to the arrival of new information

The **bayes' rule** for updating prior probability of an event is:
$$\mathrm{Updated\,probability = \frac{Probability\,of\,new\,information\,for\,a\,given\,event}{Unconditional\,probaility\,of\,new\,information} \times Prior\,probability\,of\,event}$$

We can derive Bayes' formula using the multiplication rule and noting that $P(AB)=P(BA)$
Since that's the case, $P(AB) = P(A|B) \times P(B)$ and $P(BA) = P(B|A) \times P(A)$, therefore
$P(A|B)\times P(B)=P(B|A)\times P(A)$

$$P(A|B)=\frac{P(B|A)\times P(A)}{P(B)}$$

$$\mathrm{P(Event|Info)=\frac{P(Info|Event)\times P(Event)}{P(Info)}}$$

where the event is unknown, and info is the new information given.
The information might require addition rule and total probability rule from the decision tree, as to add up all the possibility.

![[Screenshot 2023-06-24 at 13.49.57.png]]
![[Screenshot 2023-07-14 at 12.53.28.png]]
![[Screenshot 2023-07-14 at 12.53.51.png]]
![[Screenshot 2023-07-14 at 12.53.44.png]]

## Principle of counting 
- help to determine the *total number of possibilities* in a problem
- labelling refers to the situation where there are $n$ items and that each can receive $k$ different labels

### Multiplication rule of counting
- multiplication rule is used for calculating the total number of possibilities by multiplying the number of possibilities in each step.

### Factorial

$$n\times(n-1)\times(n-2)\times\dots\times1=n!$$

### Multinomial Formula (Labeling)
**Multinomial formula** is used when $n$ items are **all** distributed into $k$ groups  (i.e. $n_1 + n_2 + ... + n_k = n$)
The **multinomial formula** is as follows:
$$\mathrm{Number\,of\,Ways\,of\,Assigning} = \frac{n!}{n_1!n_2!\dots n_k!}$$
where $n$: the number of random variable in each group; $k$: labels; can think of it as boxes that need to be filled completely and no left overs.

⇒labelling refers to the situation where there are $n$ items and that each can receive $k$ different labels; the number of labels receives label 1 is $n_1$ and the number that receive label 2 is $n_2$ and so on...

![[Screenshot 2022-10-12 at 14.44.58.png]]

If there are $n$ labels $(k=n)$, we have $\frac{n!}{1} = n!$. The number of ways to assign $n$ different labels to $n$ items is $n!$.

![[Screenshot 2023-06-24 at 13.53.06.png]]

### Combination Formula/ binomial formula
- 'n choose r'
- sequence is **not important**
- there are items that are left-over and not chosen
- when the number of labels equals to 2 (i.e. $k$ = 2); that is $n$ items can only be in one of the 2 groups, and $n_1+n_2 = 1$. Since there're only two categories, then the $r = n_1$ and $n-r = n_2$; where $r$ items is being chosen, and $(n-r)$ items are not chosen.

The general formula expressing this is:
$$\mathrm{nCr} = \frac{n!}{r!(n-r)!}$$
where $nCr$ is the number of possible ways (combinations) of selecting $r$ items from a set of $n$ items when the order of selection is not important; and think of it as there are left-overs.

![[Screenshot 2022-10-12 at 14.45.18.png]]

### Permutation Formula
- there are items that are left-over and not chosen
- where the sequence is **important**

A permutation formula is a specific ordering of a group of objects. The question of how many different groups of size $r$ in specific order can be chosen from $n$ objects is answered by the permutation formula.

The number of permutations of $r$ objects from $n$ object is:
$$\mathrm{nPr} = \frac{n!}{(n-r)!}$$

The permutation formula implies that there are $r!$ more ways to choose $r$ items if the order of selection is **important**. i.e.:

$$\mathrm{nPr} = r! \times \mathrm{nCr}$$

![[Screenshot 2022-10-12 at 14.45.33.png]]

## Guidelines to determine the counting method
Five guidelines may be used to determine which counting method to employ when dealing with counting problems:

- The **multiplication rule of counting** is used when there are ***two or more groups***. The key is that only one item may be selected from each group. If there are $k$ steps required to complete a task and each step can be done in $n$ ways, the number of different ways to complete the task is $n_1 × n_2 × … × n_k$.

- *Factorial* is used by itself when there are no groups—we are only arranging a given set of $n$ items. Given $n$ items, there are $n!$ ways of arranging them.

- The **labeling formula** applies to ***three or more subgroups*** of predetermined size. Each element of the entire group must be assigned a place, or label, in one of the three or more subgroups.

- The **combination formula** applies to ***only two groups of predetermined size***. Look for the word “choose” or “combination” or "select".

- The **permutation formula** applies to ***only two groups of predetermined size***. Look for a specific reference to “order” being important.

---
## Questions before starting this section:
- [ ] what are empirical, subjective, and a priori probabilities?
- [ ] how to base on past performance to predict future probabilities?
- [ ] what are the limitations in each type of probability prediction?
- [ ] how to yield to higher probability of success in analysing the market?
- [ ] what is updated probability using bayes'?
- [ ] how do we understand the probability of a stock going up or down, according to the elliot wave structure?
- [ ] what is the variance of more than two assets?
- [ ] what is the expected return for more than two assets?
- [ ] how do we find the joint probability table? or how to calculate?