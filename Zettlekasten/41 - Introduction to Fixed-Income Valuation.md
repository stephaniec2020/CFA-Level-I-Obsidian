
# 41 - Introduction to Fixed-Income Valuation
202302281740
Status: #📥 
Tags: [[CFA Level I]]

## Objectives:
- [ ] calculate a bond’s price given a market discount rate.
- [ ] identify the relationships among a bond’s price, coupon rate, maturity, and market discount rate (yield-to-maturity).
- [ ] define spot rates and calculate the price of a bond using spot rates.
- [ ] describe and calculate the flat price, accrued interest, and the full price of a bond.
- [ ] describe matrix pricing.
- [ ] calculate annual yield on a bond for varying compounding periods in a year.
- [ ] calculate and interpret yield measures for fixed-rate bonds and floating-rate notes.
- [ ] calculate and interpret yield measures for money market instruments.
- [ ] define and compare the spot curve, yield curve on coupon bonds, par curve, and forward curve.
- [ ] define forward rates and calculate spot rates from forward rates, forward rates from spot rates, and the price of a bond using forward rates.
- [ ] compare, calculate, and interpret yield spread measures

---

## Bond Price and Time Value of Money
**Bond pricing** is through discounted cash flow, if a bond is due to return 100 at par value, the current amount is 90.91 if we discounted at 10%.

![[Screenshot 2023-02-28 at 17.49.55.png]]

As for a 5-year bond, the discounted cash flow has to be the sum of all discounted cash flow for each year, including the coupon payment and market discount rate to obtain the value of present value by using the TVM function of the calculator.

![[Screenshot 2023-02-28 at 17.52.09.png]]

### Market Discount Rate
**Market discount rate** depends on the investor's required rate of return, and normally the present value will be the par value of the bond at initial year of investment. 

However, as the time past since the date of acquiring the bond, there might be several factors that might affect the bond price (thus the yield of the bond):
- Interest rate environment
- Issuer's credit quality
- Time to maturity

The yield of the investors requirement can change due to the several factors mentioned above, the new **market discount rate** will be the investors' updated required yield for the bond for investment.

The bond **fair market value** is **trading at premium** as the bond price is traded above its par value when the investor demand in **lower yield of bond (i.e. lower market discount rate)**.

![[Screenshot 2023-02-28 at 17.57.20.png]]

