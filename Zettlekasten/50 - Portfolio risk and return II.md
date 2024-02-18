# 50 - Portfolio risk and return II
202305010041
Status: #📥 
Tags: [[CFA Level I]]

## Objectives:
- [ ] describe the implications of combining a risk-free asset with a portfolio of risky assets.
- [ ] explain the capital allocation line (CAL) and the capital market line (CML).
- [ ] explain systematic and nonsystematic risk, including why an investor should not expect to receive additional return for bearing nonsystematic risk.
- [ ] explain return generating models (including the market model) and their uses.
- [ ] calculate and interpret beta.
- [ ] explain the capital asset pricing model (CAPM), including its assumptions, and the security market line (SML).
- [ ] calculate and interpret the expected return of an asset using the CAPM.
- [ ] describe and demonstrate applications of the CAPM and the SML.
- [ ] calculate and interpret the Sharpe ratio, Treynor ratio, M2, and Jensen’s alpha.

---
## Capital market theory
### Capital allocation line, indifference curve and optimal risky portfolio
The **capital allocation line** is **steepest** when it's **tangential to the efficient frontier**, and it is here where we get the **optimal risky portfolio.** There is a portfolio that the **capital allocation line** meets the **investor's utility indifference curve**, this point is the **optimal portfolio** for this particular investor.

The **efficient frontier** is formed based on the investors expectations about:
- the expected returns
- standard deviations
- correlations of returns of all risky assets

However, due to the **expectation** of the investor, there will be a **different optimal risky portfolio** and a **different capital allocation line** for another investor.

![[Screenshot 2023-05-04 at 14.54.33.png]]

### Modern portfolio theory assumption, capital market line and market portfolio
One **simplifying assumption** underlying modern portfolio theory (MPT) is that investors have **homogenous expectations**, which is they **all have the same estimates** of:
- expected return
- standard deviation (risk) 
- correlations with other risky assets for all risky assets.

Under this assumption, all investors face the **same efficient frontier** of risky portfolios and all have the **same optimal capital allocation line** termed the **capital market line**, and that means every investor will use the same optimal risky portfolio, which is the **market portfolio**.

**Theoretically**, the market should encompass all investible risky assets. However, can be quite impractical and inconvenient to model. For this reason, the local or regional stock market index as the market's proxy.

![[Screenshot 2023-05-04 at 14.56.39.png]]

### Indifference curve and market portfolio
Depending on their **indifference curves** (which is determined by the utility curve), investors may choose different combinations of the **risk-free asset and the market portfolio** along the capital market line

Investors who are **more risk averse** may put a **greater proportion of their money in risk free assets**, while **less risk averse** investors **may put more or even borrow to invest in the market**.

![[Screenshot 2023-05-04 at 15.02.00.png]]

We can estimate:
- the **expected return of the market** ($E(R_m)$)
- the **standard deviation of the market** ($\sigma_m$)
and 
we can learn the investor's portfolio:
- expected return ($E(R_p)$)
- its standard deviation ($\sigma_p$)

The **relationship of investor's portfolio** and **market portfolio** is as follows:
$$\mathrm{E(R_p)=R_f+\frac{\sigma_p}{\sigma_m}[E(R_m)-R_f]}$$
where E: expected; $R_p$: return of investor's portfolio; $R_m$: return of market portfolio; $R_f$: return of risk-free asset; $\sigma_p$: standard deviation of portfolio; $\sigma_m$: standard deviation of market portfolio

The equation of **market risk premium (MRP)**:
$$\mathrm{Market\,risk\,premium =[E(R_m)-R_f]}$$
We can see that an investor can expect to get one unit of **market risk premium** for **every unit of market risk** that the investor is willing to accept.

$$\mathrm{E(R_p)=R_f+w_m[E(R_m)-R_f]}$$
where the $\frac{\sigma_p}{\sigma_m}$ is substituted by $w_m$, which is the proportion of market portfolio in investor's portfolio.

>The beta of a stock is 0.7. Based on a market risk premium of 17% and a risk-free rate of 2.5%, what is the expected return of the stock using CAPM? **14.4%**
>
>E(R) = Rf + β x MRP = 2.5 + 0.7 x 17 = 14.4%

