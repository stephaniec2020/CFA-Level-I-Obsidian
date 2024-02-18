# 30 - Cost of capital
202305111910
Status: #📥 
Tags: [[CFA Level I]]

## Objectives:
- [x] calculate and interpret the weighted average cost of capital (WACC) of a company.
- [ ] describe how taxes affect the cost of capital from different capital sources.
- [ ] calculate and interpret the cost of debt capital using the yield-to-maturity approach and the debt-rating approach.
- [ ] calculate and interpret the cost of noncallable, nonconvertible preferred stock.
- [ ] calculate and interpret the cost of equity capital using the capital asset pricing model approach and the bond yield plus risk premium approach.
- [ ] explain and demonstrate beta estimation for public companies, thinly traded public companies, and nonpublic companies. 
- [ ] explain and demonstrate the correct treatment of flotation costs.
---

## Weighted average cost of capital (WACC)
### Calculating WACC
The **discount rate** of future expected cash flow is the **weighted average cost of capital (WACC)**.
#### Component cost of capital
The **capital components** of a firm usually consists of:
- Debt
- Equity
- Preferred stock
Any increase in a firm's total assets will have to be financed through an increase in at least one of these capital accounts.

These are the **return demanded** from investors for the risk they take.
$r_d$: Cost of debt (before tax) - rate at which firm needs to pay when it issues new debt  - The yield on a BBB corporate bond reflects a pre-tax cost of debt. 
$r_p$: Cost of preferred stock - rate at which firm needs to pay when it issues new preferred stock
$r_e$: Cost of common equity - required rate of return on firm's common stock, and generally difficult to estimate.

Typically, the cost of debt is the cheapest, and equity the highest (i.e. $r_d$ < $r_p$ < $r_e$).

The weighted average cost of capital equation is as follows:
$$\mathrm{WACC=w_d\times r_d(1-T) + w_p\times r_p +w_e\times r_e}$$
where $w$: weight of each component; $r$: required rate of return (in %); $d$: debt $p$: preferred equity; $e$: equity. (1-T) since the interest paid on corporate debt is tax deductible, so therefore that is tax-adjusted to reduce the **marginal** tax rate (not the effective tax rate).

### Tax effects 
#### Corporate debt tax deductible nature
Do note that in many countries, the **interest paid on corporate debt is tax deductible**.
The **actual cost of the debt to the firm (after-tax cost of debt)**:
$$w_d\times r_d(1-T)$$
where

The yield on a BBB corporate bond reflects a pre-tax cost of debt. 

#### Example of corporate tax
If a company has $10 million debt and pays 10% interest on it, the total interest paid each year is $1 million. However, this $1 million is tax deductible. So if the marginal tax rate is 30%, the company will pay $300,000 less taxes. In aggregate, the after-tax cost of debt to the company is $700,000, which is 7% of the outstanding debt. If you take 10%, multiply by 1 minus 0.3 (i.e. $r_d(1-T)$), you get the same figure. **Note** that this tax deductible
only applies to interest paid on a company's debt.

![[Screenshot 2023-05-12 at 19.36.49.png]]

#### Example of WACC calculation
![[Screenshot 2023-05-13 at 18.16.48.png]]

### Assigning weights
In most companies, the decisions on **raising capital** and the decisions on **budgeting or investments** are considered independently.

The **financing department** is responsible for **keeping costs low** and using a **balance of funding sources**, i.e. debt, preferred stock, and common equity. Most firms have a **target capital structure**, which is the proportions of debt, preferred stock, and equity that the firms strive to achieve over time.

**In the short run**, as funds are typically raised in large sums, the actual weights can **sometimes differ significantly from the target weights**. Nevertheless, **most firms will adhere** to the target weights in the long run. The weights in the calculation of WACC should be **based on the firm's target capital structure**.

However, a firm's target capital structure may not be made known to analysts outside the firm.

In such a case, you can estimate it using the company's current capital structure based on:
- the market values of the securities
- analyze trends in the firm's capital structure
- industry average capital structure to estimate the target capital structure

The financing department determines the capital structure of the firm, from which we can compute the WACC of the firm. Each investment decision must be made assuming a WACC. If a project's return on investment is greater than the WACC, the firm's value is increased and such projects should be pursued.

![[Screenshot 2023-05-13 at 18.28.28.png]]

