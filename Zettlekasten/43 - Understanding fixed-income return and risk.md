# 43 - Understanding fixed-income return and risk
202305231813
Status: #📥 
Tags: [[CFA Level I]]

## Objectives:
- [ ] calculate and interpret the sources of return from investing in a fixed-rate bond.
- [ ] define, calculate, and interpret Macaulay, modified, and effective durations
- [ ] explain why effective duration is the most appropriate measure of interest rate risk for bonds with embedded options.
- [ ] define key rate duration and describe the use of key rate durations in measuring the sensitivity of bonds to changes in the shape of the benchmark yield curve
- [ ] explain how a bond’s maturity, coupon, and yield level affect its interest rate risk.
- [ ] calculate the duration of a portfolio and explain the limitations of portfolio duration.
- [ ] calculate and interpret the money duration of a bond and price value of a basis point (PVBP).
- [ ] calculate and interpret approximate convexity and compare approximate and effective convexity.
- [ ] calculate the percentage price change of a bond for a specified change in yield, given the bond’s approximate duration and convexity.
- [ ] describe how the term structure of yield volatility affects the interest rate risk of a bond
- [ ] describe the relationships among a bond’s holding period return, its duration, and the investment horizon.
- [ ] explain how changes in credit spread and liquidity affect yield-to-maturity of a bond and how duration and convexity can be used to estimate the price effect of the changes.
- [ ] describe the difference between empirical duration and analytical duration.

---

## Sources of return for bonds
### Sources of return for fixed-rate bonds
There are 3 sources of returns from investing in a fixed rate bond:
- **Coupon + principal payments**
- **Reinvestment return** - coupons paid before the maturity date can be reinvested to earn interest up to the maturity date
- **Gain/loss** on the sale of the bond.

The reinvestment assumption that is embedded in any present value-based yield measure implies that all coupons and principal payments must be reinvested at the specific rate of return, in this case, the yield to maturity. Thus, to obtain a certain % of total dollar return, the investor must **reinvest all the coupons at the same certain % rate of return**. Total dollar return is made up of three sources, coupons, principal, and reinvestment income.

There are 2 main factors that can affect the returns:
- **Market interest rate** - prevailing interest rate after the purchase of the bond affects the reinvestment rate. If the market interest rate increases, the reinvestment rate for the coupons received can also be higher; the market price of the bond before maturity is also affected by the prevailing interest rates.
- **Credit quality** - coupon or principal payments may not be made on time if credit quality changed; can also affect the market price of the bond if the bond is to be sold prior to maturity.

### Effect of market price risk and reinvestment risk on returns of bonds
#### The market interest rate remains the same throughout the period
##### Hold-till-maturity investor and same market interest rate
The **rate of return** is the same rate as the **yield-to-maturity** at purchase. Fixed-rate-bond that has a reinvestment rate equal to the **yield-to-maturity**, an investor who holds the bond until maturity will earn a rate of return equal to the **yield to maturity** at purchase. This is regardless of whether the bond is purchased at a discount or at a premium.

**Yield-to-maturity** is an estimate of what the investor annual rate of return by calculating in the factor of today's price and hold till maturity. It is the internal rate of return (IRR) on expected cash flow. The CF calculation is detailed in the quantitative calculation. Yield-to-maturity has an inverse relationship to price. As the price of a bond goes up, the yield-to-maturity goes down.

![[Screenshot 2023-05-23 at 18.32.21.png]]

##### Sells before maturity investor and same market interest rate
In another case, sells the bond before maturity, the value of a bond that is sold at a discount or premium will move to its par value by the maturity date. If the yield never changes, the price follows the constant yield price trajectory. This is the carrying value of the bond to the investor over time and reflects the amortisation of the discount or premium since the bond was purchased. An investor who sells a bond prior to maturity will earn a rate of return equal to the yield to maturity and purchase **if the yield to maturity at sale has not changed** since purchase.

![[Screenshot 2023-05-23 at 18.35.06.png]]