The bond **fair market value** is **trading at a discount** compare to its par value as the investor require a **higher yield of bond (i.e. higher market discount rate)** due to any of the factors changed (e.g. issuer's credit quality decreases).

![[Screenshot 2023-02-28 at 18.00.02.png]]

There is an **inverse relationship** between **market discount rate (i.e. yield)** and **price**:

|Market Discount Rate | Coupon Rate | Description |
|----|----|----|
|10%|10% | Par|
|8%|10% | Premium|
|12%|10% | Discount|

Although some bonds payout annually for coupon, but the majority of the bonds payout **semi-annually**. These follow calculations of the **fair market value** of the bond price is positioned on coupon payment date to compute the price value based on whole period.

![[Screenshot 2023-02-28 at 18.07.21.png]]

### Yield-to-maturity
We can use the **bond price** to calculate the **cash flow**, thus the **yield-to-maturity (i.e. the market discount rate)**.

![[Screenshot 2023-02-28 at 18.10.25.png]]

For the calculation now, is to calculate the **IRR (yield-to-maturity)**, since it is doing semi-annual payment, needs to $\times 2$ to calculate the annual yield-to-maturity.

The investor will only realise the 14% YTM if:
- Bond is held to maturity
- The issuer does not default on any of the scheduled payments
- All coupon received are reinvested immediately at the same yield of 14%.

### Price vs Yield
There are several effects that affect the **price/yield relationship**:
- Inverse effect
- Convexity effect
- Coupon effect
- Maturity effect

#### Inverse effect
There is an **inverse relationship** between **market discount rate (i.e. yield)** and **price**:

|Market Discount Rate | Coupon Rate | Description |
|----|----|----|
|10%|10% | Par|
|8%|10% | Premium|
|12%|10% | Discount|

#### Convexity effect
The **price/yield relationship** shares a **convexity effect**. **Convexity effect** means that the percentage decrease in value when the yield increases by a given amount is smaller than the increase in value when the yield decreases by the same amount.

Convexity demonstrates how the duration of a bond changes as the interest rate changes.
If a bond's duration increases as yields increase, the bond is said to have negative convexity.
If a bond's duration rises and yields fall, the bond is said to have positive convexity.

![[Screenshot 2023-02-28 at 18.15.58.png]]
https://www.investopedia.com/terms/c/convexity.asp

#### Coupon effect
**Coupon effect** is when although there is a same time to maturity, the lower coupon bond has a greater percentage price change than a higher coupon bond, where the market discount rates change by the same amount.

![[Screenshot 2023-02-28 at 18.25.58.png]]

Bonds with a higher coupon rate have lower price volatility. 

#### Constant yield price trajectory
If the yield has not changed for the remaining period, this conversion to par value at maturity is known as the **constant yield price trajectory.** Regardless of whether the **market discount rate is above or below** the **bonds coupon rate**, the price **always converges to the par value**.

![[Screenshot 2023-02-28 at 18.29.07.png]]

#### Maturity effect
**Maturity effect**, generally speaking when the bond is further from maturity has a greater price sensitivity to a change in market discount rate than a bond that is closer to maturity.

![[Screenshot 2023-02-28 at 18.32.04.png]]

### Spot rates
**Spot rates** are the more fundamental approach of using a sequence of **market discount rate** that correspond to the **cash flow dates**.

If we isolate the cash flows, each of them can be viewed as a zero coupon bond maturing at the date of the cash flow, the **spot rate** can be viewed as the **yield of the zero coupon bond**.

![[Screenshot 2023-02-28 at 18.33.48.png]]

The PV of the bond can't be calculated by the TVM calculator, instead it has to be treated as zero-coupon bond where each cash flow is calculated separately, where the principle value is the last one.

Example question:
Remember semi-annual means that the **coupon rate** has to be $\div 2$, so as the **discount factor** has to $\div 2$. Then apply the PV to get the I/Y, and I/Y $\times 2$ to get the annual yield-to-maturity.
![[Screenshot 2023-02-28 at 18.45.38.png]]

### Flat price vs full price

In reality, those trades are made in between coupon payment dates. For instance, if coupon payment dates are first of April and 1st of October and we want to determine the price of the bond on the 1st of June based on a market discount rate of 12.6%, how do we calculate its price?

![[Screenshot 2023-02-28 at 18.50.54.png | 600]]

As the coupons are paid to the bondholder, the coupon should no longer be factored into the price. This accounts for the sharp drop in price on every coupon payment date. This price is known as the **full price** or **dirty price**.

![[Screenshot 2023-02-28 at 18.51.33.png]]

The **full price** is the price an investor pays or receives when a trade is made, ignoring the effect of spread.

The **full price** of the 

![[Screenshot 2023-02-28 at 18.57.15.png]]
where MDR is the market discount rate.

**Accrued interest** is the coupon $\times$ the proportion of the days held for the coupon.
The equation of **accrued interest** is as follows:
$$\mathrm{Accrued\,interest=Coupon \times Proportion}$$
The coupon dates and dates of holding the coupon depends on the actual number of days (i.e. the actual/actual method) or 30/360 (for corporate bond).


#### Flat price
The **flat price** or **clean price** is quoted ignoring the effects of accrued interest, it is equal to the quoted price. This is the price quoted by bond dealers. So, in effect, the difference between the full price and the flat price is the accrued interest.

For example, on the 1st of June, a bond dealer will quote the price of the bond at X dollars, which
is its flat price. If a buyer wants it, she has to pay not just the quoted price, but also the accrued interest to the seller. This is because the buyer will receive the full coupon payment of 50 dollars on the next payment date, which is the 1st of October. But rightfully part of this payment belongs to the seller who held the bond for two out of the six months of this period.

The equation of **flat price** is as follows:
$$\mathrm{Flat\,price=Full\,price-Accrued\,interest}$$

#### Difference in calculation of accrued interest 
**Accrued interest calculation** differs depending on the type of bond held. 
**Government bonds** - Actual/Actual method - uses the actual number of days
**Corporate bonds** - 30/360 method - assumes 30 day a month and 360 day a year

Corporate bond yields are typically based on a 30/360 day count. When calculating spreads, corporate yields are often restated to the actual/actual basis typically used to state government bond yields

![[Screenshot 2023-02-28 at 19.03.53.png]]

Example for calculation of **full price**, **accrued interest**. and **flat price**:
If the bond does not say the **future value**, automatically assume the **par value is at $100**.

The **full price** equation is as follows:
$$\mathrm{Full\,price = Price \times (1+MDR)^{adjusted\,num\,of\,days}}$$
where the MDR has to be adjusted, if the bond is semi-annual bond, the MDR/2 to get the value.

![[Screenshot 2023-02-28 at 19.16.57.png]]

### Matrix pricing
We have been using **market discount rate** to calculate the bond price, or using the bond price to calculate the **yield-to-maturity**. However, what should we do if we don't know either of them due to the bond **not being publicly/actively traded**, or **pricing new issuance**. 

![[Screenshot 2023-02-28 at 19.30.22.png |600]]

**Matrix pricing** is the estimation process where to estimate the market discount rate and price based on the quote or flat prices of more frequently traded comparable bonds, these comparable bonds should have similar credit quality to the bond of interest.

![[Screenshot 2023-02-28 at 19.21.29.png]]

The key is to use the rates of comparable bonds to estimate the **market discount rate** for the bond interested in. As we know, the discount rate tends to increase with the time to maturity as there is a **maturity risk premium**.

Our bond of interest has four years to maturity, none of these comparable bonds have four years to maturity, but we can use their yields to estimate its yield. We can use the **interpolation method**.

#### Interpolation method of estimation of market discount rate

![[Screenshot 2023-02-28 at 19.25.10.png]]

Since the relationship is linear, the increase in yield for the four year over the two year. The **yield -to-maturity** for Bond X should therefore be 6.55% + $\frac{2}{3} \times$ 1.25% = 7.38%.

![[Screenshot 2023-02-28 at 19.30.08.png]]

#### Matrix pricing through yield spread + benchmark
**Matrix pricing** can also be used to calculate **pricing new issuance**. The principle is to get an estimate of the required **yield spread** + the **benchmark rate**. 

The **yield spread** is the compensation for additional credit and liquidity risk and the difference in tax status compare to government bonds.

**Benchmark rate** is the yield-to-maturity of a government bond.

![[Screenshot 2023-02-28 at 19.30.44.png]]

At any time, there are government bonds trading with various times to maturity so we can form a continuum known as the **yield curve**. 

For a particular issuer or issuers with similar credit quality, the bonds also trade at various times to maturity at various spreads above the yield curve to compensate with the additional **credit** and **liquidity risk**.

![[Screenshot 2023-02-28 at 19.35.07.png]]

So, for example, if a company wants to issue a bond of 10 years to maturity, we can estimate the

benchmark yield as the midpoint between the yields of government bonds with nine and 11 years to maturity.
![[Screenshot 2023-02-28 at 19.36.10.png]]

![[Screenshot 2023-02-28 at 19.36.24.png]]

Example question:
Remember to convert the corporate bond to the yield spread and calculate the spread, then add the market discount rate of the new corporate bond.
![[Screenshot 2023-02-28 at 19.39.38.png]]

## Bond yield measure
**Effective yield measurement** as the coupon payout rate increases, the effective yield is higher than the ones with lower payment frequency.

![[Screenshot 2023-02-28 at 21.19.47.png]]

### Effective annual rate (EAR)
- Effective annual rate = How much interest is effectively given out in a year, allow us to compare interest rate with different compounding period, and here is the equation:

$$EAR = (1+r)^N -1$$
where EAR: Effective annual rate; r: periodic interest rate; N: number of compounding period $(1+r)^N$: Future value factor 

and 

- Periodic interest rate ($r$) = annual interest rate ($IR$)/compounding frequency in a year ($n$)
$$r = \frac{IR}{n}$$
where r: periodic interest rate; IR: annual interest rate; n: number of compounding frequency in a year

### Fixed rates bonds 

#### Yield-to-maturity vs effective yield
The difference between **yield-to-maturity** and **effective yield**.

The equation for **effective yield** is as follows:
Gather information of N, PV, PMT, FV ⇒ I/Y (Yield per time period)
$$\mathrm{Effective\,yield = (1+I/Y)^{coupon\,freq} -1}$$

![[Screenshot 2023-02-28 at 21.23.27.png]]

![[Screenshot 2023-02-28 at 21.23.38.png]]

There are also other factors such as the coupon payment date, if the coupon payment date lands on a weekend, the payment will have to delay till the day of payment. 

For example, 

![[Screenshot 2023-02-28 at 21.26.53.png]]

#### Resolution towards government bond yield and corporate bond yield calculation difference
**Government bond yields** are usually quoted on an **actual/actual** day count basis. On the other hand, **corporate bond yields** are usually quoted on the **30/360 basis**.

30/360 basis - The convention is a 30 day month, 360 day year, regardless of the actual number of days.

A **government equivalent yield** is quoted for a corporate bond, a government equivalent yield restates a yield to maturity for a corporate bond to one based on the actual actual convention.

The government equivalent yield on a corporate bond can be used to obtain the spread over the government yield, doing so keeps the yield stated on the same day count convention basis.

![[Screenshot 2023-02-28 at 21.30.40.png | 240]]

#### Current Yield
**Current yield** is the sum of the coupon payments in a year over flat price. 

The equation to calculate current yield is as follow: $$\mathrm{Current\,yield = \frac{\sum Coupon\, payments\,in\,a\,year}{Flat\,price}}$$
The **current yield** is a **crude measure** of the **rate of return** to an investor.

**Shortcoming of current yield**: It does not consider capital gains or losses, which, does not include the realisation of a capital gain if held to to maturity.

![[Screenshot 2023-02-28 at 21.38.09.png]]

#### Simple Yield
**Simple yield** is the straight-line amortised share of gain/loss + sum of the coupon payments in a year over flat price. 

$$\mathrm{Simple\,yield = \frac{Straight\,line \, amortised\,share\,of\,gain/loss+\sum Coupon\, payments\,in\,a\,year}{Flat\,price}}$$

![[Screenshot 2023-02-28 at 21.38.01.png]]

![[Screenshot 2023-02-28 at 21.39.00.png]]
If the bond embedded with callable options, the bond allows the issuer to buy back the bond from the investors at one callable dates (European)/ any days after the callable date (American)/ specified dates after first call date (Bermuda style).

There are multiple styles to be called:
- European style - only on specified call date
- American style - any time after call date
- Bermuda style - specified dates after first call date

For the investors in callable bonds, the bond yield depends on when the issuer decided to call back the bond. The bond yield can be determined by the . The **yield-to-worst** is the mimimum of yield-to-calls compare to the yield to maturity (min(yield-to-calls, yield-to-maturity)).

Another method of accessing the callable bond is the **option adjusted yield**,  

The equation is as follows: 

$$\mathrm{Flat\,price\,callable\,bond + Value\,call\,option = Option\,adjusted\,price}$$
However, be mindful that this is not the price of what the investor pays, the investor pays the price + accrued interest. Since the value of the call option can never be negative, the option adjusted price will always be $\le$ to flat price.

![[Screenshot 2023-03-03 at 16.19.13.png]]

![[Screenshot 2023-03-03 at 16.19.29.png | 400]]

The flat price allows to calculate yield-to-maturity, while the option adjusted price allow to calculate the option adjusted yield.

The **yield-to-maturity** has a higher yield to compensate the bond holders for issuer’s call option and **option adjusted yield** used to compare yields of bonds with different options/straight bonds.

### Floating rates bonds 
**Floating rate bonds** coupons are given out as the reference rate $\pm$ fixed margin, the fixed margin determined by the credit risk of the issuer compare to the credit risk of the reference (e.g. 180 day LIBOR). The initial fixed margin is called the **”quoted margin”**. 

In order to simplify the calculation for discounted cash flow, since we don’t know the future reference rate, we would have to use the latest **coupon rate**, (I.e. Latest 180-day LIBOR + quoted margin). -> coupon payment

**Discount rate** is the reference rate + discount margin (I.e. Latest 180-day LIBOR + discount margin). The **discount margin** is the credit risk of the issuer to the credit risk of reference, however this margin is not fixed. Therefore, we need to use the latest discount margin. -> yield

![[Screenshot 2023-03-03 at 16.20.33.png]]
Discount margin: I/Y
Quoted margin: PMT

The **coupon rate** equation for floating rate note is calculated as follows:
$$\mathrm{Coupon\,rate = 180d\,LIBOR + quoted\,margin}$$
where then this figure is used in **PMT** for TVM calculation.

The **discount rate** equation for floating rate note is calculated as follows:
$$\mathrm{Discount\,rate = 180d\,LIBOR + discount\,margin}$$
where then this figure is used in **I/Y** for TVM calculation.

### Money market securities
**Money market securities** are short-term debt securities, with maturities $\le$ 1 year. 

There are the three most common ones issued by different institutes:
- US T-bills - government issues
- Commercial paper - corporate issues
- Certificate of Deposits - bank issues

There are difference in quoting the yield through **discount basis** and **add-on yield**. The money market securities also are quoted on a basis of either a 360 day basis or 365 day basis.

The **US T-bills** are quoted on discount basis at 360 days, **commercial paper** are quoted on discount basis or add-on yield at 360 days. The certificate of deposits are add-on yield with either 360-day or 365-day. Nevertheless, the money market instruments are quoted on **simple annual interest** basis vs with bonds which are quoted on **compounding interest basis**.

![[Screenshot 2023-03-03 at 16.21.28.png]]

#### Compare the yield between different quoted interest
1. Calculate the actual payment given its quoted interest or yield
2. Compare yields that are quoted on different yield bases.

US T-bills, commercial paper, and certificate of deposit
Equivalent add-on yield = discount coupon/price at issuance
For 365 days = add-on yield of 90 days x 365/90 = 

![[Screenshot 2023-03-03 at 16.20.59.png]]

#### Compare the yield between different semi-annual coupon bond
**Calculate the bond equivalent yield**
1. Convert holding period yield 
2. Effective semi-annual yield
3. Multiply by 2 to calculate the bond equivalent yield

![[Screenshot 2023-03-03 at 16.22.01.png]]

## Maturity structure of interest rate 
### Yield curve
**Yield curve** is the relationship between the interest rate/bond yield to the time-to-maturity.

There are several types of yield curves depending on the context:
- Coupon bonds
- Spot rate
- Par bond

#### Coupon bonds yield curve
The US treasuries in the market, there are different **times-to-maturity**, **coupon rates**, **yields-to-maturity**. The yield curve is plotted by the data points of respective coupon bonds, and the missing values are interpolated by linear interpolation. 

When interpreting the information, the analyst must make sure the currency, credit risk, periodicity, liquidity, and coupon rates are similar to make comparable analysis. However, the coupon rate can vary a lot, it goes against the rule of keeping the coupon rate at similar comparable level.

![[Screenshot 2023-03-03 at 16.22.26.png]]

#### Spot rate yield curve
**Spot rate yield curve** solves the problem of coupon bonds yield curve as it is using zero-coupon bonds to calculate the yield curve. However, the US T-bonds and T-notes are mainly coupon-bearing bonds. We can utilise stripped bonds, where the **coupon payments** and **principal repayments** are stripped into separate components and sold separately. 

The **spot curve** is also known as the **”stripped curve”**/**”zero curve”**, often interpreted as “risk-free”rate.

![[Screenshot 2023-03-03 at 16.23.34.png]]
![[Screenshot 2023-03-03 at 16.23.20.png]]
#### Par curve yield curve
**Par curve yield curve** is calculated from a spot curve. The **coupon rate** that a hypothetical bond at each maturity would need to have to be **priced at par**. 

To price a bond, normally discount all the future cash flows using spot rates.
In this case, the PMT is unknown, not the price, the price = 100.

![[Screenshot 2023-03-03 at 16.23.51.png]]

The bond pricing using spot rate equation is as follows:
$$\mathrm{Price = \frac{PMT}{(1+S_1)}+\frac{PMT}{(1+S_2)^2}+\frac{PMT}{(1+S_3)^3}}$$


### Forward rates
**Forward rate** is the borrowing/lending rate for a loan to be at some future dates.  Besides for interest rate to determine the forward rate, the **loan commencement date** is also another important factor to determine the forward rate.

![[Screenshot 2023-03-03 at 16.24.16.png]]

**Notation** is today’s date till the time to loan commencement date, followed by the length of the loan.  

For example, for a loan 2y3y, is read as “2-yr into 3-yr rate”. It means 2 years to commencement with a 3 year loan.

![[Screenshot 2023-03-03 at 16.24.28.png]]

#### What does it mean by forward rate?
If a company requires a 2-year loan now, there are several options:
- Option A: take 2-year loan at spot rate (e.g. 3.0%)
- Option B: take 1-year loan at spot rate (e.g. 2.5%) and take 1y1y forward loan (e.g. 3.2%).

The AER is then calculated at:
Option A: Total interest cost: $(1.03)^2-1 = 6.09\%$
Option B: Total interest cost: $(1.025 \times 1.032)-1 = 5.78\%$(Geometric method)

**Principle of arbitrage**, the arbitrage will cease only when both are equal. The 1y1y will then be adjusted so that the option A and option B will be equal.

Spot-forward pricing relationship for 3 periods:
There are several options:
- 3 year loan at spot rate
- 1 year loan at spot rate + 1y1y forward loan + 2y1y forward loan
- 2 year loan at spot rate + 2y1y forward loan
- 1 year loan at spot rate + 1y2y forward loan

This is the 1 year loan at spot rate with 1y1y and 2y1y forward loan:
$$(1+S_3)^3 = (1+S_1)\times(1+1y1y)\times(1+2y1y)$$
Where 1y1y is the forward loan of 1 year ahead for 1 year period, and 2y1y is the forward loan of 2 year ahead for 1 year period.

This is the 2 year loan at spot rate with 2y1y forward loan:
$$(1+S_3)^3 = (1+S_2)\times(1+2y1y)$$

This is the 1 year loan at spot rate with 1y2y forward loan:
$$(1+S_3)^3 = (1+S_1)^1\times(1+1y2y)^2$$

The general spot-forward pricing relationship can be summarised at:
$$(1+S_B)^B = (1+S_A)^A\times(1+Ay(B-A)y)^{B-A}$$

This is known as the implied forward rate since it is calculated from the spot rate and not the actual market rate.

![[Screenshot 2023-03-03 at 16.25.09.png]]





missing last few slides



## Yield spreads
### Yield spreads over benchmark rates
Understand the spread between the **benchmark rate** and **yield-to-maturity**. It is influenced by the macroeconomic and microeconomic factors. 
Some of the macroeconomic factors mostly affect the bench market rate, and they are as follows:
- Expected inflation
- Economy/Business cycle
- Foreign exchange rates
- Monetary/fiscal policy

The microeconomic factors affect the spread, and they are as follows:
- Issuer’s credit risk/ratings
- Liquidity
- Tax status

![[Screenshot 2023-03-03 at 16.26.00.png]]

![[Screenshot 2023-03-03 at 16.26.15.png]]
Risk free rate of return + risk premium


The benchmark + spread names are as follows:
![[Screenshot 2023-03-03 at 16.26.40.png]]

#### Comparison of 3 year corporate bond vs US T-notes
3-year corporate bond with 3 years to maturity should use **on-the-run** (i.e. recently-issued bond, yield more representative of current market) **US T-notes** with 3 years to maturity.

#### Unconventional maturity date
The G-spread with interpolated yield between 2 US T-notes.  For example, there is a corporate bond which 3.2 years to maturity, having a 5.48% yield; since US T-note has only 3 years to maturity and 3.5 years to maturity, therefore use this interpolated rate to calculate the G-spread.

#### Calculate swap rate and I-spread (interpolated spread)
The benchmark uses the interest swap rate with the same currency and same time-to-maturity. Interpolated spreads are used for bonds denoted in Euros. For example, the corporate bond in Euros (EUR) with 3 year maturity date, it is compared with the 3-year EUR swap rate. 

### Yield spreads over benchmark yield curve
In the previous section, the spread is the YTM of bond - the benchmark rate of the bond through discounting all the future cash flow of the bond. However, this might not be the most suitable model as the benchmark yield curves tend to be upward sloping as investors demand a premium for holding longer-term securities.

![[Screenshot 2023-03-03 at 16.27.00.png]]

In order to compensate the upward-sloping yield curve, to add the ‘Z’ on top of every spot rate, which is known as the zero-volatility spread (z-spread). 
To solve for Z, use a computer or use trial and error.

For bonds with embedded options, z-spread can also be used for option-adjusted spread (OAS). The callable bond subtract the option value in bps/year. 

$$\mathrm{Option\,adjusted\,spread = Z\,spread-Option\,value}$$

For rearrangement of the equation to get this:

$$\mathrm{Z\,spread = Option\,adjusted\,spread+Option\,value}$$
where the z-spread is the spread for callable bond, OAS: the spread for equivalent straight bond; Option value: extra yield as compensation for call.

 
![[Screenshot 2023-03-03 at 16.27.48.png]]

![[Screenshot 2023-03-03 at 16.28.08.png]]






---
## Questions before starting this section:
- [ ]