### Marginal cost of capital
The **marginal cost of capital curve (MCC)** describes the phenomenon of the more capital the firm raises, the higher the risk since WACC of a firm does not remain constant regardless of the amount that it raises. Investors will demand more as compensation for the risk.

Let's say there are three projects that the firm is considering and the three projects are not mutually exclusive.

Project A costs $10 million and has an IRR of 27%.
Project B also costs $10 million and has an IRR of 20%.
Project C costs $10 million as well and has an IRR of 14%.

If the company decides to invest in project A for $10 million, it can raise the funds at a cost of 12% and have a 15% margin of safety. This project is likely to be very profitable.

If the company decides to invest in Project B as well, it can raise funds at a cost of 17%
and have a 3% margin of safety. This should also be profitable for the company.

However, if the company decides to invest in project C as well, the cost of capital will be 28%, which is higher than the project IRR of 14%. Project C should not be accepted.

![[Screenshot 2023-05-13 at 18.31.30.png]]

#### Optimal capital budget
Investment opportunity schedule demonstrates a company's investment opportunities generally decrease as the company makes additional investments. The **optimal capital budget** is the intersection of the **investment opportunity schedule (IOS)** with the marginal **cost of capital curve (MCC)**.

The firm should:
- undertake all those projects with IRRs greater than the marginal cost of capital (i.e. **IRR > MCC ⇒ accept the project**) - This will maximize the value created
- no projects with IRRs less than the marginal cost of capital should be undertaken as they will erode the value created by the firm (i.e. **IRR < MCC ⇒ reject the project**)
- accept positive NPV projects
- reject negative NPV projects

![[Screenshot 2023-05-13 at 18.36.25.png|300]]![[Screenshot 2023-05-13 at 18.36.36.png|300]]

## Costs of the different sources of capital
The **weighted average cost of capital (WACC)** equation is as follows:
$$\mathrm{WACC=w_d\times r_d(1-T) + w_p\times r_p +w_e\times r_e}$$
where $w$: weight of each component; $r$: required rate of return (in %); $d$: debt $p$: preferred equity; $e$: equity. (1-T) since the interest paid on corporate debt is tax deductible, so therefore that is tax-adjusted to reduce the **marginal** tax rate (not the effective tax rate). The WACC weights should use the firm's target capital structure.

Each component, there are different ways to calculate:
- **Cost of debt** - YTM, Debt-rating approach
- **Cost of preferred stock** - r=D/P - where P is current market price
- **Cost of common stock** - CAPM, bond yield+risk premium

### Cost of debt
The **cost of debt** is the interest a firm needs to pay when issuing bonds/take bank loan.

There are several approaches to calculate the cost of debt:
- **Yield-to-maturity method**
- **Debt rating approach**

It can be calculated by the **yield-to-maturity (YTM)** of outstanding bonds.

The **yield-to-maturity** of a bond is the yield that equates the present value of the promised payments to its market price. This is the **preferred method if the bond is publicly and frequently traded**.

![[Screenshot 2023-05-13 at 18.54.55.png]]

However, some of the limitations of YTM approach:
- primarily issues floating rate debt (the interest rate adjusts periodically according to a benchmark) ⇒ cost depends on current yield & future yield (unknown), might use current yield curve and term structure theory to work out an average cost
- bonds that have embedded options (e.g. call, conversion, put options) ⇒ options affect the cost company pays for its debt

Estimating cost of debt using **the debt rating approach**:
- estimated using the yield on comparable bonds in terms of **credit rating and maturity**. However, their **marginal tax rate** can be different.
	- $\mathrm{r_d(1-T)}$; where $r_d$: similar credit rating and maturity, but after-tax cost of debt need to use this equation
	- suitable when a company's bonds are private placements or thinly traded where market information is limited:
-  Estimate by **interpolating the fields of a number of comparable bonds** (matrix pricing)

### Limitations of debt rating approach 
There are several limitations in using the debt rating approach:
- **Comparable bonds can have different characteristics** that affect their yields: 
	- Seniority
	- Covenants
	- Embedded options
- **Some companies issue non-rated debt** - methods to estimate debt rating can be imprecise

### Cost of preferred stock
The market price of a company's preferred stock is the amount of preferred dividends divided by the required rate of return.

