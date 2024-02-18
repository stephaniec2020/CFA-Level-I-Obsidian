# 49 - Portfolio risk and return I
202304292245
Status: #📥 
Tags: [[CFA Level I]]

## Objectives:
- [ ] calculate and interpret major return measures and describe their appropriate uses.
- [ ] compare the money-weighted and time-weighted rates of return and evaluate the performance of portfolios based on these measures.
- [ ] describe characteristics of the major asset classes that investors consider in forming portfolios.
- [ ] calculate and interpret the mean, variance, and covariance (or correlation) of asset returns based on historical data.
- [ ] explain risk aversion and its implications for portfolio selection.
- [ ] calculate and interpret portfolio standard deviation.
- [ ] describe the effect on a portfolio’s risk of investing in assets that are less than perfectly correlated.
- [ ] describe and interpret the minimum-variance and efficient frontiers of risky assets and the global minimum-variance portfolio. explain the selection of an optimal portfolio, given an investor’s utility (or risk aversion) and the capital allocation line.

---

## Return measures
Financial assets normally generate **two types of return for investors**:
- periodic income through interest or dividend payments
- a capital gain or loss when the asset is sold or redeemed

### Single period
**Single period returns** have only one way to calculate, through **holding period return (HPR)**, the return earned from holding an asset for a specified period of time.


**The holding period of return (HPR)** formula is as follow:
$$\mathrm{HPR = \frac{P_1+CF}{P_0}-1}$$
where $P_1$: Ending value; $P_0$: Beginning value; CF: cash flow received

If the period is not exactly one year, the figure can be annualised by using these formulas, depending on the number of years, months or days in each period:

Annualise to number of years:
$$\mathrm{(1+HPR)^{1/num.\,of\,yrs}-1}$$
Annualise to number of months:
$$\mathrm{(1+HPR)^{12/num.\,of\,months}-1}$$
Annualise to number of days:
$$\mathrm{(1+HPR)^{365/num.\,of\,days}-1}$$

However, if there are multiple cash inflows and outflows going into the portfolio during the period, this approach will not work.

### Multiple periods
The correct approach should be to break up the returns into multiple periods of the same length, **calculate the holding period (HPR)** for each period, and then **calculate the average returns per period**.

![[Screenshot 2023-05-01 at 01.17.37.png]]

![[Screenshot 2023-05-01 at 01.17.05.png]]
There are several approaches to determine this average return:
- **arithmetic mean return**
- **geometric mean return**
- **the money weighted return**

#### Arithmetic mean return
The **arithmetic mean return** is simply the simple average, which is to sum all the periodic returns and divide by the number of periods it has the statistical property of being an **unbiased estimate of the true mean** of the underlying distribution of returns.

$$\mathrm{Arithmetic\,mean\,return=\frac{\sum R_n}{n}}$$
The **arithmetic mean shortcoming** is that it can be **upwardly skewed by large positive gains**.

#### Geometric mean return
The **geometric mean return** provide a **more accurate representation of the growth** in portfolio value over a given time period than does an arithmetic mean return since it accounts for the **compounding rates of returns over multiple periods**, multiply all the returns.

The equation of **geometric mean** is as follows: 
$$G = \sqrt[n]{(X_1 \times X_2 \times ... \times X_n)}$$
where G: geometric mean

**Note**: it can only be calculated if the products are non-negative

Geometric mean of return/growth, $R_{G}$ is as follows:

$$1+R_{G} = \sqrt[n]{[(1+R_{1})\times(1+R_{2})\times...\times(1+R_{n})]}$$

![[Screenshot 2023-05-01 at 01.44.02.png]]
![[Screenshot 2023-05-01 at 01.51.35.png]]

#### Market weighted rate of return (MWRR)
**Market weighted rate of return (MWRR)** is the same as internal rate of return (IRR) based on portfolio's cash flow, which means it is the **discount rate** that equates all the cash inflows with all the cash outflows.
$$\mathrm{MWRR = IRR}$$
which is clearly not the best way in measuring the performance, it is affected by the amount of cash inflow and outflow
**Note**: The final cash flow (CF) should add the inflow and the residual amount in the account