#### The market interest rate increased throughout the period
##### Hold-till-maturity investor and market interest rate increase
If the market yield to maturity for the bond are assumed reinvestment rate increases after the bond is purchased but before the first coupon date, a buy and hold investors realised return will be higher than the yield to maturity of the bond when purchased.

For a **buy-and-hold investor,** the change in return due to a change in interest rate is solely because of the **change in reinvestment return**.

![[Screenshot 2023-05-23 at 18.39.42.png]]

##### Sells before maturity investor and market interest rate increase
The market price of the bond is affected by the market interest rate. If the market rate increases, this is lower than the price on the constant yield price trajectory. Capital losses occur if a bond is sold at a price below this trajectory. 

There are opposing factors that affect the investors returns that sells bonds before maturity when the market interest rates change.
The factors are:
- **Market price** - an inverse relationship with interest rates, the market price affects the capital gain or loss to the investor who sells before maturity.
- **Reinvestment rate** - a direct relationship to interest rates; affects the amount of reinvestment interest the investor receives.

When the market interest rate increases, the capital gain decreases, while the reinvestment interest increases. When interest rates decrease, the reverse happens. The **net effect on the rate of return depends on which component experiences greater change**.

![[Screenshot 2023-05-23 at 18.40.31.png]]

##### Sells before maturity investor and time horizon
As mentioned, the sells before maturity investor return depends on:
- **Market price** - an inverse relationship with interest rates, the market price affects the capital gain or loss to the investor who sells before maturity.
- **Reinvestment rate** - a direct relationship to interest rates; affects the amount of reinvestment interest the investor receives.
The **net effect on the rate of return depends on which component experiences greater change**.

If the **investment horizon is long**, the **coupon reinvestment risk dominates** over the return to the investor (i.e. The rate of return has a direct relation to market interest rates). 

If the **investment horizon is short, the market price risk dominates over the return to the investor.** (i.e. The rate of return has an inverse relation to market interest rates.) 

![[Screenshot 2023-05-23 at 18.54.36.png]]

#### The market interest rate decreased throughout the period
##### Hold-till-maturity investor and market interest rate decrease
For a buy-and-hold investor, the change in return due to a change in interest rate is solely because of the change in reinvestment return. If the market yield to maturity decreases, then the return to the investor will be lower.

![[Screenshot 2023-05-23 at 18.39.52.png]]

##### Sells before maturity investor and market interest rate decrease
The market price of the bond is affected by the market interest rate. If the market rate increases, this is lower than the price on the constant yield price trajectory. The price is higher than the price on the constant yield price trajectory. Capital gains occur if a bond is sold at a price above this trajectory.

When interest rates decrease, the capital gain increases, while the reinvestment interest decreases. The net effect on the rate of return depends on which component experiences greater change.

![[Screenshot 2023-05-23 at 18.40.22.png]]

### Conclusion on returns and risk of fixed-rate bonds
Th**e investment horizon** is the core of **interest rate risk and return**:
- **Hold-to-maturity investor** - only be concerned with reinvestment risk (i.e. hope that market interest rates increase so that the coupons can be reinvested at higher rates)
- **Investor with a long investment horizon (sells before maturity)** - concerned with reinvestment risk and market price risk is insignificant to affect these returns.
- **Investor with a short investment horizon (sells before maturity)** should be more concerned with market price risk as reinvestment risk affects her returns to a lesser extent, as market price has an inverse relationship with interest rates.

![[Screenshot 2023-05-23 at 18.59.18.png]]

## Duration
In general, the **duration** of a bond **is a measure of its interest rate risk. (i.e. bond sensitivity to changes in interest rates)**. It is required to calculate the duration through 
yield to maturity (YTM). **YTM** is calculated through the benchmark rate (real return +  inflation premium) + spread (tax premium + liquidity premium + credit risk premium).

e.g. If the duration of a bond is high, we would expect a high fluctuation in the bonds price when its yield changes.
e.g2. If the duration is low, the price fluctuation due to change in interest rate will be low as well.

There are 3 methods to calculate **durations**:
- Macaulay duration
- Modified duration
- Money duration

