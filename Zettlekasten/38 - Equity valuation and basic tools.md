# 38 - Equity valuation and basic tools
202305202122
Status: #📥 
Tags: [[CFA Level I]]

## Objectives:
- [ ] evaluate whether a security, given its current market price and a value estimate, is overvalued, fairly valued, or undervalued by the market.
- [ ] describe major categories of equity valuation models.
- [ ] describe regular cash dividends, extra dividends, stock dividends, stock splits, reverse stock splits, and share repurchases.
- [ ] describe dividend payment chronology.
- [ ] explain the rationale for using present value models to value equity and describe the dividend discount and free-cash-flow-to-equity models.
- [ ] calculate the intrinsic value of a non-callable, non-convertible preferred stock.
- [ ] calculate and interpret the intrinsic value of an equity security based on the Gordon (constant) growth dividend discount model or a two-stage dividend discount model, as appropriate.
- [ ] identify characteristics of companies for which the constant growth or a multistage dividend discount model is appropriate.
- [ ] explain the rationale for using price multiples to value equity, how the price to earnings multiple relates to fundamentals, and the use of multiples based on comparables.
- [ ] calculate and interpret the following multiples: price to earnings, price to an estimate of operating cash flow, price to sales, and price to book value.
- [ ] describe enterprise value multiples and their use in estimating equity value.
- [ ] describe asset-based valuation models and their use in estimating equity value.
- [ ] explain advantages and disadvantages of each category of valuation model.

---

## Equity valuation - concept and basic tools
### Intrinsic value vs market price
**Intrinsic value** **("fundamental value")** of a company stock is defined as the **value placed by rational investors if they had complete understanding of the stock's fundamentals and characteristics**.

**Estimate of the intrinsic value** from the analyst implicitly saying that the market is inefficient (weak-form of market) and that **abnormal profits** can be made by trading to profit when the **market price converges towards the intrinsic value**.

If the estimated intrinsic value < the market price, the stock is overvalued and the investor should sell or short the stock. If the intrinsic value > market price,  the stock is undervalued and the investor should buy the stock. If the two values are equal, the stock is fairly valued and no abnormal profit is expected.

### Consideration when deciding whether to act on analyst estimate
There are 5 points should be considered:
- **% difference between the market price and the estimate** - small differences are to be expected; if the difference is large, the expected profit may be worth taking the risk for.
- **Confidence in the appropriateness of the valuation model** - is the model appropriate for this company's line of business?
- **Confidence in assumptions used?** - e.g. growth rate; some models are extremely sensitive
- **Reasons behind the mispricing** - no satisfactory reason, insider trading?
- **Believe that market price will move toward estimate within the time horizon**

## Major categories of equity valuation model
There are 3 major categories of equity valuation model:
- **Present value models** - discounted cashflow model (DCF); intrinsic value = PV of future benefits expected
	- **Dividend discount model** - **Gordon growth model** assumed to grow at a constant rate; **2-stage dividend discount model** -  
	- **Free cash flow to equity (FCFE) model (cash flow available distributed to shareholders)**
- **Multiplier models** - based on relative valuation 
	- **Share price multiple** - (Price/fundamental e.g. P/E, P/S, P/B, P/CF) - multiply the multiple to calculate the price
	- **Enterprise value multiple** - EV/EBITDA; EV/Revenue (where **enterprise value** is all $\mathrm{All\,outstanding\,securities - Cash - Short\,term\,investment}$; which the $\mathrm{EV = Debt+Preferred\,stock+ (Intrinsic\,value)\,stocks}$)
- **Asset-based valuation models** - **adjusted to fair value** and $\mathrm{Intrinsic\,value\,of\,common\,stock=Assets - Liabilities -Preferred\,stock}$

## All about dividends
### Type of dividends
A **cash dividend** is:
- a cash distribution a company makes to its shareholders
- when dividend is mentioned, it usually refers to cash dividends unless otherwise stated.
- not an obligation, but are entirely up to the discretion of the management
- typically paid out regularly at known intervals and are known as regular cash dividends.
- a long term record of stable or increasing dividends is widely viewed by investors as a sign of a company's financial stability
- when a firm pays out cash dividends, the cash leaves the company's books and equity is reduced by the amount of cash paid out.