![[Screenshot 2023-05-04 at 15.02.09.png]]

### Lending portfolio
**Lending portfolios** are to the left of the market portfolio as investors are at least partially invested in some risk-free assets.

e.g., if the investor is 65% invested in the market portfolio (i.e. $w_m$=0.65) and the rest in risk-free assets that yield 4% (i.e. $R_f$=4) and the return of the stock market is 12% (i.e. $R_m$=12), the **expected return of the investor's portfolio**:
$$\mathrm{E(R_p)=R_f+w_m[E(R_m)-R_f]}$$
where the $w_m$: weight of the market portfolio (leverage = 1/equity weightage)
$$=4+0.65(12-4)=9.2\%$$
The expected return of the investor's portfolio is 9.2%.

### Borrowing portfolio
**Borrowing portfolio** are to the right to the market portfolio are known as borrowing portfolios as investors borrow to **get leveraged returns** (assuming they are borrowing at risk-free rate and the interest cost is none).

e.g. If we assume that investors can **borrow at the risk-free rate** as well, they can select portfolios to the right of the market portfolio.

For example, if the investor borrows 30% more than the cash, he has to invest into the market, the weight in the market portfolio is 130% (i.e. $w_m$=1.3). The **expected return of the investor's portfolio**:
$$\mathrm{E(R_p)=R_f+w_m[E(R_m)-R_f]}$$
where the $w_m$: weight of the market portfolio (leverage = 1/equity weightage)
$$=4+1.3(12-4)=14.4\%$$
The expected return of the investor's portfolio is 14.4%.

> An investor’s portfolio is 60% financed with debt borrowed at the risk-free rate of 4%. The portfolio is fully invested in an S&P500 ETF, with an expected return of 11%, and standard deviation of 28%. 
> What is the expected return of the investor’s portfolio? 21.5%
> 
> 60% debt -> 40% equity  
> 1/0.4 = 2.5 -> investor’s portfolio has a 2.5x leverage -> weight of market portfolio is 250%
> $\mathrm{E(R_p)=R_f+w_m[E(R_m)-R_f]}$ = 4 + 2.5 x (11-4) = 21.5%


### Passive portfolio
**Passive portfolio** are constructed by investors who believe in efficient markets often follow a passive investment strategy, which is to invest in a broad market equity fund (e.g. S&P500 ETF) that serves as a proxy for the **market portfolio** and allocate the rest of the spare cash in risk-free assets, such as short term government securities. The **risk and return of the passive portfolio should closely follow the capital market line**.

![[Screenshot 2023-05-04 at 15.21.17.png]]

### Active portfolio
**Active portfolio** are for investors who **do not believe in market efficiency** will not use the weight to the market portfolio.

The active investor will:
- Overweight undervalued securities
- Underweight overvalued securities
where the key goal is to obtain **higher risk-adjusted returns** relative to the market. To be exact, he expects the risk-adjusted return of his portfolio to be higher than that of the market portfolio. This means that the **portfolio risk and returns should plot above the CML**.

![[Screenshot 2023-05-04 at 15.23.02.png]]

## Unsystematic vs. systematic risk
There are broadly two categories of risk:
- **Unsystematic risk** - i.e. company specific, industry specific, diversifiable risk
- **Systematic risk** - i.e. market 

The total risk is the sum of both unsystematic risks and systematic risk:
$$\mathrm{Total\,risk=Unsystematic\,risk+Systematic\,risk}$$
where both the unsystematic risk and systematic risk uses the **variance**.

### Unsystematic risk
**Unsystematic risk** is a type of risk that is local or limited to a particular asset/industry. Since rest of the market are largely unaffected, the unsystematic risk **can be diversified away** and with **limited impact to a well-diversified portfolio**.

Some of the factors that can be unsystematic risk:
- Company specific factors - only affects company and its associates
- Earning miss
- Accounting fraud
- Major contract win
- Mergers & acquisitions (M&A)

### Systematic risk
**Systematic risk** cannot be avoided and inherent in overall market, and the market factor affects almost entire market. Therefore, systematic risk cannot be diversified away as the entire portfolio suffers.