### Macaulay duration
**Macaulay duration** is a measure of a bond sensitivity to changes in interest rates by using the weighted average of the number of years until each bond's promised cash flows is to be paid.
When a bond investors investment horizon matches the bonds' **Macaulay duration**, a parallel shift in the yield curve prior to the first coupon payment will minimally affect the investors net return.

In general, the **duration** of a bond **is a measure of its interest rate risk.** More specifically, it measures the sensitivity of the bonds full price to a change in its yield. 
e.g. If the duration of a bond is high, we would expect a high fluctuation in the bonds price when its yield changes.
e.g2. If the duration is low, the price fluctuation due to change in interest rate will be low as well.

![[Screenshot 2023-05-23 at 19.04.36.png]]
![[Screenshot 2023-05-23 at 19.04.44.png]]

The **Macaulay duration** is calculated as the **weighted average** of the **number of years** until each of the **bonds promised cash flows is to be paid**. The weights are the present values of each cash flow as a percentage of the bonds full value.

The **Macaulay duration weights** equation is as follows:
$$\mathrm{Macaulay\,duration\,weights=\frac{PV\,of\,each\,CF}{Full\,value}}$$

There are 4 steps in calculating the Macaulay duration:
1. Identify all the cash flow (coupon, final: coupon + final principle payment)
2. Discount to PV using the bond's yield (depending whether semi annual, if so divide YTM by 2; if quarterly, divide YTM by 4)
3. Calculate the weights (by dividing the PV by the last traded price)
4. Sum up the weights with the number of years (i.e. weights $\times$ number of payment period then convert into years) as Macaulay Duration unit is in years.

One shortcoming of this measure is that Macaulay duration does not tell you how much the market price will drop when interest rates increase, which is a bigger concern to bond investors.

![[Screenshot 2023-06-21 at 18.31.05.png]]
![[Screenshot 2023-05-23 at 19.11.35.png]]
![[Screenshot 2023-05-23 at 19.14.44.png]]

**Duration gap** is when the bonds yield to maturity (YTM) changes the difference between a bonds **Macaulay duration and the investors investment horizon**.

A **positive duration gap** exposes the **investor to market price risk from increasing interest rates, the rate of return will be lower** (i.e. market price risk > reinvestment risk). 

A **negative duration gap** exposes the **investor to reinvestment risk from decreasing interest rates, the rate of return will be higher as the coupons will have more time to earn higher interest** (i.e. market price risk < reinvestment risk).

![[Screenshot 2023-05-23 at 19.18.54.png]]

### Modified duration 
The **modified duration** provides an approximate **percentage change** in a bond's price for a **1% change** in yield to maturity (YTM). The **modified duration** uses YTM, and it is applicable to measure the change of bond price in option-free bond (i.e. straight bonds), as the YTM and cashflows are well defined.

The **modified duration** equation is as follows:
$$\mathrm{Modified\,duration=\frac{Macaulay\,duration}{1+YTM}}$$
For **semi-annual modified duration** is as follows:
$$\mathrm{Modified\,duration_{semi}=\frac{Macaulay\,duration}{1+YTM/2}}$$
and the **semi-annual to annual modified duration**
$$\mathrm{Modified\,duration_{annual}=\frac{Modified\,duration_{semi}}{2}}$$
The **modified duration** can approximate the relationship between the bond price and the change in yield as follows. The approximate % change in bond price is the negative of the modified duration, multiplied by the change in yield to maturity (YTM).

$$\mathrm{Approx. \% \,price\,change=-Modified\,duration\times \Delta YTM}$$
where the modified duration has to be converted into annual unit.

At this instance, if the bonds yield (YTM) instantaneously increases by 1%, the bond's price would drop by approximately the % of modified duration and vice versa.

![[Screenshot 2023-05-23 at 19.31.09.png]]
![[Screenshot 2023-06-21 at 15.35.53.png]]
![[Screenshot 2023-05-29 at 19.30.20.png]]