**Special dividend (extra dividend)** is:
- when companies pay irregular one-off dividends
- many cyclical firms use special dividends to share profits with shareholders when times are good, but maintain the flexibility to conserve cash when profits are poor
- can also be paid by companies that do not pay regular cash dividends

**Stock dividend** is:
- when sometimes dividends are not paid in cash, but in the form of new shares
- e.g. 10% stock dividend means every shareholder gets 10% more stock
- In the case of a stock dividend, the cash is conserved in the firm's balance sheet and the shareholders equity remains the same

>**Syntax for stock splits**:
>{num of shares after split}-for-{every num of shares before split}
>A 10% stock dividend is equivalent to owning 11 shares for 10 shares owned before the dividend.

![[Screenshot 2023-05-20 at 22.17.27.png]]

**Share repurchase** is:
- An alternative to cash dividend payments
- A transaction in which a company uses cash to **buy back** its own shares
- Shares that have been repurchased (treasury) are not considered for dividends, voting or computing EPS
- lead to fewer number of outstanding shares, the earnings attributable to each share is increased, thus increasing the value of each share and shareholder's wealth

### Share repurchase vs cash dividends
There are 4 main reasons for management for share repurchase over cash dividends:
- Flexibility in the **amount** and **timing** of distributing cash to shareholders
- **Support** the share price and **signal** that the shares are undervalued
- Higher taxes on dividends received, stock repurchase can help shareholders **pay less tax**
- **Offset** an increase in outstanding shares from the exercise of employee stock option

### Dividend payment chronology
The payout of regular cash dividends to common shareholders follows a standard chronology:
1. Company's board of directors votes to pay the dividend
2. **Declaration date** - the day that the company issued a statement declaring a specific dividend.
3. **Ex-dividend date** - first date that a share trades without the dividend, if you buy the share on or after this date, you will not receive the dividend.
4. **Holder-of-record date** - 1 or 2 business days later than the ex-dividend date, all shareholders listed on the company's books are recorded down for receiving the upcoming dividend (trades on the stock exchange typically take one to two business days to settle).
5. **Payment date** - company actually mails out or electronically, transfers a dividend payment to the shareholders.

One last thing you need to know is that the share price will drop by the amount of dividend paid at the opening of the ex-dividend date since buyers of the shares on this date onwards are no longer eligible to receive this dividend.

![[Screenshot 2023-05-20 at 22.59.31.png]]

## Present value model - Dividends discount model
**Present value model**, also known as **discounted cash flow model** (the intrinsic value = discount the future benefits expected):

### Dividend discount models
The **dividend discount model** defined such benefits as the expected future dividends to be distributed to shareholders.

#### Single year holding period
For a **holding period of one year**, the value of the stock today is the **present value of any dividends** during the year, plus the present value of the **expected price of the stock at the end of the year** referred to as its terminal value.

The **intrinsic value of stock in single-year holding period through dividend discount model**:
$$\mathrm{PV_stock=\frac{Future\,dividend}{(1+r)^1}+\frac{Terminal\,value}{(1+r)^1}}$$
The **discount rate (r)**: required rate of return on common stock for the firm.

![[Screenshot 2023-05-20 at 23.21.10.png]]

#### Multi year holding period
The intrinsic value of a stock for a **multi-year holding period** can be estimated using the the same method as one year holding period.

The **intrinsic value of stock for multi-year holding period using dividend discount model (DDM)**:
$$\mathrm{PV_stock=\sum PV_div+PV_{terminal}}$$
which is the $\sum PV_{div}$: is the sum of all dividends discounted to present value; $PV_{terminal}$: and the terminal value discounted to present.

The **sum of present value of dividends** can be calculated through:
$$\mathrm{\sum PV_div=\sum\frac{D_1}{(1+r)^1}+\frac{D_2}{(1+r)^2}+\frac{D_3}{(1+r)^3}...+\frac{D_t}{(1+r)^t}}$$
where D: dividend; r: required rate of return.

![[Screenshot 2023-05-20 at 23.21.22.png]]