There are factors that are considered as systematic risk:
- **Interest rate**
- **Inflation**
- **Political uncertainty**
- **Widespread natural disaster**

### Diversification benefits of unsystematic risk
When a portfolio is made up of just one security, the total risk is the systematic risk and the unsystematic risk of that one security.

However, **as the number of securities in the portfolio increases, the unsystematic risk gets diversified away** to the point where the unsystematic risk is just negligible.

One study showed that it only took about 12 to 18 stocks in a portfolio to achieve 90% of the maximum diversification possible. Another study indicated it took 30 securities, Nevertheless, it is substantially lower that the total number of securities/risky assets.

Lower correlation between securities ⇒ fewer securities required.

![[Screenshot 2023-05-04 at 15.43.14.png]]

### Pricing risk
Risk averse investors demand:
- ↑ expected returns for assets with ↑ risk, and the mechanism is through the determination of its market price. 
- The price of an asset has an inverse relationship to its expected returns when investors perceive that the risk in the asset has increased.
- They demand a higher expected return by selling the asset until its price falls to the equilibrium point where the expected return is what the investor demands.

![[Screenshot 2023-05-04 at 15.49.27.png]]

### Efficient market and pricing risk
In an **efficient market**, 2 assets that have the same risk should have market prices that reflect the same equilibrium returns for both assets, as there might be **differences in proportions of systematic and unsystematic risk**.

The **market prices** often **reflect differences and equilibrium returns between 2 assets with the same total risk**. 

![[Screenshot 2023-05-06 at 18.12.08.png]]

e.g., the stock of a **biotech firm** may have **very high proportion of unsystematic risk** as the return of the stock depends much on the success of a clinical trial that it is conducting, it's not so much affected by macroeconomic conditions. The proportion of systematic risk is smaller. 

Whereas in cyclical firms, may have a **higher proportion of systematic risk as the return of the stock depends more on the state of the economy**. The proportion of firm-specific risk (unsystematic risk) is therefore lower.

Since unsystematic risk is diversifiable, so there's no cost in diversification, and the investor simply adds more securities into a portfolio. As investors will not be compensated for bearing risk that can be eliminated at no cost on. only systematic risk is reflected in an asset price.

If we assume that **only the systematic risk of security is priced**, this accounts for the **lower expected returns for the biotech stock as only its systematic risk is priced in and higher expected returns for cyclical firms as their systematic risk is higher**.

![[Screenshot 2023-05-06 at 18.17.44.png]]

### Unsystematic risk and pricing risk
To sum up, **systematic risk is not compensated** in equilibrium because **it can be eliminated for free through diversification**. Investors **don't receive any return for accepting unsystematic risk, therefore it's in the interest of risk averse investors to hold only well diversified portfolios**.

## Returns generating models and beta
Returns generating models are used to estimate the expected returns on risky securities based on specific factors, can be classified as 
- **Macroeconomic** - e.g. GDP growth, inflation or consumer confidence,
- **Fundamental** - e.g. earnings, earnings growth, firm size and research expenditures
- **Statistical factors** - e.g. factors that explain variance or covariance in the returns (be mindful that some have no basis in finance theory, may represent only relations for a specific time period, likely identified by data mining)

### Multifactor models
Another important input to the multifactor model is the **estimate of the sensitivity of the asset returns ($\beta_{ij}$) to each specific factor**. Let's say there are k number of factors.

The general form of a **multifactor model of k number of factors** will be as follow:
$$E(R_i)-R_f=\beta_{i1}\times E(factor\,1)+\beta_{i2}\times E(factor\,2)...\beta_{ik}\times E(factor\,k)$$

The first factor is often the **expected excess return on the market**, which is an **estimate of the average market return over the risk-free rate**, which is as follows:
$$E(R_i)-R_f=\beta_{i1}\times [E(R_m)-R_f]$$

One multifactor model that is often used is that of **Fama and French**.

#### Fama and French model
In the Fama and French model, estimated the sensitivity of security returns to 3 factors:
- **The excess return on the market**
- **Size premium** 
- **Book-to-market ratio**