$$\mathrm{NPV = \sum_{t=0}^n\frac{CF_t}{(1+r)^t}}$$
$$\mathrm{NPV = \frac{CF_0}{(1+r)^0}+\frac{CF_1}{(1+r)^1}+\frac{CF_2}{(1+r)^2}+\frac{CF_3}{(1+r)^3}}$$
where CF: cash flow; r: internal rate of return; t: time period cash flow.
However, this question is typically difficult to solve, therefore, calculator is used to calculate IRR.

![[Screenshot 2023-05-01 at 01.51.50.png]]

### Other measures
**Unrealised gains**, **realised capital gains** and **dividends received** constitute the **total returns** to an investor.
The **total return** equation is as follows:
$$\mathrm{Total\,return=Unrealised\,gains+Realised\,gains+Dividends}$$
which **dividend income** and **realised capital gains** are often **subject to ta**x, so part of the returns go to the government.

The **gross return** **do not include commission and trade expense** as those belong to the brokerage. The **net return** is the return after management fees.

**Pre-tax nominal return** refers to the return prior to paying taxes and after tax nominal return refers to the return after the tax liability is deducted.

Lastly, **nominal returns** can be considered to be made up of **real returns** and an **inflation** adjustment.

![[Screenshot 2023-05-01 at 01.54.13.png]]

>Seiko bought a mutual fund with an annual 2% management fee. He paid a 0.8% commission to his broker. After 1 year, Seiko sold the funds at a gross return of +15.3%. He was taxed 30% on the gains. His after-tax nominal returns is closest to:
>
>Commissions/trade expenses are not included in gross returns. 
>Pre-tax returns = 15.3% – 2% = 13.3%  
>After-tax returns = 13.3 x 0.7 = 9.31%

**Real returns** measures the increase in an investor's purchasing power, that is, how much more goods can the investor purchase at the end of one year due to the increase in the investment value?

The formula to calculate the real return is this:
$$\mathrm{Real\,return=\frac{(1+Nominal\,return)}{(1+Inflation\,rate)}-1}$$

### Leveraged return
**Leveraged return** is common and derivative and real estate investments where some investors purchase on margin as the portfolio is **partly financed through debt**. The **actual cash outlay by the investor is lower than the portfolio value**.

When the portfolio value increases, the proportion of increase based on the cash outlay by the investor is larger and this is known as the **leveraged return**.

The **leveraged returns** should take into account the **cost of financing the loan**,**management fees**, **admin fees and commissions and trading fees** and will be covered in detail of complete equity investment course.

![[Screenshot 2023-05-01 at 01.58.56.png]]

## Market weighted rate of return (MWRR)
**Market weighted rate of return (MWRR)** is the same as **internal rate of return (IRR)** based on portfolio's cash flow, which means it is the **discount rate** that equates all the cash inflows with all the cash outflows.
$$\mathrm{MWRR = IRR}$$
which is clearly not the best way in measuring the performance, it is affected by the amount of cash inflow and outflow
**Note**: The final cash flow (CF) should add the inflow and the residual amount in the account

$$\mathrm{NPV = \sum_{t=0}^n\frac{CF_t}{(1+r)^t}}$$
$$\mathrm{NPV = \frac{CF_0}{(1+r)^0}+\frac{CF_1}{(1+r)^1}+\frac{CF_2}{(1+r)^2}+\frac{CF_3}{(1+r)^3}}$$
where CF: cash flow; r: internal rate of return; t: time period cash flow.
However, this question is typically difficult to solve, therefore, calculator is used to calculate IRR.

![[Screenshot 2022-10-10 at 16.15.07.png]]

## Holding period return (HPR)
It can be used to calculate from the beginning and ending value with the cash flow (i.e. coupon and dividend).

**The holding period of return (HPR)** formula is as follow:
$$\mathrm{HPR = \frac{P_1+CF}{P_0}-1}$$
where $P_1$: Ending value; $P_0$: Beginning value; CF: cash flow received

When there's unequal cash flow in and out of the account the HPR should be calculated for each time period and the summation of all periods to get the final HPR.

![[Screenshot 2022-10-10 at 16.15.28.png]]

## Time weighted rate of return (TWRR)
**Time weighted rate of return (TWRR)** is the most widely used measurement to calculate the portfolio performance across time
**TWRR** is the **geometric mean** of portfolio.