![[Screenshot 2023-05-20 at 23.21.40.png]]

However, there might be some concerns:
- What if the company is not expected to pay dividend?
- **Growth companies pay little or no dividends**, the company conserve cash for expansion
- future dividend payouts can be hard to predict for firms with a short history.
In these scenario, **free cash flow to equity (FCFE) models** can be used.

### Free cash flow to equity (FCFE) models
**Free cash flow to equity (FCFE) model** is an equity valuation model when predicting intrinsic value of stock without dividends.

The equation for **free cash flow to equity (FCFE) model** is as follows:
$$\mathrm{PV_stock=PV_{FCFE}+PV_{terminal}}$$
**Free cash flow to equity (FCFE)**  is an appropriate alternative as it represents the **amount of cash** collected during the period that's **available** for **distribution to common shareholders**. Therefore, FCFE reflects the firm's capacity to pay dividends.

The amount of cash available to distribute to the shareholder is:
- **Net cash from operation** (i.e. $\mathrm{CFO - FC_{Inv}}$)
- **Net borrowing** (i.e. $\mathrm{New\,borrowing - Debt\,repayment}$)

The **net cash from operations** is the cash generated from a company's business operations (i.e. $\mathrm{Net\,CFO - FC_{Inv}}$), minus the costs required to operate the business, so not all of this cash is available to common shareholders.

The company typically invests part of it back to the business during the period to maintain the value of the company as a going concern (i.e. **Fixed capital** invested back into the company to maintain value of company).

Another source of cash for the company is through **new borrowings** during the period within the same period, the company can use the cash to pay off some of the existing debt. The **net amounts borrowed are considered to be available for distribution** to common shareholders.

As such, **FCFE equation** can be expressed as follows:
$$\mathrm{FCFE=Net\,CFO- FC_{Inv}+Net\,borrowings}$$
where $FC_{Inv}$: fixed capital investment; $\mathrm{Net\,borrowings=New\,borrowing - Debt\,repayment}$.

After acquiring the FCFE value, the **intrinsic value of stock calculated from FCFE** is as follows:
$$\mathrm{PV_stock=PV_{FCFE}+PV_{terminal}}$$
where $PV_{FCFE}$: discounted present value of FCFE; also have to adjust to the FCFE per share; $PV_{terminal}$: discounted terminal value.
![[Screenshot 2023-05-20 at 23.31.58.png]]
![[Screenshot 2023-05-20 at 23.36.06.png]]
![[Screenshot 2023-05-20 at 23.39.03.png]]

### Determine the required rate of return
The **required rate of return for the stock is needed** as the discount rate for the future cash flows for both **dividend discount model** or the **FCFE** model.

The **required rate of return (r)** is CAPM's ${E(R_i)}$
However, ${E(R_i)}$ is an estimated number based on:
- the **risk-free rate** ($R_f$)
- **systematic risk of investment (stock)** ($\beta$)
- **expected return on market** ($E(R_m)$)
, which is explained in detail below.

**Capital asset pricing model (CAPM)** can be used for **the required rate of return for a stock is a function of the risk-free rate**. 

The **capital asset pricing model (CAPM)** equation is as follows:
$$\mathrm{E(R_i)=R_f+\beta_i\times[E(R_m)-R_f]}$$
where $E(R_i)$: expected return on investment (stock); $R_f$: risk-free rate; $\beta$: systematic risk of investment (stock); $E(R_m)$: expected return on market.

These values are **estimated** through:
- **$R_f$: risk-free rate** - government bond yield
- **$\beta$: systematic risk of investment (stock)** - volatility of returns of stock
- **$E(R_m)$: expected return on market** - broad market index returns

![[Screenshot 2023-05-21 at 11.02.17.png]]

### Preferred stock solution
**Preferred stock** have fixed dividend and is paid at regular intervals.

The **preferred stock intrinsic value through dividend discount model** is as follows:
$$\mathrm{PV_{pref.}=\frac{D}{(1+r)^1}+\frac{D}{(1+r)^2}+...+\frac{D}{(1+r)^N}}$$
$$\mathrm{PV_{pref.}=\frac{D}{r}}$$
where D: dividend; r: required rate of return; N: interval into perpetuity.