$$\beta_{i1}\times [E(R_m)-R_f]
+\beta_{i2}\times E(size\,premium)+\beta_{i3}\times E(Book\,to\,market\,ratio)$$

#### Carhart model
The **Carhart model** is an extension of the **Fama and French model**, adding a **4th factor** that measures **price momentum** using **prior period returns**.

Together, these four factors do a relatively good job of explaining returns differences for U.S. equity securities over the period for which the model has been estimated.

$$\beta_{i1}\times [E(R_m)-R_f]
+\beta_{i2}\times E(size\,premium)+\beta_{i3}\times E(Book\,to\,market\,ratio)+\beta_{i3}\times E(Price\,momentum)$$

#### Single factor model
A **single factor model** consists of only one risk factor and estimates only that **one sensitivity of an asset to that factor**.

**One special case** of this is the single-index model where that single factor is the **excess return on the market**, the equation is as follow:
$$E(R_i)-R_f=\beta_{i1}\times [E(R_m)-R_f]$$
This is the same as the first factor for the Fama-French and Carhart models.

It is similar to the equation of **capital market line**:
$$\mathrm{E(R_p)=R_f+\frac{\sigma_p}{\sigma_m}\times[E(R_m)-R_f]}$$
If we regard portfolio as an asset and rearrange the equation, we get something quite similar, as follows:
$$\mathrm{E(R_i)-R_f=\frac{\sigma_i}{\sigma_m}\times[E(R_m)-R_f]}$$
$$\mathrm{E(R_i)-R_f=\beta_i\times[E(R_m)-R_f]}$$
where the $\beta$ = $\frac{\sigma_i}{\sigma_m}$ i.e. standard deviation of an asset is the beta of the asset multiplied by the standard deviation of the asset.

The key takeaway here is that the capital market line, which is only for well diversified portfolios, is fully consistent with a single index model.

### Market model 
A simplified form of **single-index model** is the market model represented by the equation:
$$\mathrm{R_i=\alpha_i+\beta_i R_m+e_i}$$
where $R_i$: actual return; $\alpha_i$: intercept; $\beta_i$: slope coefficient; $e_i$: abnormal return.

Then, the market model expected return equation is as follows:
$$\mathrm{E(R_i)=\alpha_i+\beta_i R_m}$$

If we require that the intercept be the $R_f(1-\beta_i)$, which is when the alpha is:
$$\mathrm{\alpha_i=R_f(1-\beta_i)}$$
the equation will be consistent with a single-index model in excess returns form:
$$\mathrm{R_i=\alpha_i+\beta_i R_m+e_i}$$
$$\mathrm{= R_f+\beta_i(R_m-R_f)+e_i}$$
$$\mathrm{=\beta_i\times[E(R_m)-R_f]}$$
![[Screenshot 2023-05-06 at 18.50.38.png]]

e.g. :
If the a stock's beta (i.e. $\beta$=0.6) against the market, the risk-free rate is 4% (i.e. $R_f$=4%)
The equation is as follows:
$$\mathrm{\alpha_i=R_f(1-\beta_i)}=4\times(1-0.6)=1.6$$
therefore, the intercept of market model, $\alpha_i$=1.6. 

If the market return for the year is 7%, the expected return of the stock is therefore 5.8%, according to the equation of:
$$\mathrm{R_i=\alpha_i+\beta_i R_m=1.6+0.6\times7=5.8\%}$$

If the actual return of the stock for the year is 8%, the abnormal return is therefore 2.2%, according to the equation of:
$$\mathrm{R_i-E(R_i)=e_i=8-5.8\%=2.2\%}$$
where $R_i$: market model; $E(R_i)$: expected return; $e_i$: abnormal return.
This means that the stock has performed better than expected by 2.2% for the year.

![[Screenshot 2023-05-06 at 19.03.31.png]]

### Beta
How do we **estimate the beta of an asset**, which in this case is the sensitivity of the assets return to the markets return?

There are 3 ways of estimate the beta of an asset:
- through covariance of the asset and market return
- through correlation of asset and market return
- through regression method