### Money duration
**Money duration**, also known as dollar duration, provides an approximate **absolute change** in a bond's price for a **1% change (i.e. 100bp)** in yield to maturity (YTM).

There are several methods of expression of **money duration**:
- **Based on full price of bond position**
- **Per 100 of par value**
- **Price value per basis point (PVBP)** 

#### Based on full price of bond position
The equation of money duration **based on full price of bond position** is as follows:
$$\mathrm{Money\,duration=Modified\,duration\times Full\,price\,bond\,position}$$
where the full price bond position is the holdings of the investor; money duration: if YTM increase by 1%, then the bond position change by _money duration_.

#### Per 100 of par value
The equation of money duration **Per 100 of par value** is as follows:
$$\mathrm{Money\,duration=Modified\,duration\times Full\,price\,of\,bond\,per\,100\,of\,par}$$
where the full price of bond per 100 of par value ($\mathrm{\frac{PV}{par\,value}}$ $\times$ 100); and if YTM increase by 1%, every $100 par change by _money duration_ $\times$ 1%. Calculate the change in bond position remembering that current par change is measured every $100. 

![[Screenshot 2023-06-21 at 15.51.43.png]]

#### Price value per basis point (PVBP)
**Money duration of PVBP**, also known as **dollar duration**, provides an approximate **absolute change** in a bond's price for a **1bp change** in yield to maturity (YTM).
The equation of money duration **Price value per basis point (PVBP)** is as follows:
$$\mathrm{PVBP=\frac{(V_{-}-V_{+})}{2}}$$
where 1 bp is 0.01%; and the money duration should be calculated per 100 par and convert all the values to per 100 par. Money duration: if YTM increase by 1% (100bp), then the bond position change by _money duration_ (PVBP $\times$ 100).

![[Screenshot 2023-06-21 at 15.52.02.png]]
![[Screenshot 2023-06-21 at 16.10.01.png]]

## Approximate modified duration and convexity adjustment
**Modified duration (ModDur)** can be used to calculate the **approximate change in price** of a bond **given a change in YTM of the bond**. However, in reality, the actual price-YTM relationship follows a convex curve, and to find that can use the **approximate modified duration**.

![[Screenshot 2023-06-21 at 16.12.29.png]]

### Approximate modified duration
The **approximate modified duration** is very similar as the **modified duration**, when the YTM should be very small and the precision in calculation should be high.
The equation for approximate **modified duration (ApproxModDur)** is as follows:
$$\mathrm{ApproxModDur=\frac{(V_{-}-V_{+})}{2\times V_0 \times \Delta YTM}}$$

where the $V_0$ is the present value of the bond by DCF; $V_{-}$ is price after the small change of YTM in negative direction, and $V_{+}$ is the price after small change of YTM in positive direction, and the change in YTM could be 1bp, which equals to 0.0001 (0.01%).

![[Screenshot 2023-06-21 at 16.14.40.png]]
![[Screenshot 2023-06-21 at 16.23.26.png]]

The **modified duration** is using a **straight line for approximation** for **small change of YTM and its influence towards the price change**. However, if there is a **huge change in YTM**, the **modified duration method will severely underestimate the magnitude of change**. 

> For large changes in yield, duration **underestimates** the increase in price when yield decreases and overestimates the decrease in price when yield increases. This is because duration is a linear estimate that does not account for the convexity (curvature) in the price/yield relationship.

![[Screenshot 2023-06-21 at 16.24.57.png]]

### Convexity adjustment
In the scenario where there is a huge change in YTM, there is a need for accounting the **2nd order effects**. which is the **convexity adjustment** in order for better estimation of the change in bond price. **Convexity** is the measure of the curvature of the price-yield relation. 

The **1st order effect** of YTM and change in bond price is mentioned before:
$$\mathrm{Approx. \% \,price\,change=-Modified\,duration\times \Delta YTM}$$

The **2nd order effect** of YTM and change in bond price is as follows :
$$\mathrm{Approx. \% \,price\,change=\frac{1}{2}Convexity\times (\Delta YTM)^2}$$
which accounts for the convexity of the curve.