![[Screenshot 2023-05-21 at 11.18.31.png]]

## Present value model - Gordon growth model
### Gordon growth model
**Gordon growth model** assumes **the dividend growth at a constant rate**. 

The **equation of the dividend in the dividend discount model**:
$$\mathrm{\sum PV_div=\sum_{t=1}^{\infty}\frac{D_t}{(1+r)^t}=\frac{D_1}{(1+r)^1}+\frac{D_2}{(1+r)^2}+...+\frac{D_N}{(1+r)^N}}$$
where $D_t$: dividend at time t; $r$: required rate of return.
It makes no sense to estimate dividends too far out into the future. Therefore, we have to assume from some point onward the **growth rate (g) of dividends to be constant**.

Since we now have a constant growth rate, every future dividend can be expressed in terms of the current or most recent dividend payout, which we denote as did not.

The **equation of the dividend in the Gordon growth model**, with the assumption of **constant growth rate of dividends (g)**:
$$\mathrm{\sum PV_div=\sum_{t=1}^{\infty}\frac{D_t}{(1+r)^t}=\frac{D_0(1+g)^1}{(1+r)^1}+\frac{D_0(1+g)^2}{(1+r)^2}+...+\frac{D_0(1+g)^N}{(1+r)^N}}$$
where the **growth rate of dividend is assumed to be at constant rate**, which can be summarised to:
$$\mathrm{V_0=\frac{D_0(1+g)}{r+g}}$$
where ${V_0}$: intrinsic value of stock; ${g}$: growth rate of dividend; $r$: required rate of return; $D_0(1+g)$: next period's dividend. **Note:** the numerator is the dividend for the following year, which you have to multiply $D_0$ by the **growth rate (g)** to estimate it.