The equation of **market price of preferred stock** is:
$$\mathrm{P=\frac{D}{r}}$$
where P: current market price of preferred stock; D: dividends; r: required rate of return (i.e. return that investors require from firm's preferred stock = cost company needs to pay when it issues new preferred stock).

The newly-issued preferred shares of most companies generally sell at par. As such, the dividend yield on a firm's newly-issued preferred shares is the market's required rate of return. 

By rearranging the equation, the equation of **cost of preferred stock** is:
$$\mathrm{r=\frac{D}{P}}$$
where P: market price of preferred stock; D: dividends; r: required rate of return (i.e. cost company needs to pay when it issues new preferred stock).

![[Screenshot 2023-05-13 at 20.38.48.png]]

### Cost of common equity
There are two ways of **estimating cost of equity**: 
1. **Capital asset pricing model (CAPM)** 
2. **Bond yield + Risk premium**.

#### Capital asset pricing model (CAPM)
The **capital asset pricing model (CAPM)** asserts that the expected return of assets vary **only by their systematic risk** (measured by $\beta$), that is two different assets with the same $\beta$ will have the same expected return irrespective of the nature of those assets.

The **capital asset pricing model (CAPM)** equation is as follows:
$$r=R_f+\beta[E(R_m)-R_f]$$
where r: required rate of return; $R_f$: risk-free rate; $\beta$: systematic risk of stock; $E(R_m)$: expected return on market.

Below denoted the equation origin, it is explained in detail in portfolio management section.

##### Security market line
The relationship between an **assets expected return** against its **systematic risk** should be straight line. This line is known as the **security market line**. 

If the asset's beta is 0 (i.e. $\beta$=0), it's considered risk-free on the **expected return is the risk-free rate**. If the asset's beta is 1 (i.e. $\beta$=1), this means that the asset has the same systematic risk as that of the market, so we should expect a return that is the same as the market. If the asset's beta is below 1  (i.e. $\beta$<1), the expected return is lower than the market. If the asset's beta is above 1  (i.e. $\beta$>1), the expected return is greater than that of the market.

![[Screenshot 2023-05-07 at 15.18.42.png]]

Again, the **capital asset pricing model (CAPM)** equation is as follows:
$$r=R_f+\beta[E(R_m)-R_f]$$
where r: required rate of return; $R_f$: risk-free rate; $\beta$: systematic risk of stock; $E(R_m)$: expected return on market. The required rate of return ($r$) is the return that investors required from firm's common stock, which is the cost company needs to pay when it issues new common stock.

In order to use this method, we need to estimate all the **three parameters (i.e. $R_f$, $\beta$, $E(R_m)$)** of the CAPM:
$R_f$: risk-free rate ⇒ government bond yields like US treasury notes, to make an effort to match the maturity of the risk-free benchmark to the useful life of the project.
$\beta$: systematic risk of the stock ⇒ estimated from the volatility of returns of the stock using historical data.
$E(R_m)$: expected return on market  ⇒ estimated from past broad market index returns

![[Screenshot 2023-05-13 at 20.58.03.png]]

#### Bond yield + risk premium
The **bond yield plus risk premium approach** can be referred to as a "lazy approach" of estimating the cost of equity.

The equation of **bond yield + risk premium to calculate cost of equity** is as follows:
$$\mathrm{r_e=r_d+Risk\,premium}$$
where $r_e$: cost of equity; $r_d$: yield of long-term debt (YTM); risk premium: arbitrarily, a figure from 3% to 5% should be appropriate.

![[Screenshot 2023-05-13 at 21.13.58.png]]
![[Screenshot 2023-05-13 at 21.21.33.png]]

## Project beta
Limitations of the NPV or IRR method is the assumption that **the project under consideration has the same level of risk as the firm's existing projects** by using the WACC calculation. However, this may not be a reasonable assumption, as most of the times the project under consideration is of a different risk level. This implies that the firm's WACC is not suitable for evaluation of the project.

One way to factor in the difference in risk level is to estimate the **project's beta**. **A project's beta** is a measure of the **project's systematic risk on its own**. We can use a project's beta to estimate the cost of equity for a specific project.

### Pure-play method
**Pure-play method** is to make inferences from other publicly-traded companies which are engaged in a business similar to the project under consideration.

e.g. If Walmart is looking to set up a fast food chain using the beta of its own stock to estimate the cost of equity for the new project, may not be suitable as it's based on the risk level of its current hypermarket business also not other conglomerate as its beta depends on its many different lines of business. Rather, McDonald's stock trade beta or the fast food industry average beta may be more appropriate.

![[Screenshot 2023-05-13 at 21.26.46.png]]

#### Beta and financial leverage
Another important consideration is that the **degree of financial leverage** can differ significantly between firms and the **beta** of a firm **is a function of its financial leverage**.

In general, the higher a firm's debt-to-equity ratio, the greater is its beta (i.e. ↑D/E ⇒ ↑$\beta$).

To do that, **unlever the beta of the equity of the reference company** using this formula:
$$\mathrm{\beta_{asset}=\frac{\beta_{equity}}{[1+(1-T)\times D/E]}}$$
where $\beta_{asset}$: beta of asset without borrowing; = $\beta_{equity}$: beta of the stock; $T$: marginal tax rate; $D/E$: debt-to-equity ratio.

Then, to **re-lever the subject company's capital structure** to get to beta of the project:
$$\mathrm{\beta_{project}=\beta_{asset}\times{[1+(1-T)\times D/E]}}$$
where $\beta_{asset}$: beta of asset without borrowing; = $\beta_{equity}$: beta of the stock; $T$: marginal tax rate;  $D/E$: debt-to-equity ratio.

![[Screenshot 2023-05-13 at 21.37.47.png]]

Once we have the beta of the project, we can use this beta to estimate the **cost of equity** of the project and plug this in to find the **WACC** applicable to the project.

![[Screenshot 2023-05-13 at 21.38.07.png]]

![[Screenshot 2023-05-13 at 21.44.33.png]]

### Challenges in estimating equity's beta ($\beta_{equity}$)
To estimate the beta of a stock $\beta_{equity}$, the **volatility of the stock price** is measured against the **volatility of a benchmark**. **Beta** is greater than one if the stock's volatility is higher (i.e. $\beta_{equity} > 1$)than the benchmark and lower than one if its volatility is lower (i.e $\beta_{equity} < 1$).

There are 4 challenges in estimating equity's beta:
- **Historical data** - not indicative of future patterns, it is sensitive to the length, period frequency of data used, it can be different between analyst
- **Choice of benchmark** - inappropriate benchmark makes beta not meaningful
- **Betas believed to be reverting to 1 over time** - lower estimate if $\beta>1$; raise estimate if $\beta<1$
- **May not capture risk in small firms**
- **Does not adequately capture country risk for companies in developing countries**

## Flotation costs
When a company raises new capital, it generally seeks the assistance of investment bankers.
The investment bankers typically charge **flotation costs** between **2 and 7% on the amount of equity capital raised**. **Flotation costs are not an ongoing cost to the project, it is only charged once in the initiation of the project**. Such fees are substantial and should be factored in when a company is evaluating a capital project.

The fees for **preferred stock and debt, however, are usually not considered as they're usually quite insignificant (i.e. < 1%)**.

To incorporate the flotation cost, there are 3 components to calculate to get to the final NPV:
- **Cost of equity** - Dividend discount model
- **Weighted average of cost of capital (WACC)** - weighted average of debt, preferred stock, and common equity
- **Net present value (NPV)** - NPV of the project is the present value of all the cash flows discounted by the WACC 

The equation of **cost of equity (dividend discount model)** is as follows:
$$\mathrm{Cost\,of\,equity=\frac{D_1}{P_0}+g}$$
where $D_1$: dividend; $P_0$: market price; $g$: growth rate (1+x).

The **weighted average cost of capital (WACC) equation** is as follows:
$$\mathrm{WACC=w_d\times r_d(1-T) + w_p\times r_p +w_e\times r_e}$$
where $w$: weight of each component; $r$: required rate of return (in %); $d$: debt $p$: preferred equity; $e$: equity. (1-T) since the interest paid on corporate debt is tax deductible, so therefore that is tax-adjusted to reduce the **marginal** tax rate (not the effective tax rate). The WACC weights should use the firm's target capital structure.

The net present value is the NPV on calculator after discounting the future cash flows.

![[Screenshot 2023-05-13 at 21.54.22.png]]

![[Screenshot 2023-05-13 at 22.08.14.png]]

#### Example of project beta calculation
![[Screenshot 2023-06-25 at 11.39.50.png]]


#### Example of floatation cost calculation
![[Screenshot 2023-06-25 at 11.45.12.png]]
---
## Questions before starting this section:
- [ ]