Therefore, the full equation of **approximate modified duration with convexity adjustment** is as follows:
$$\mathrm{\% \Delta\,price=-Modified\,duration\times \Delta YTM+\frac{1}{2}Convexity\times (\Delta YTM)^2}$$

The **approximate convexity** can be calculated by using this formula:
$$\mathrm{Approximate\,convexity=\frac{(V_{-}+V_{+}-2V_0)}{V_0 \times \Delta YTM^2}}$$
where the $V_0$ is the present value of the bond by DCF; $V_{-}$ is price after the small change of YTM in negative direction, and $V_{+}$ is the price after small change of YTM in positive direction, and the change in YTM could be 1bp, which equals to 0.0001 (0.01%).

![[Screenshot 2023-06-21 at 16.40.05.png]]

where the YTM change is huge, the approximate modified duration and approximate convexity could help to calculate the price change of a bond. It should then be using per 100 par in the money duration to get the actual absolute price change per YTM change.

![[Screenshot 2023-06-21 at 16.45.50.png]]
![[Screenshot 2023-06-21 at 16.56.11.png]]

### Credit and liquidity risk
The **duration** of a bond is a **measure of its interest rate risk**. (i.e. bond sensitivity to changes in interest rates). It is required to calculate the duration through 
**yield to maturity (YTM)**. Generally, **longer duration indicates higher price sensitivity**, while **shorter duration suggests lower price sensitivity**.

**"Duration matching"** or "duration alignment" is the **duration of a bond is closely related to the time it takes to recover the bond's price through its cash flows**. For investors with a **shorter investment horizon**, such as those planning to hold the bond until maturity or for a relatively brief period, bonds with **shorter duration** may be more suitable 
**(i.e. shorter investment horizon ⇒ shorter duration)**.

On the other hand, investors with a longer investment horizon, such as those seeking to hold bonds for an extended period, may consider bonds with longer duration. Longer-duration bonds tend to offer higher yields to compensate for the increased risk associated with their higher price sensitivity. While they may exhibit greater price volatility in response to interest rate changes, investors with a longer time horizon have more time to potentially benefit from the bond's income payments and to wait for the bond's price to recover if it temporarily declines **(i.e. longer investment horizon ⇒ longer duration)**.

**YTM** is calculated through:
- the benchmark rate (**real return** +  **inflation premium**) - e.g. treasury/risk-free rate
- spread (**tax premium** + **liquidity premium** + **credit risk premium**) - credit quality of the bond

Since all of the components are additive, a given increase/decrease in any of these components will increase/decrease the bond's YTM by the same amount, that is the **modified duration** of the bond, which means we can estimate each component using the same formula.

Therefore, **any of these components** can be substituted into the approximate % price change equation:
- spread
- benchmark curve
- credit risk
- liquidity premium
- tax premium
- inflation premium
- real return

Therefore, the full equation of **approximate modified duration with convexity adjustment** is as follows:
$$\mathrm{\% \Delta\,price=-Modified\,duration\times \Delta YTM+\frac{1}{2}Convexity\times (\Delta YTM)^2}$$
where the YTM can be substituted with any of the components (e.g. spread, benchmark curve, credit risk, liquidity premium, tax premium, inflation premium, real return). 
![[Screenshot 2023-06-21 at 17.00.19.png]]
![[Screenshot 2023-06-21 at 17.02.05.png]]
![[Screenshot 2023-06-21 at 17.05.31.png]]

## Effective duration and key rate duration
### Effective duration
**Effective duration** is the **approximate percentage change in a bond's price** for **1% change** in the **benchmark yield**.

The **effective duration equation** is as follows:
$$\mathrm{Effective\,duration=\frac{(V_{-}-V_{+})}{2\times V_0 \times \Delta curve}}$$
where the curve is the benchmark yield curve, and assumes parallel shift in benchmark yield curve. 

![[Screenshot 2023-06-21 at 17.28.11.png]]

#### Application of effective duration
The application of **effective duration** is for:
- bonds with embedded options 
- mortgage-backed securities