#### Through covariance of asset and market return
The beta ($\beta$) can be calculated through this equation:
$$\beta_i=\frac{Cov_{i,m}}{\sigma_m^{2}}$$
where the $\beta_i$: beta of asset; $Cov_{i,m}$: covariance of return of asset ($R_i$) with return of market ($R_m$); $\sigma_m^2$: variance of return of market ($R_m$).

#### Through correlation of the asset and market return
As the covariance can be expressed with correlation (i.e. $Cov_{i,m}=\rho_{i,m} \sigma_i \sigma_m$), so another equation can be:
$$\beta_i=\rho_{i,m}\frac{\sigma_i}{\sigma_m}$$
 $\beta_i$: beta of asset; $\rho_{i,m}$: correlation of return of asset ($R_i$) with return of market ($R_m$); $\sigma_i$: standard deviation of return of asset ($R_i$); $\sigma_m$: standard deviation of return of market ($R_m$).

![[Screenshot 2023-05-07 at 14.48.00.png]]

#### Through regression
Another approach to estimate beta ($\beta$) is by **regressing** returns on the assets on those of the market index.

For example, if the market excess return for the period is 7%, while the excess return of the asset is 8%, we plot a point here.

Plot many of such points based on past data, and we begin to see a pattern. Regression is the mathematical method of determining the line of best fit. From here, we can determine $\beta$ based on the slope of the straight line.

![[Screenshot 2023-05-07 at 15.08.09.png]]

## CAPM and security market line 
### Capital asset pricing model (CAPM)
The **capital asset pricing model (CAPM)** asserts that the expected return of assets vary **only by their systematic risk** (measured by $\beta$), that is two different assets with the same $\beta$ will have the same expected return irrespective of the nature of those assets.

![[Screenshot 2023-05-07 at 15.13.30.png]]

### Beta, the measure of an asset's risk
**Beta ($\beta$)** is the **sensitivity of an assets return** with a **market's return** and that an assets systematic risk is due to market factors. **Systematic risk** can be measured by the **variance of market returns ($\sigma_m{^2}$)**, while unsystematic risk is due to firm specific factors. Unsystematic risk can be diversified away for free, so investors should not get additional return by taking on unsystematic risk. 

This is consistent with the CAPM. A systematic risk is the only factor that determines the assets expected returns.
![[Screenshot 2023-05-07 at 15.17.54.png]]

### Security market line
The relationship between an **assets expected return** against its **systematic risk** should be straight line. This line is known as the **security market line**. 

If the asset's beta is 0 (i.e. $\beta$=0), it's considered risk-free on the **expected return is the risk-free rate**.

If the asset's beta is 1 (i.e. $\beta$=1), this means that the asset has the same systematic risk as that of the market, so we should expect a return that is the same as the market.

If the asset's beta is below 1  (i.e. $\beta$<1), the expected return is lower than the market.

If the asset's beta is above 1  (i.e. $\beta$>1), the expected return is greater than that of the market.


![[Screenshot 2023-05-07 at 15.18.42.png]]

### Example of using CAPM formula
![[Screenshot 2023-05-07 at 15.24.09.png]]

### Assumptions of CAPM
There are several assumptions of the CAPM equation:
- **Investors** - risk adverse, maximize utility, 1 period time horizon, homogenous expectation
- **Market** - competitive market, frictionless market
- **Investable assets** - all investments are infinitely divisible

This implies that an investor can invest as little or as much as he wishes.