The formula of **time weighted rate of return (TWRR)**  is as follow:
$$TWRR=\sqrt[n]{(1+R_1) \times (1+R_2) \times ... \times (1+R_n)}$$
where $R_{1\,to\,n}$: calculated through the holding period return (HPR) which previously discussed.

>Candice bought 2 bonds at $98 each at t=0, and another bond at $102 at t=1. At t=2, she sold all 3 bonds at $99 each. At t=1 and t=2, she received a coupon of $2 per bond for each period.
> 
> The geometric mean return for each period is closest to: +2.5%
> 
> $R_1$ = (102×2 + 2×2)/(98×2) -1 = +6.12%; where 102 is new price of bond, 98 is old price of bond; 2 is coupon $\times$ amount of bond held
> $R_2$= (99×3 + 2×3)/(102×3) -1 = -1%; where 99 is new price of bond, 102 is old price
> 
> Geometric mean return = (1.0612 x 0.99)^.5 – 1 = +2.5%



#### Practice question:
![[Screenshot 2022-10-10 at 16.35.36.png]]
![[Screenshot 2022-10-10 at 16.36.13.png]]

## Summary of MWRR, HPR, TWRR
The summary of ways of calculating portfolio return:
- **Market weighted rate of return (MWRR)** - MWRR = IRR, use CF to calculate
- **Holding period return (HPR)** - New + CF/ Old - 1
- **Time weighted rate of return (MWRR)** - Computes all the HPR and find geometric mean

![[Screenshot 2022-10-10 at 16.36.42.png]]

## Expected returns and standard deviation of returns
### Asset risk and returns
Given the price history of an asset, there are various ways (e.g. **arithmetic mean, geometric mean, money-weighted**) to calculate the **average return of the asset**, which can be an estimate of the **expected returns of the asset**.

The other important aspect to study is the **risk** of an asset. There are various ways to estimate this, but perhaps the most widely adopted way is to calculate the **standard deviation or returns** based on the assets price history.

**Population standard deviation**: $$\sigma = \sqrt\frac{\sum(X-\mu)^2}{N}$$
**Sample standard deviation** (an estimate of population standard deviation):
$$s = \sqrt\frac{\sum(X-\bar{X})^2}{n-1}$$
where $\bar{X}$ is the sample mean, and $n$ is the sample population.
The denominator is $n-1$, and it allows us to have unbiased estimate
The sample standard deviation can be interpreted as the unbiased estimator of the population standard deviation, $\sigma$.

#### Analysis of US market in 1926 to 2008
![[Screenshot 2023-05-03 at 18.40.58.png]]
We can observe that as the average return increases, the standard deviation of returns also increases. i.e. small cap stocks have had the greatest average returns and greatest risk, while t bills have the lowest average returns and the lowest risk, they supports the idea of a **trade off between risk and return**.

#### Limitations of expected return and risk estimates
Average returns give us an estimate of an assets, expected returns, and its standard deviation gives us an estimate of the risk.
However, there are limitations of this approach:
- **assumption that asset returns follow normal distribution** (actual return is negatively skewed (tendency towards large downside deviation) and higher kurtosis (frequent extreme deviations on both the upside and downside))
- **does not consider liquidity of asset** - lower liquidity ⇒ lower selling price ⇒ lower expected return (especially in emerging market securities, low quality corporate bond)

### Portfolio risks and returns
#### Portfolio returns
**Portfolio weighted average return**, the expected return of two-asset portfolio is simply the weighted average return of the two assets.

The expected return of two asset portfolio is as follows:
$$E(w_xR_x+w_yR_y) = w_xR_x+w_yR_y$$
where E: expected; R: return; w: weight; X and Y: asset X and asset Y; the expected portfolio return of asset X and Y is equals to the sum of expected value of weighted asset X + weighted expected value of Y.

eg. started off with 2-asset investment portfolio
|Asset|Weight|Expected Return|
|------|-------|----------------|
|X|$w_x$|$R_x$|
|Y|$w_y$|$R_y$|

where $w_x + w_y = 1$, and the return are often not independent as it's in the financial market and is expected to have some degree of influence on each other.

#### Portfolio variance
The **portfolio variance** measures **how spread out the returns** of the investments in the portfolio are from their average return. Portfolio variance is calculated by **taking the weighted average of the variances** of the individual investments in the portfolio, where the weights are the proportions of each investment in the portfolio and **standard deviation is the square root of variance**.