Bonds with embedded options (e.g. callable bonds). With the fall in market interest rate, the company is likely to call back the bond and refinance with lower interest rate, and the YTM is not well defined.

Another fixed income security, mortgage-backed securities with prepayment option, as the borrowers are allowed to prepay the principal, the prepayments increases as the interest rate falls significantly because homeowners can refinance at a lower rate.

The effective duration of a putable bond is less than the effective duration of an otherwise identical option-free bond at relatively high yields. Assuming no default, the price of a putable bond will not fall below its put price. The put price acts as a floor. Therefore, as yields increase into the range in which the embedded put option becomes valuable, the price of a putable bond decreases less than that of an otherwise identical option-free bond.

![[Screenshot 2023-06-21 at 17.15.51.png]]
![[Screenshot 2023-06-21 at 17.21.53.png]]

#### Differences between modified duration and effective duration
Unlike the **approximate modified duration**, a small YTM can have a great change in bond price, therefore **it requires accurate calculation (i.e. 1bp)**. However, the market interest rate needs to change by a **larger amounts to affect decisions** to call a bond or refinance a mortgage, therefore **larger change in yield, more accurate** the **effective duration**.

![[Screenshot 2023-06-21 at 17.24.35.png]]

#### Effective duration convexity approximation
The effective duration convexity approximation is similar to the approximate modified duration convexity.
The **effective duration convexity approximation** equation is as follows:
$$\mathrm{Effective\,convexity=\frac{(V_{-}+V_{+}-2V_0)}{V_0 \times \Delta {curve}^2}}$$
where the curve is a parallel shift in benchmark yield curve.

Note, that the price-yield relationship of bond with options (i.e. callable/putable bond)is not as straight forward for option-free bond.

![[Screenshot 2023-06-21 at 17.25.52.png]]

#### Price-yield relationship for callable bond
If this bond has an **embedded call option** that allows the issuer to call back the bond at a certain price, this effectively becomes a cap to the price of the bond as no investor will buy the bond above its call price.

We also know that the bond is more **likely to be called when the benchmark yield is low**, as the issuer can recall this loan at lower interest rates.

As such, the price to yield curve will have negative convexity beyond a certain yield, with a price capped at the call price. The difference between the option for a bond price and the equivalent callable bond price is the value of the call option.

Since the issuer of **a callable bond has an incentive to call the bond when interest rates are very low in order to get cheaper financing**, this puts an **upper limit on the bond price for low interest rates and thus introduces negative convexity between yields and prices**.

![[Screenshot 2023-06-21 at 17.26.58.png]]

#### Price-yield relationship for putable bond
For a putable bond, we know that the put option is of value to the bond holders, so the price of a putable bond has to be higher than the equivalent option for a bond (i.e. price of putable bond > option-free bond).

The value of the **put option is higher when the benchmark yield is high**, thus accounting for the shape of the curve as compared to its option for a counterpart. When interest rates are high, the option to sell back the bond to the issuer is more valuable as it allows the bond holders to liquidate and reinvest the money into higher yielding assets.

![[Screenshot 2023-06-21 at 17.26.49.png]]

### Key rate duration
The **effective duration** **assumes** **parallel shift** in the **benchmark yield curve**, however, in reality, this is generally not the case. **Key rate duration** estimates the "shaping risk" of a bond and yield curve, it is the sensitivity of the value of a bond to changes in the spot rate for a specific maturity, holding other spot rates constant.

The US treasury yield curve can be one of those 3 curves:
- steepen yield curve
- flatten yield curve
- inversion yield curve
![[Screenshot 2023-06-21 at 17.34.23.png]]
![[Screenshot 2023-06-21 at 17.34.40.png]]

## Empirical duration
### Analytical duration vs. empirical duration
The **analytical duration** measures that we have learned are based on **mathematical analysis**, like the **expected future cash flows and maturity of the fixed income instruments**. Another approach, **empirical duration**, to measure duration is to use the **historical relationship between the benchmark yield and bond prices**.