#### Investors
In the CAPM, the model assumes the **investors**:
- **Risk averse** -  to accept a greater degree of risk; investors require a higher expected return
- **Maximize utility** (investors indifference curve - optimizes the risk and return based on their individual preferences
- **One period time horizon** - assume decisions are on the basis of 1 period; CAPM is a single period model, this is applied out of convenience as a multiple time horizon is much harder to model
- **Homogenous expectations** - all investors have the same expectations for assets expected returns ($R_i$), standard deviation of returns ($\sigma_i$) and correlations between assets returns ($\rho_{i,j}$).

#### Market
In the CAPM, the model assumes the **market**:
- **Competitive nature** - Investors are just price takers and no investor can influence prices with their trades.
- **Frictionless markets** where there are no taxes, transaction costs or other barriers to trading.

#### Investable assets
In the CAPM, the model assumes the **investable assets**:
- all investments are infinitely divisible; this implies that an investor can invest as little or as much as he wishes.

![[Screenshot 2023-05-07 at 15.38.51.png]]

### Capital market line vs. security market line
Some candidates get confused between the **security market line (SML)** and the **capital market line (CML)**. Not only are there terms similar, the equations look similar and the graphs also look similar.
The SML and CML both intersect the vertical axis at the risk-free rate. 

However, there are many **key differences**: 
- **CML** uses **total risk** on the x axis, hence only efficient portfolios will plot on the CML- portfolios that are not efficient or individual assets will plot inside of the efficient frontier.
- On the other hand, the **SML** uses only **systematic risk** on the x axis.
- In CAPM, all properly priced assets and portfolios will plot on the SML.
- The **SML** describes the risk/return tradeoff for **individual** securities or portfolios, whereas the **CML** describes the risk/return tradeoff of **various combinations of the market portfolio and a riskless asset**.

![[Screenshot 2023-05-07 at 15.38.20.png]]

e.g. Note that a low beta asset such as stock D is not necessarily low risk when total risk is considered. The total risk of the stock is actually quite high for the low expected returns. The unsystematic risk of this stock is high.

![[Screenshot 2023-05-07 at 15.41.44.png]]

So even though the portfolio C is not the market portfolio, as it's not on the efficient frontier, it's beta is equal to one as it has the same expected return as the market portfolio.

![[Screenshot 2023-05-07 at 15.42.54.png]]

Also, a portfolio on the CML to the left of the market portfolio is a combination of the market portfolio and some risk-free asset. The beta of the portfolio is less than one.

Conversely, a portfolio on the small to the right of the market portfolio is created by borrowing at the risk-free rate to invest in the market portfolio as leverage is used, the beta is therefore greater than one.

![[Screenshot 2023-05-07 at 15.45.22.png]]
![[Screenshot 2023-05-07 at 15.45.31.png]]

### Applications of CAPM
There are two major applications of CAPM:
- **Capital budgeting process** - calculate the cost of equity
- **Equity valuation** - dividend model and forecast evaluation

#### Capital budgeting process
**CAPM** can be used by companies in the **capital budgeting process**. In estimating the weighted average cost (WACC) of capital of the firm, CAPM is one of the methods to estimate the cost of equity of the firm.

The weighted average cost of capital (WACC) equation is as follows:
$$\mathrm{w_d\times r_d(1-T)+w_p\times r_p+w_e\times r_e}$$
where $r_e$: cost of equity

Using the beta of the company stock, the required rate of return for the stock is calculated and this serves as an estimate of the cost of equity for the firm. This process is covered in the course on corporate finance.

![[Screenshot 2023-05-07 at 15.49.32.png]]

#### Equity valuation
**CAPM** can be used for **equity valuation** when using **dividend discount models** to value a stock, the required rate of return is an important parameter that needs to be estimated.

The **CAPM** is one very common way to estimate the required **rate of return** based on the stocks beta. 

The **dividend discount model** equation is as follows:
$$\mathrm{v_0=\frac{D_1}{r-g}}$$
where $v_0$: intrinsic price of equity; $D_1$: dividend of the next period; $r$: required rate of return; $g$: dividend growth rate.

This process is covered in the course on equity investments.

![[Screenshot 2023-05-07 at 15.49.44.png]]

On a related note, analysts often compare their forecast of a stock's return to its required return based on its beta risk. If the forecast return is higher than the required return, the stock is undervalued. Conversely, if the forecast return is lower than the required return, the stock is overvalued.

![[Screenshot 2023-05-07 at 15.54.52.png]]


![[Screenshot 2023-05-07 at 15.57.51.png]]

>The beta of a stock is 1.3. The return of the market is 24%, and the risk-free rate is 3%. An analyst forecasts that the stock will give a return of 17.4% in the next year.
>
>Based on the analyst’s forecast, the stock is most likely:
>Using CAPM, expected return = 3 + 1.3 x (24-3) = 30.3%
>
>As the forecast return is lower than the expected (required) return, the stock is overvalued.

## Measures of portfolio performance
The 4 measures that can be divided into 4 quadrants, based on:
- **Total risk** - represents the overall risk associated with an investment or portfolio.
- **Systematic risk** - measures the portion of risk that cannot be eliminated through diversification
- **Risk-free rate adjustment** -  accounts for the risk-free rate of return and adjusts the measure accordingly
- **Market risk adjustment** - reflects the additional risk associated with the specific market conditions and factors affecting the investment

The **4 risk measure ratios** are as follows:
- **Sharpe ratio** - measures the **risk-adjusted return** of an investment by considering its **excess total return over the risk-free rate per unit of volatility**.
- **$M^2$ measure** - evaluates the risk-adjusted return of an investment by combining the Sharpe ratio and the Treynor ratio, providing a comprehensive assessment of performance.
- **Treynor measure** - assesses the **risk-adjusted return** of an investment by dividing the **excess return over the risk-free rate by its beta**, indicating how well it compensates for systematic risk.
- **Jensen's alpha** - calculates the **risk-adjusted excess return** of an investment by comparing its actual return with the expected return based on the Capital Asset Pricing Model (CAPM) (i.e. market portfolio)??.

### Sharpe ratio
The **Sharpe ratio** is a **risk-free rate adjusted** measure based on **total risk**. It's defined as the excess returns per unit of total portfolio risk, calculated simply as the portfolio return, minus the risk free rate divided by the standard deviation of the portfolio.

The **Sharpe ratio** equation is as follows:
$$\mathrm{Sharpe\,ratio=\frac{R_p-R_f}{\sigma_p}}$$
where $R_p$: return of portfolio; $R_f$: return of risk-free rate; $\sigma_p$: standard deviation of portfolio. The excess returns per unit of total portfolio risk.

The Sharpe ratio of a portfolio as the slope of its **capital allocation line (CAL)** and can be compared to the slope of the **capital market line (CML)**, which is the Sharpe ratio for any portfolio along the CML. If the slope of the **CAL** is steeper than the **CML**, it means that the portfolio outperforms the market on a risk-adjusted basis.

![[Screenshot 2023-05-07 at 15.59.03.png]]

### $M^2$ measure
**$M^2$ measure** is the measure of **total risk against the market portfolio**.

e.g., this portfolio has a lower return than the market returns but if we project the return based on its Sharpe ratio, the portfolio is actually outperforming the market.

The $M^2$ is the excess return over the market on a risk-adjusted basis (i.e. with the same as market total risk, the portfolio is generate excess return).

The $M^2$ measure equation is as follow:
$$\mathrm{M^2=(R_p-R_f)\frac{\sigma_m}{\sigma_p}-(R_m-R_f)}$$
where $M^2$: ; $R_p$: return of portfolio; $R_f$: risk-free rate; $\sigma_m$: standard deviation of market; $\sigma_p$: standard deviation of portfolio; $(R_m-R_f)$: return of market minus risk-free rate. 

![[Screenshot 2023-05-07 at 16.06.33.png]]

### Treynor measure
**Treynor measure** is the equivalent of the **Sharpe ratio based on systematic risk**, so the returns are measured as per unit **systematic risk**.

The **Treynor measure** equation is as follow:
$$\mathrm{Treynor\,ratio=\frac{R_p-R_f}{\beta_p}}$$
In this case, we simply replace the portfolio standard deviation with portfolio beta ($\beta$).
Likewise, the Treynor measure is the slope of this line.

![[Screenshot 2023-05-07 at 16.16.20.png]]

### Jensen's alpha
**Jensen's alpha** is based on systematic risk, but market adjusted.

The difference with the $M^2$ in this case is that instead of measuring the excess return based on the market risk, the Jensen's alpha is a measure of excess return based on the portfolio beta.

Based on the security market line, the portfolio's expected return is supposed to be here, and calculate this using the CAPM.

If the portfolio's actual return is here, the Jensen's alpha is therefore this portion here, the portfolio's actual return minus its expected return.

The **Jensen's alpha return** equation is:
$$\mathrm{Alpha=R_p-[R_f+\beta_p\times(R_m-R_f)]}$$
where $R_p$: actual return of portfolio; $[R_f+\beta_p\times(R_m-R_f)]$: CAPM equation.

![[Screenshot 2023-05-07 at 16.17.00.png]]

### Conclusion of measures of portfolio performance
![[Screenshot 2023-05-07 at 16.21.02.png]]

> An investor would like to know if the return of one of his many portfolios is outperforming the market on a risk-adjusted basis. Which of the following measures is the most appropriate? **Jensen’s alpha**.
> 
> The investor has many portfolios so the unsystematic risk is less relevant. The measure should be based on systematic risk.
> 
> Treynor and Jensen’s alpha measure based on systematic risk, but only Jensen’s alpha is market risk adjusted.



### Example of measurement of portfolio performance
![[Screenshot 2023-05-07 at 16.27.28.png]]
It's interesting to note that based on its systematic risk, only the portfolio outperformed, well, based on total risk, the portfolio underperformed the market.

### Determining the appropriate measure to use
In essence, the choice is between the type of risk that is the more appropriate benchmark where the risk adjustment should be based on total risk or systematic risk depends on who the investor is.

#### Only 1 portfolio
If the investor only owns this particular portfolio, then he is exposed to both a systematic and unsystematic risk of the portfolio.

This investor should use the **Sharpe ratio** and $M^2$ measure to evaluate this portfolio as it is based on total risk.

#### Multi-portfolio with well diversification
If this portfolio is just one of the many portfolios that the investor has, the unsystematic risk of the portfolio will be of little significance to the investor if their portfolios are well diversified from each other issued.

Therefore, use the **Treynor measure** and **Jenson's alpha** to evaluate this portfolio.

![[Screenshot 2023-05-07 at 16.21.31.png]]


---
'

Level I CFA candidate Adeline Bass is a member of an investment club. At the next meeting, she is to recommend whether or not the club should purchase the stocks of CS Industries and MG Consolidated. The risk-free rate is at 6% and the expected return on the market is 15%. Prior to the meeting, Bass gathers the following information on the two stocks:

|Info|CS Industries|MG Consolidated|
|:-:|:-:|:-:|
|Current Market Value|$25|$50|
|Expected Market Value in One Year|$30|$55|
|Expected Dividend|$1|$1|
|Beta|1.2|0.80|

In the context of the SML, a security is underpriced if the required return is less than the holding period (or expected) return, is overpriced if the required return is greater than the holding period (or expected) return, and is correctly priced if the required return equals the holding period (or expected) return.

Here, the holding period (or expected) return is calculated as: (ending price – beginning price + any cash flows / dividends) / beginning price. The required return uses the equation of the SML: risk free rate + Beta × (expected market rate − risk-free rate).

- For CS Industries: ER = (30 – 25 + 1) / 25 = 24%, RR = 6 + 1.2 × (15 – 6) = 16.8%. Stock is underpriced - purchase.
- For MG Consolidated: ER = (55 – 50 + 1) / 50 = 12%, RR = 6 + 0.80 × (15 – 6) = 13.2%. Stock is overpriced - do not purchase.




Charlie Smith holds two portfolios, Portfolio X and Portfolio Y. They are both liquid, well-diversified portfolios with approximately equal market values. He expects Portfolio X to return 13% and Portfolio Y to return 14% over the upcoming year. Because of an unexpected need for cash, Smith is forced to sell at least one of the portfolios. He uses the security market line to determine whether his portfolios are undervalued or overvalued. Portfolio X's beta is 0.9 and Portfolio Y's beta is 1.1. The expected return on the market is 12% and the risk-free rate is 5%. Smith should sell: **portfolio Y only.**


Portfolio X's required return is 0.05 + 0.9 × (0.12-0.05) = 11.3%. It is expected to return 13%. The portfolio has an expected excess return of 1.7%

Portfolio Y's required return is 0.05 + 1.1 × (0.12-0.05) = 12.7%. It is expected to return 14%. The portfolio has an expected excess return of 1.3%.

Since both portfolios are undervalued, the investor should sell the portfolio that offers less excess return. Sell Portfolio Y because its excess return is less than that of Portfolio X.





---
## Questions before starting this section:
- [ ]

## Codes to test understanding of objectives