Variance of the 2-asset portfolio of X and Y:
$$\sigma^2(X+Y) = {w_x}^2\sigma_x{^2} + {w_y}^2\sigma_y{^2}  + 2 {w_x}{w_y}Cov_{x,y}$$
where **Note**: $Cov_{x,y}$ = $ρ_{x,y} \times σ_x \times σ_y$; where ρ = correlation between assets 1 and 2
The sum of the weighted variance of each asset plus the covariance of two assets (1 covariance for each asset, so in total of **2** in $2 {w_x}{w_y}Cov(X,Y)$, as they are not independent from each other.  

Substituting the covariance portion of asset X and Y, this 2-asset portfolio of X and Y variance is more commonly used:
$$\sigma^2(X+Y) = {w_x}^2\sigma_x{^2} + {w_y}^2\sigma_y{^2}  + 2 {w_x}{w_y}\rho_{x,y}(\sigma_x\sigma_y)$$

Variance of 3-asset portfolio of X, Y and Z:
$$
\displaylines{\sigma^2(X,Y,Z)= {w_x}^2\sigma_x{^2}+{w_y}^2\sigma_y{^2}+
{w_z}^2\sigma_z{^2}\\+2w_xw_yCov_{x,y}+2w_xw_zCov_{x,z}+2w_yw_zCov_{y,z}}$$

At last, to convert into standard deviation:
$$\sigma=\sqrt{\sigma^2}$$
where $\sigma$: standard deviation; $\sigma^2$: variance.

![[Screenshot 2023-05-03 at 19.07.19.png]]

### Covariance and correlation
**Covariance** between two variables is a measure of the degree to which the two variables tend to move together. However, it is difficult to interpret as the covariance is not normalised, hard to make sense of its magnitude (unbounded to the end, has -$\infty$ to +$\infty$ , and the unit is in returns$^2$. For these reasons, most practitioners prefer to use a standardised measure called the correlation coefficient. 

### Covariance
**Covariance** between two variables is a measure of the degree to which the two variables tend to move together. Covariance has ranges from -$\infty$ to +$\infty$; that is $-\infty \le Cov_{x,y} \le +\infty$
There are 3 main category of covariance:
- **Positive covariance** - indicates that the variables **tend to move together**
- **Negative covariance** - indicates that the variables tend to move in **opposite directions** 
- 0 covariance - no linear relationship between the variables

The formula of **covariance** is as follows: $$\mathrm{covariance}=Cov_{x,y} = \frac{\sum|(X-\bar{X})(Y-\bar{Y})|}{n-1}$$
where $n$: number of periods
**Note:** variance of one variable - the covariance is with itself

Negative covariance means rates of return for one security will tend to be above its mean return in periods when the other is below its mean return, and vice versa. Positive covariance means that returns on both securities will tend to be above (or below) their mean returns in the same time periods. For the returns to always move in opposite directions, they would have to be perfectly negatively correlated. Negative covariance by itself does not imply anything about the strength of the negative correlation, it must be standardised by dividing by the product of the securities' standard deviations of return.

#### Correlation 
**Correlation** is a measure of the strengths of the *linear* relationship of two random variables.
- correlation has no units
- correlation ranges from -1 to +1, that is $-1 \le r_{xy} \le +1$

In order to calculate correlation, one must calculate the covariance first.
The formula of **correlation coefficient** is as follows:
$$\mathrm{correlation} = \rho_{x,y} = \frac{Cov_{x,y}}{(\sigma_x\sigma_y)} = \mathrm{\frac{covariance}{products\,of\,std.dev.}}$$
correlation is a standardised measure of which whether two products move together.
where correlation:
$\rho_{xy} = -1$ means negative linear relationship (perfect negative correlation)
$\rho_{xy} = 0$ means no linear relationship (uncorrelated)
$\rho_{xy} = 1$ means positive linear relationship (perfect positive correlation)

From rearranging the equation, the **covariance** of asset X and Y is as follows:
$${Cov_{x,y}} = \rho_{x,y} {(\sigma_x\sigma_y)}$$
where covariance = correlation of asset X and asset Y $\times$ products of standard deviations of asset X and asset Y.

## Theory of portfolio diversification
The theory of portfolio diversification is based on the idea that by **investing in a mix of assets with low or negative correlations**, an investor **can reduce the overall risk** of their portfolio while still achieving a desirable level of return.

The **portfolio variance** of 2-asset portfolio is as follows:
$$\sigma^2(X+Y) = {w_x}^2\sigma_x{^2} + {w_y}^2\sigma_y{^2}  + 2 {w_x}{w_y}\rho_{x,y}(\sigma_x\sigma_y)$$

and the **standard deviation** of the 2-asset portfolio is the square root of variance:
$$\sigma(X+Y) = \sqrt{{w_x}^2\sigma_x{^2} + {w_y}^2\sigma_y{^2}  + 2 {w_x}{w_y}\rho_{x,y}(\sigma_x\sigma_y)}$$

The **standard deviation of returns** are used to **estimate the portfolio risk**.

We can infer that the **standard deviation** of the portfolio is a function of:
- the **standard deviations of the assets** that make up the portfolio
- their **respective weights** in the portfolio
- **correlation of returns between the two assets**

![[Screenshot 2023-05-03 at 23.40.04.png|500]]

### Scenarios to understand the correlation aspects in portfolio
**In perfectly positively correlated assets**, the $\rho_{x,y}$ = +1.0.

When substituted the correlation ($\rho_{x,y}$) as +1: 
$$\sigma(X+Y) = \sqrt{{w_x}^2\sigma_x{^2} + {w_y}^2\sigma_y{^2}  + 2 {w_x}{w_y}\rho_{x,y}(\sigma_x\sigma_y)}$$
$$= \sqrt{{w_x}^2\sigma_x{^2} + {w_y}^2\sigma_y{^2}  + 2 {w_x}{w_y}(\sigma_x\sigma_y)}$$
$$= \sqrt{({w_x}^2\sigma_x{^2} + {w_y}^2\sigma_y{^2})^2}$$
$$= {w_x}^2\sigma_x{^2} + {w_y}^2\sigma_y{^2}$$
$$=0.375^2\times25{^2} + 0.625^2\times 15{^2}=18.75\%$$
which is the weighted average of standard deviation, which is 18.75% in this case.

The portfolio return is:
$$E(w_xR_x+w_yR_y) = w_xR_x+w_yR_y$$
$$= 0.375\times 12 + 0.625\times 6 = 8.25\%$$
The portfolio return is 8.25%.

#### Relationship of return and standard deviation if assets are perfectly positively correlated
![[Screenshot 2023-05-03 at 23.49.01.png]]

#### Relationship of return and standard deviation if assets are perfectly negatively correlated

![[Screenshot 2023-05-03 at 23.53.32.png|300]]

**In perfectly negatively correlated assets**, the $\rho_{x,y}$ = -1.0. 
When substituted the correlation ($\rho_{x,y}$) as -1: 
$$\sigma(X+Y) = \sqrt{{w_x}^2\sigma_x{^2} + {w_y}^2\sigma_y{^2}  + 2 {w_x}{w_y}\rho_{x,y}(\sigma_x\sigma_y)}$$
$$= \sqrt{0.375^2\times25{^2} + 0.625^2\times 15{^2}  + 2 \times 0.375\times0.625\times(-1)\times25\times 15}$$
$$=0\%$$

The standard deviation is really zero. If you're able to find two assets that are really **perfectly negatively correlated**, you can create a portfolio with zero risk while the portfolio return remains the same at 8.25%.

![[Screenshot 2023-05-03 at 23.51.22.png]]

In fact, if you start with a portfolio that's 100% in assets 2, you and slowly add on an allocation into asset 1, you'll find that the risk return of the portfolio follows this line. This continues until the optimal allocation where the risk is zero and the risk return increases as you continue to add on until the allocation is 100% in asset 1.

### Diversification through low correlation between assets
These two extreme examples serve to highlight one important principle. The **lower the correlation between the assets in a portfolio, the lower the risk of the portfolio**. This theory illustrates the **benefit of diversification**.

![[Screenshot 2023-05-03 at 23.55.06.png]]

#### Relationship of return and standard deviation if assets are with no correlation
In **zero correlation** between the assets, which is more practical, the $\rho_{x,y}$ = 0.0.

The portfolio standard deviation when no correlation:
When substituted the correlation ($\rho_{x,y}$) as 0: 
$$\sigma(X+Y) = \sqrt{{w_x}^2\sigma_x{^2} + {w_y}^2\sigma_y{^2}  + 2 {w_x}{w_y}\rho_{x,y}(\sigma_x\sigma_y)}$$
$$= \sqrt{0.375^2\times25{^2} + 0.625^2\times 15{^2}}=13.3\%$$
The standard deviation for the portfolio is 13.3%.

Again, if we plot the risk return relationship for this case of no correlation between the assets, we get this curve. This allocation is the optimal allocation for these two assets.

This is **lower than the risk of both assets** by themselves. An investor who just wants to put all his money into one safer asset with lower returns, **he may want to consider diversifying some of the money into a riskier asset** **with little correlation to the safer asset**. This not only **increases the expected return**, it also **reduces the portfolio risk**.

![[Screenshot 2023-05-03 at 23.57.48.png]]

### Multi asset portfolio and diversification benefits
In practice, most portfolios comprise several different assets to improve the diversification benefits. For different combinations of allocation weights, we're able to plot the **expected return and standard deviation** on the graph. If we repeat this for many different combinations, we'll probably get something that looks like this.

We find that **at each level of expected return**, there's a portfolio that has the **minimum standard deviation**. The **minimum variance portfolio** is the **lowest risk** amongst a **set percentage of expected return**. All of the minimum variance portfolio make up the **minimum variance frontier**.

![[Screenshot 2023-05-04 at 00.09.07.png]]

#### Risk adverse investors and greatest expected return
Assuming that investors are **risk averse**, such investors prefer the portfolio that has the greatest expected return amongst portfolios that have the same level of risk. These two portfolios have the **same level of risk, but one has a higher expected return than the other**. The risk averse investor will **naturally prefer the portfolio with the higher expected return**. Based on this reasoning, none of the portfolios at the lower half of the minimum variance frontier is optimal for the investor. These portfolios at the top half that have the greatest expected return for each level of risk make up the **efficient frontier**.

A **risk averse investor** would only choose portfolios that are on the **efficient frontier**, especially **the global minimum variance portfolio**, which has the lowest risk amongst all the portfolios.

![[Screenshot 2023-05-04 at 00.15.20.png]]

## Investor's optimum portfolio
### Risk aversion
Simply given that there are two assets that have the same yield. One has lesser risk and the other is risky.

Upon 2 assets with same yield but different levels of risk, **investors** can be:
- **risk neutral** - would be indifferent between the 2 assets
- **risk averse** -  would opt for the risk-free (or less risk) as there is no incentive to take on additional risk
- **risk seeking** - would prefer the risky asset despite both assets having the same expected return, probably anticipation of much higher returns

![[Screenshot 2023-05-04 at 00.27.16.png]]

To convince a **risk averse** investor to **take more risk**, the investor **demands a higher expected return**. If the difference is sufficiently large to compensate the investor for taking on the additional risk, then the investor maybe indifferent between the two assets.

![[Screenshot 2023-05-04 at 00.27.34.png]]

### Indifference curves
The **investor indifference curve** is a graphical representation of an investor's preferences for **different combinations of risk and return** in their investment portfolio. The curve is upward sloping, indicating that as the expected return of the portfolio increases, the investor is willing to accept higher levels of risk.

The investor indifference curve is based on the **assumption** that **investors are rational** and seek to **maximize their utility or satisfaction** from their investment portfolio.

![[Screenshot 2023-05-04 at 00.28.12.png]]

#### Utility and indifference curve
**Utility** in this context is **the satisfaction that the investor derives from an investment**. Even for the same investor, there can be various in **different curves** that represent the **different levels of utility** to the investor.

The investor's expected utility is the same for all points along a single indifference curve.
e.g., if the investor finds two different investments (i.e. portfolio A or portfolio B) that **sit on the same indifference curve**, the investor would have the same level of satisfaction for both and would be **OK to choose either one of them**.

![[Screenshot 2023-05-04 at 00.43.58.png]]

However, if the portfolios (i.e. portfolio A and portfolio B) sit on different indifference curves, the investor will prefer a portfolio A as the satisfaction that she gets from it is higher.

![[Screenshot 2023-05-04 at 00.45.58.png]]

However, it is important to note that the curve is based on assumptions and simplifications, and may not accurately capture the complexity of individual investors' preferences and risk tolerance.

### Capital allocation line
If we extend the analysis to consider all investible risky assets in the market and there are hundreds and thousands of them, we can construct an **opportunity set of investments**, which is all the combinations of portfolios in the market that an investor can invest in.

Likewise, there'll be an **efficient frontier of risky assets**, which represents the set of **most optimal portfolios for each level of return**.

![[Screenshot 2023-05-04 at 00.47.02.png]]

#### Risk-free asset with risky asset portfolio
Most investors have access to a **risk free asset** (i.e. government bonds), and the addition of a risk free asset opens up a new dimension to allow an investor to invest in a portfolio that matches their level of risk aversion.

A **risk free asset has no risk**, so its **standard deviation should be zero** (i.e. $\sigma$ = 0).
The expected return ($E(R)$) is simply the **risk-free rate**.

A portfolio that is 100% invested in a risk-free asset will therefore sit here on the graph. If we combine a risk free asset with a risky portfolio, we get this **straight line**.
Any combination of the risk-free asset and the risky portfolio should lie on this line.

For example, if an investor places 70% of his money in a risk-free asset and 30% in a risky portfolio, this is the expected risk and return to the investor. In fact, this line can extend beyond where the investor **leverages on debt to buy more** (i.e. demonstrated as 140% through leverage). This entire line is called the **capital allocation line**.


![[Screenshot 2023-05-04 at 00.48.00.png]]

Ideally, this line should be as steep as possible, a steeper line means that the investor gets more return per extra unit of risk taken (high Sharpe ratio - _risk-adjusted relative returns_).

The **capital allocation line** is **steepest** when it's **tangential to the efficient frontier**, and it is here where we get the **optimal risky portfolio.**

![[Screenshot 2023-05-04 at 00.53.34.png]]

### Optimal portfolios

There is a portfolio that the **capital allocation line** meets the **investor's utility indifference curve** (in this case, it is moderate utility), this point is the **optimal portfolio** for this particular investor.

Since low utility brings less satisfaction than moderate utility, it's not regarded even though there are portfolios that meet the indifference curve.

![[Screenshot 2023-05-04 at 00.53.54.png]]

The **expected return of risk-free and risky portfolio equation** is as follows:
$$E(w_fR_f+w_rR_r) = w_fR_f+w_rR_r$$
where E: expected; R: returns; w: weight; $R_f$: return of risk-free asset; $R_r$: return of risky assets.

The **standard deviation of risk-free and risky portfolio** equation is as follows:
$$\sigma(F+R) = \sqrt{{w_f}^2\sigma_f{^2} + {w_r}^2\sigma_r{^2}  + 2 {w_f}{w_r}\rho_{f,r}(\sigma_f\sigma_r)}$$
$$= \sqrt{{w_r}^2\sigma_r{^2}} = {w_r}\sigma_r$$
where E: expected; R: returns; w: weight; $R_f$: return of risk-free asset; $R_r$: return of risky assets; where $\sigma_f{^2}$ = 0 because the standard deviation of risk-free asset is 0; $2 {w_f}{w_r}\rho_{f,r}(\sigma_f\sigma_r)$ where  $\sigma_f{^2}$ = 0 due to standard deviation of risk-free asset is 0 and $\rho_{f,r} = 0$ since the correlation between risk-free and risky asset is 0.

![[Screenshot 2023-05-04 at 00.55.19.png]]

### Example of 60% risk-free and 40% risky portfolio
![[Screenshot 2023-05-04 at 01.05.25.png]]


As mentioned earlier, different investors vary in their level of risk aversion, the higher the risk aversion, the steeper the curve. For highly risk averse investors, their optimal portfolio should have a much higher proportion of risk free asset and consequently lower risk and return. In contrast, less risk averse investors have a flatter indifference curve so their optimal portfolio can have a much higher proportion of the risky portfolio, even to the point of leverage. The risk and return of the portfolio is consequently higher.

![[Screenshot 2023-05-04 at 01.04.08.png]]

---
## Coding:
- [ ] find the best optimal investor portfolio in the risky asset and risk free asset 