### Reason to use empirical duration

#### Estimate the sensitivity of price of corporate bond
**Empirical duration** is better suited for corporate bond price sensitivity to interest rate analysis. Corporate bonds has a credit spread above the benchmark yield.

If we use an analytical duration to estimate the change in price of a corporate bond based on the expected change in benchmark yield, the implicit assumption is that the credit spread remains constant. However, this may not be a valid assumption.

In a typical flight to quality scenario where investors sell risky assets in a market turmoil to purchase government bonds, the benchmark yield decreases while the credit spread increases. The net change in yield of the bond is not equal to the change in benchmark yield. Using the analytical duration to estimate the increase in price of a corporate bond is inappropriate as the price may increase less or even decrease depending on its credit quality.

In contrast, empirical duration, which is based on historical relationships, has already factored in the relationship between credit spread and benchmark bond yields. As such, empirical duration may produce more appropriate estimates of the changes in corporate bond price for a corporate bond portfolio, its empirical duration is likely to be lower than its analytical duration.

![[Screenshot 2023-05-29 at 18.01.57.png]]

#### Government bond
In contrast, a **government bonds yield** is fully the **benchmark yield**. 
The change in interest rate is the change in benchmark yield. 
As such, the analytical duration of a portfolio of government bonds is likely to be very close to its empirical duration. Either of them provides a good estimate of the change in price due to a change in benchmark yield.

![[Screenshot 2023-05-29 at 19.01.38.png]]

## Duration of a bond portfolio
The **duration** mentioned above stated several ways to calculate percentage change in **a single bond price** when the YTM/benchmark yield curve change:
- **Macaulay duration** - 
- **Modified duration** - the %$\Delta$ in bond price when YTM change by 1% or 1 bp
- **Money duration** - the absolute $\Delta$ in bond price when YTM change by 1% or 1 bp
- **Effective duration** - the %$\Delta$ in bond price when the benchmark yield curve changes, assuming the change is a parallel shift

There are 2 approaches to calculate the duration of a bond portfolio:
- aggregate all the cashflow
- **weighted average method** - more commonly used

### Aggregate all the cash flow in bond portfolio
To calculate aggregated cash flow in bond portfolio:
1. Find the cash flow yield using IRR
2. Use the cash flow yield to find the PV of the cash
3. Use the PV and the initial investment value to find the respective weight of the cash flow
4. Use the weight of the cash flow and multiple the years, to get the **Macaulay duration**
5. Divide the Macaulay duration by the cash flow yield to get the **modified duration**

To aggregate all the cash flow yield, one must find the internal rate of return (IRR) for the aggregated cash flow, where using TVM calculator (CF and IRR):
- $CF_0$: initial investment (cash outflow)
- $C01$: cash inflow at period 1
- $F01$: cash inflow frequency of C01
The cash flow yield will be used the **Macaulay duration** of the portfolio.
![[Screenshot 2023-06-21 at 18.00.40.png]]


![[Screenshot 2023-06-21 at 18.00.57.png]]

Limitations of aggregate all the cash flow in bond portfolio:
- cannot apply if portfolio contains callable, putable or floaters
- interest rate risk usually expressed as change in benchmark yield, not cash flow yield

### Weighted average of bond in bond portfolio
1. Calculate the total market value of the bond
2. Use the current market value of the bond to find out respective weights of the bond in portfolio
3. Calculate the Macaulay duration of respective individual bond (discount the PV)
4. Calculate the Modified duration of respective individual bond ($\mathrm{\frac{Macaulay\,duration}{1+ YTM}}$)
5. Use the weights to multiple the Macaulay duration of individual bond to get the Macaulay duration of portfolio and Modified duration for Modified duration of portfolio

![[Screenshot 2023-06-21 at 18.26.58.png]]
![[Screenshot 2023-06-21 at 18.01.49.png]]

Advantage:
- Callable, putable or floaters can be included using their effective durations

Limitations: 
- Only an approximation of theoretically correct value, more accurate if YTM between bonds are similar
- assumes parallel shift in yield curve