If **$D_1$ (next period's dividend)** is known,
$$\mathrm{V_0=\frac{D_1}{r+g}}$$
where ${V_0}$: intrinsic value of stock; ${D_1}$: next period's dividend; $r$: required rate of return; ${g}$: growth rate of dividend.

The **Gordon growth model** have several **assumptions** and **limitations**:
- **Dividends** are the **correct metric** for valuation purposes - however, some early stage companies **pay little or no dividend**
- **dividend growth rate (g)** is forever constant (i.e. perpetual and never changes)
- **required rate of return (r)** is also constant over time.
- the **required rate of return (r)** is strictly greater than the **dividend growth rate (g)**  (i.e. r>g)

The Gordon growth model **characteristics**:
- the stock value is very sensitive to the difference between the **required rate of return (r)** and the **dividend growth rate (g)** 
- when the r-g narrows, the stock price increases; when the r-g widens, the stock price decreases

The stock value due to **dividend growth rate**, we assume the **growth rate is 0%**:
$$\mathrm{V_0=\frac{D_1}{r}}$$
where $V_0$: intrinsic value of stock price; $D_1$: dividend (which remains unchanged); $r$: required rate of return.

and from there **stock value due to dividend growth**, we use an estimate of intrinsic value with positive growth rate minus estimate using 0 growth:
$$\mathrm{Stock\,value\,due\,to\,dividend\,growth=V_{E+}-{V_{0G}}}$$
where $V_{E+}$: intrinsic stock value using positive growth rate; $V_{0G}$: intrinsic stock value of 0 growth rate.

![[Screenshot 2023-05-21 at 11.52.05.png]]
![[Screenshot 2023-05-21 at 11.52.58.png]]
![[Screenshot 2023-05-21 at 12.15.32.png]]
![[Screenshot 2023-05-21 at 12.20.24.png]]

### Multistage dividend discount model
**2-stage dividend discount model** is where:
- the **growth rate** differs between the two stages
	- i.e. **g*:initial growth rate** and **g: constant growth rate**. 
- often used to model **rapidly growing companies** where they are expected to experience an **initial finite period of high growth**, but **slowing to an infinite period of sustainable slower growth**.

The **Gordon growth model** can be used to **estimate the value for the second phase of growth (g)**, but **the value has to be discounted back to its present value**.

The **2-stage dividend discount model** equation is as follows: 
$$\mathrm{PV_stock=\sum PV_div+PV \,of\,\frac{D_0(1+g)}{(r-g)}}$$
where $PV_{div}$: discounted value of dividend; and discounted value of the **Gordon growth model**; $g$: constant dividend growth rate.

which **2-stage dividend discount model** can also be expressed as :
$$\mathrm{PV_stock=\sum \frac{D_t}{(1+r)^t}+ PV\,of\,\frac{D_0(1+g)}{(r-g)}}$$
where $D_t$: dividend; $r$: required rate of return; discounted value of the **Gordon growth model**; $g$: constant dividend growth rate.

![[Screenshot 2023-05-21 at 12.21.29.png]]
![[Screenshot 2023-05-21 at 12.28.02.png]]

### Estimate growth rate 
There are 3 ways of estimating the **dividend growth rate (g)**:
- Use the **historical growth** in dividends for the firm - not for the firms with irregular/erratic history of dividend payouts
- Use the median **industry** dividend growth rate - does not reflect the true potential of the company
- Use the **firm's sustainable growth rate** 

The **sustainable growth rate ($g$)** equation is as follows:
$$\mathrm{g = ROE \times Retention\,rate}$$
where **ROE** equation is as follow:
$$\mathrm{ROE =\frac{Net\,income}{Avg.\,shareholders'\,equity}}$$
where **retention rate** equation is as follows:
$$\mathrm{Retention\,rate=(1-Dividend\,payout\,ratio)}$$
where **dividend payout ratio** equation is as follows:
$$\mathrm{Dividend\,payout\,ratio = \frac{Dividends\,paid}{Net\,income}}$$

The **sustainable growth rate** has several assumptions:
- ROE remains constant
- Dividend payout ratios remain constant
- No new equity sold

> A company had a net income of $1.5 million and the beginning owner’s equity on its books was $12 million. The company paid $600,000 dividend to common stockholders and it does not have any preference stockholders.
> 
> Calculate the sustainable growth rate of the company based on the information given.
> ROE = Net Income to common / Total Equity = $1.5M / $12M = 12.5%
> Dividend payout ratio = Dividend paid / Net Income = 0.6/1.5 = 40%
> g = ROE x (1-Div Payout Ratio) = 0.125 x (1-0.4) = 7.5%


### Choosing appropriate model
For choosing the appropriate present value model:
- **Dividend discount model** - not practical to estimate every future dividend
	- **Gordon growth model** - assumption: single constant growth rate in perpetuity; appropriate for: stable and mature, non-cyclical, dividend-paying firms
	- **Multistage growth model** - 
		- **2-stage growth model** - assumption: initial high growth rate, constant sustainable long-term growth rate; appropriate for: firms with high current growth rate that will drop to a stable rate in future
		- **3-stage growth model** - assumption: 3 stages of growth, transition, maturity; appropriate for: firms with high current growth rate, followed by transitional lower growth rate, followed by constant growth rate in the long run.
- **Free cash flow to equity (FCFE) model** - assumption: firm's earning growth rate can be estimated; appropriate for: non-dividend paying firms, firms with uncertain future dividends

![[Screenshot 2023-05-21 at 17.41.35.png]]
![[Screenshot 2023-05-21 at 19.39.23.png]]

## Multiplier models - Price multiple model
### Price multiples
**Price multiple** computes a ratio that has the stock price as the numerator and affirm fundamental as the denominator, common price multiples used:
- **price-to-earnings (P/E) ratio**, the company's stock price divided by its earnings per share (EPS) - it could be **leading (forecast 12 months EPS)** or trailing **(past 12 months EPS)**
- **price-to-sales (P/S)** ratio, the stock price divided by the **sales per share**
- **price-to-book (P/B)** ratio, the stock price divided by **book value of equity per share.**
- **price-to-cash flow (P/CF)** ratio, the stock price divided by **cash flow per share**; where the **CF could be operating CF or free CF**

### Benefits of using price multiples
The benefits of using price multiples:
- most listed companies are available from media outlet
- easy to calculate
- time-series and cross sectional comparison
- useful for predicting stock returns

Many of these ratios have been shown to be useful for predicting stock returns, where stocks with low multiples tend to produce higher future returns.

### Disadvantage of using price multiples
The disadvantage of using price multiples:
- The fundamentals were used are mostly trailing (historical data)
To overcome this issue, some of the analysts use forward data, however, should ensure consistency when making comparisons

The **price multiples** can then be compared using:
- **based on fundamentals** - based on some valuation model
- **based on comparables** - other firms or own historical multiples

### Based on fundamentals
**Multiples** based on fundamentals such as **Gordon growth model** - have the forward dividend ($D_1$) divided by **forward earnings** ($E_1$; next year projected earnings) in the numerator.

The **price multiples of gordon growth model equation of forward P/E** is as follows:
$$\mathrm{P_0/E_1=\frac{D_1/E_1}{r-g}}$$
where $P_0$: price of this interval; $E_1$: projected next year EPS; $D_1/E_1$: expected dividend payout ratio for the next period; $r$: required rate of return of the stock; $g$: constant growth rate of dividends.

$E_0$ = trailing EPS
$E_1$ = forward EPS

$P_0/E_0$: lagging/trailing P/E ratio
$P_0/E_1$: forward/leading P/E ratio (**justified P/E**) based on the PV of the future cash flows

![[Screenshot 2023-05-21 at 18.06.32.png]]
![[Screenshot 2023-05-21 at 18.45.49.png]]

If other things equal:
$D_1/E_1$: Expected dividend payout ratio - if $D_1/E_1$ ↑ Justified P/E ↑
$r$: required rate of return of the stock - if  $r$ ↓ ⇒ Justified P/E ↑
$g$: constant growth rate of dividends - if  $g$ ↑ ⇒ Justified P/E ↑

However, in practice, other things are not equal.

**Dividend displacement of earnings** where the $D_1/E_1$ ↑ ⇒ Justified P/E ↑;  $g$ ↓ ⇒ Justified P/E ↓ since the **sustainable growth rate** = ROE $\times$ (1-div payout ratio). Therefore, the net effect of ↑ dividend payout ratio is ambiguous. Intuitively, it makes sense that firms cannot continually increase their market values by increasing the dividend payout ratio.

![[Screenshot 2023-05-21 at 18.57.25.png]]

> It can also be done through calculation, reminder of the sustainable growth rate equation is as follows:
> $$\mathrm{g = ROE \times Retention\,rate}$$Pincher corp sustainable growth rate ($g_{Pincher}$) is: 12.6% $\times$ (1 - 34.5%) = 8.2%
> Industry average sustainable growth rate ($g_{Industry}$) is: 16.7% $\times$ (1 - 34.1%) = 11.1%
> Also, the higher D/E ratio suggest high risk firm and higher required rate for equity. 
> Therefore, the **justified P/E (forward P/E)** should be lower than industry average.

### Based on comparables
Under this approach, the **price multiples** of the subject firm is **compared against the benchmark** to evaluate the **relative valuation** of its stocks.

Common benchmarks include:
- **time series comparison** - historical multiple
- **cross-sectional comparisons** - all stocks of companies and industry multiples; although not identical, but **comparable** ⇒ should have approximately same multiples

The **economic principle** guiding this method is the **law of one price**, which asserts that **two identical assets should sell at the same price**.

When comparing between different firms, should consider similarities across a number of dimensions:
- **Company size**
- **Product lines**
- **Growth rate**

![[Screenshot 2023-05-21 at 19.04.59.png]]

### Fundamentals vs. comparables
The analyst should make a judgment on which approach is more appropriate for the company being studied.

**Benefits of using comparables**: 
- may be simpler for analysts who are familiar with the particular industry.
- price multiples of various listed companies are readily provided

**Disadvantage** of using **comparables**:
- different accounting methods can result in price multiples that are not comparable across firms, especially internationally
- price multiples for cyclical firms may be greatly affected by economic conditions at a given point in time.

**Benefits** of using **fundamental** approach:
- no need to identify comparables for the company,

**Disadvantage** of using **fundamental** approach:
- estimating the required return ($r$) for the stock and the growth rate ($g$) can be challenging; and Gordon growth model are very sensitive to these two variables
- price multiples for cyclical firms may be greatly affected by economic conditions at a given point in time.

In this case, the price-to-sales (P/S) ratio may be more appropriate because the sales are less volatile than earnings.

## Multiplier models - Enterprise value model
**Enterprise value** is a measure of the **total value of a company** and often viewed as the **cost to acquire the company**.

The cost of the **enterprise value** is as follows:
$$\mathrm{Enterprise\,value=Common\,stock-Pref\,stock-Debt\,-(Cash + ST\,investments)}$$
where **common stock**, **preferred stock** and **debt** are of **market value**. However, market value of firms' debt are often unavailable.

Therefore, to estimate the **market value of bonds**:
- estimate from market value of **comparable bonds**
- use **book values** (unsuitable if market conditions have changed)

Since enterprise value takes into account both equity and debt of the company, it's an appropriate measure when comparing firms that have significantly different capital structures.

### Enterprise value multiple
The **enterprise value multiple** are often calculated with:
- **EV/Revenue** 
- **EV/EBITDA** - the **EBITDA is a proxy for CFO**; benefits of using EBITDA: is usually positive even when net income or cash flow is negative; EBITDA often includes non-cash revenues and expenses.

$$\mathrm{Enterprise\,value\,multiple=\frac{EV}{EBITDA}}$$
where the numerator represents the values of both equity and debt, the earnings available to both shareholders and creditors. Earnings before interest, since the interest is payment to creditors.

![[Screenshot 2023-05-21 at 10.40.47.png]]

For the **intrinsic value of common stock**, substitute the intrinsic EV in the EV equation:
$$\mathrm{Intrinsic\,EV=EBITDA\times Enterprise\,multiple}$$
**Intrinsic value per share**:
$$\mathrm{Intrinsic\,value\,per\,share=\frac{Intrinsic\,EV}{\#\,of\,shares\,outstanding}}$$
![[Screenshot 2023-05-21 at 10.41.19.png]]

## Asset-based valuation models
**Asset-based valuation models** **adjusts** the **fair value** of all the assets of the firm and the fair value of all the firm's liabilities. 

As we know that the from the balance sheet, 
$$\mathrm{Asset=Liabilities+Preferred\,stocks+Equity}$$
then, from rearranging the equation:
$$\mathrm{Equity=Asset-Liabilities-Preferred\,stock}$$

The **intrinsic value of the common stock through asset-based valuation equation** is as follows:
$$\mathrm{Intrinsic\,value\,per\,share=\frac{(Assets-Liabilities-Preferred\,stock)}{\#\,of\,outstanding\,shares}}$$
where **assets**, **liabilities** and **preferred stock** should use **fair value (i.e. adjusted book value)**.
which will give the intrinsic value per share.

### Fair value of assets and liabilities
**Balance sheet values** can be quite different from **fair values**.
There are 3 major ways to adjust the fair values:
- Depreciated values
- Inflation-adjusted depreciated values
- Estimated replacement values

### Issues with asset-based valuation model
There are several issues with using the asset-based valuation model:
- **Assets (PP&E) can be difficult to value** - specific information about these assets may not be made publicly available and values of these assets can be very subjective
- **Intangibles** - some intangible assets are recorded on the balance sheet (e.g. goodwill and copyright), while other are not (e.g. brand value, reputation and customer loyalty), difficult to quantify the effect of intangibles

This type of approach can give a **'floor' value** of the stock that is stripping out all the intangibles, the company's stock is worth at least this amount.

For a company that has significant intangibles, the analyst should consider supplementing these value with a more forward looking valuation, e.g. a **present value model**. This is the reason why this model is often a last resort for many analysts when no other valuation method is appropriate (e.g. private companies).

![[Screenshot 2023-05-20 at 23.19.07.png]]

## Summary of valuation models

![[Screenshot 2023-05-21 at 19.39.52.png]]
![[Screenshot 2023-05-21 at 17.41.35.png]]
![[Screenshot 2023-05-21 at 19.39.23.png]]


---
## Questions before starting this section:
- [ ]

## Codes to test understanding of objectives