## Factors that influence interest rate risks
**Duration** is a measure of the interest rate risk of a bond. 
There are 3 main properties that can determine the **interest rate risk** of a bond are:
- **Time to maturity** - direct relation (i.e. increase in time to maturity, increases interest rate risk)
- **Coupon Rate** - inverse relation (i.e. increase in coupon rate, decrease interest rate risk and lower price volatility)
- **Yield-to-Maturity** - inverse relation (i.e. increase in YTM, decrease interest rate risk)
 ![[Screenshot 2023-06-21 at 18.45.08.png]]
 
A simple way to look at this is the increase in the coupon rate means more of a bond's value will be from payments received sooner. The value of the bond will be less sensitive to changes in the yield of the bond. The same pattern holds for the yield to maturity.

The interest rate risk can modify the:
- **sensitivity to change of yield** (e.g. time to maturity, coupon rate, yield-to-maturity)
- **volatility of the bond's yield** - term structure of yield volatility (the relationship between the volatility of a bond yield to the times to maturity)

### Time to maturity on interest rate risk
There are different interest rate risk depending on the bond type:
- bullet bond (balloon payment)
- perpetual bond - does not mature and no principal to redeem, receive fixed coupon forever

If it's a bullet bond with balloon payment, the final payment is of the largest weight.
A **short time to maturity** will have a lower **Macaulay duration**. Conversely, if the time to maturity is long, the largest weight will be on the longest time, so the Macaulay duration is higher.

The general relationship for a **fixed coupon bond** is the **longer the time to maturity**, the **higher the duration**. However, **this relationship is not linear**. The longer the time to maturity, the higher the discount factor for the balloon payment. As such, the relationship is more like a curve with an upper limit and this relationship only applies to bonds purchased at par or at a premium.

However, if the bond is purchased as discount, then the relationship follows this interesting curve. The duration first increases with longer maturity and then decreases over a range of relatively long maturities until it approaches the duration of a perpetuity.

### Macaulay duration of fixed coupon bond purchased at par, premium and discount and perpetual bond 
![[Screenshot 2023-05-29 at 17.53.15.png]]

### Macaulay duration of zero coupon bond
The **Macaulay duration** of a **zero coupon bond** is simply the **number of years to maturity**. There is only one cash flow, which is on the maturity date and the weight of this cash flow is 1.0, therefore the relationship should follow a straight line that has a slope of 1.0.
![[Screenshot 2023-05-29 at 17.53.44.png]]

### Coupon rate on interest rate risk
Holding all else equal, a bond that has a **higher coupon rate** will have a lower Macaulay duration and therefore **lower interest rate risk** (i.e. ↑ coupon rate ⇒ ↓ interest rate risk).

Higher coupon rate shifts weight towards earlier cash flows, lower duration, this increase in the coupon rate means more of a bond's value will be from payments received sooner. The value of the bond will be less sensitive to changes in the yield of the bond.

![[Screenshot 2023-05-29 at 17.55.17.png]]

### Yield-to-Maturity on interest rate risk
All else equal a higher yield to maturity (YTM), decreases the discount factor of cash flows to be paid in the near term and increases the discount factor of the cash flows in the far term.

Yield-to-maturity (YTM) is calculated by the benchmark rate and spread, which the benchmark rate includes the real return, expected inflation, and the spread includes credit risk premium, tax premium and liquidity premium.
Higher YTM rate shifts weight towards earlier cash flow, lower Macaulay duration.
![[Screenshot 2023-05-29 at 17.55.36.png]]

### Term structure of yield volatility
**The term structure of yield volatility** refers to the relationship between yield volatility and time to maturity.

![[Screenshot 2023-06-21 at 18.46.32.png]]

If the term structure of yield volatility slopes upward, long-term interest rates are more variable than short-term interest rates.

If bonds are identical except for maturity and coupon, the one with the longest maturity and lowest coupon will have the greatest duration. The later the cash flows are received, the greater the duration.

---
## Questions before starting this section:
- [ ]

## Codes to test understanding of objectives