# 1a - Discounted Cash Flow (removed from 2020)
202210101452
Status: #📥 
Tags: [[CFA Level I]]

## Objectives:
- [ ] calculate and interpret the net present value (NPV) and the internal rate of return (IRR) of an investment.
- [ ] contrast the NPV rule to the IRR rule, and identify problems associated with the IRR rule.
- [x] calculate and interpret a holding period return (total return).
- [x] calculate and compare the money-weighted and time-weighted rates of return of a portfolio and evaluate the performance of portfolios based on these measures
- [ ] calculate and interpret the bank discount yield, holding period yield, effective annual yield, and money market yield for US Treasury bills and other money market instruments.
- [ ] convert among holding period yields, money market yields, effective annual yields, and bond equivalent yields.

### Review
- [ ] TWRR

---

## NPV and IRR

**Net Present Value (NPV)**: The value of all future cash flows (positive and negative) over the entire life of an investment discounted to the present.

**Internal Rate of Return (IRR):** The expected compound annual rate of return that will be earned on a project or investment.
Whether such investments are worthwhile depends on the approach that the company uses to evaluate them. A company may value the projects based on: NPV or/and IRR.
![[Screenshot 2023-01-30 at 23.13.26.png]]


## Calculate NPV and IRR
- If the investment requires periodic investment before an unequal amount of return over a period of time, the calculation of interest rate is **not** as straight forward in calculating just by calculating the difference between the sum of future cash flows minus the sum of present cash flows (formula for NPV), as it does not provide the information of 
	Net present value (NPV): $$NPV = \sum{FV}-\sum{PV}$$
- To calculate the interest rate, one has to discount all the future values to present value and sum them up to calculate the NPV.
- Lowering return expectation
- Cost of capital, 5% to today's money of NPV
- Internal rate of return is the discount rate that makes the NPV=0, actual annualised return to the investor
- IRR is valid only if these are reinvested at the same rate
Learn the BAII plus calculator to key in CF to calculate NPV and IRR

## Decision rules
- Calculation of the NPV and IRR allows the investor to compare between different products with unequal cash flow investment and payments
- After the calculation of NPV and IRR, decide whether an investor should go onto invest in the projects, first of all depending on whether the projects are not mutually exclusive or mutually exclusive.
- If the projects are not mutually exclusive, there are two rules to determine whether the investor should invest in the project: NPV and IRR rule.
	- **NPV rule:** Choose projects with positive NPV
	- **IRR rule:** Choose projects with IRR > required return (i.e. For a project to be considered, its IRR has to be higher than the cost of borrowing of the investor.)
- If the projects are mutually exclusive, then the NPV rule is used:
	- **NPV rule**: Choose the project with higher NPV, because it has the potential to increase wealth by greater amount than the other project

Do not make decision of NPV is not known.
Information is insufficient to make an informed decision because:  
(a) The cost of borrowing of Zber Corp is not known. We should only accept projects where the IRR > cost of borrowing.  
(b) If projects are mutually exclusive, should make decision based on NPV rule instead.


## Portfolio return measurements
Since the portfolio have constant inflows (i.e. subscriptions, dividends/coupons) and outflows (i.e. redemptions, dividend payouts, fees)
It is measured and evaluated through:
- **Market weighted rate of return (MWRR)** - same as IRR
- **Holding period return (HPR)** - use beginning, cashflow and end value to calculate
- **Time weighted rate of return (TWRR)** - geometric mean

## Money weighted rate of return (MWRR)
**Money weighted rate of return (MWRR)** is the same as internal rate of return (IRR)
$$\mathrm{Money\,Weighted\,Rate\,of\,Return = Internal\,Rate\,of\,Return}$$
which is clearly not the best way in measuring the performance, it is affected by the amount of cash inflow and outflow
**Note**: The final cash flow (CF) should add the inflow and the residual amount in the account

![[Screenshot 2022-10-10 at 16.15.07.png]]

## Holding period return (HPR)
**Holding period return (HPR)** can be used to calculate from the beginning and ending value with the cash flow (i.e. coupon and dividend)

**The holding period of return (HPR)** formula is as follow:
$$\mathrm{HPR = \frac{P_1+CF}{P_0}-1}$$
where $P_1$: Ending value; $P_0$: Beginning value; CF: cash flow received

When there's unequal cash flow in and out of the account the HPR should be calculated for each time period and the summation of all periods to get the final HPR.

![[Screenshot 2022-10-10 at 16.15.28.png]]

## Time weighted rate of return (TWRR)
**Time weighted rate of return (TWRR)** is the most widely used measurement to calculate the portfolio performance across time. TWRR is calculated by the geometric mean of portfolio (i.e. TWRR = geometric mean of portfolio).

The formula of **Time weighted rate of return (TWRR)** is as follow:
$$TWRR=\sqrt[n]{(1+R_1) \times (1+R_2) \times ... \times (1+R_n)}$$
where $R_{1\,to\,n}$: calculated through the holding period return (HPR) which previously discussed


## Practice question:
![[Screenshot 2022-10-10 at 16.35.36.png]]

![[Screenshot 2022-10-10 at 16.36.13.png]]

Robert opened an investment account and made an initial investment of $100,000. The account earned a return of 15% in the first year. At the beginning of the second year, Robert placed another $500,000 into the account. The account earned a return of 10% in the second year. The money weighted rate of return of the account is most likely:  lower than the time-weighted rate of return.

Weight in the second year is **higher** than the first.  
Return in the second year is **lower** than the first.  
There is a greater weight on this lower return. Hence the MWRR is lower than the TWRR.


## Summary of MWRR, HPR, TWRR
**Remember**: always clear the memory first before keying in the CF (2nd+CLR WORK).
HPR on per share basis
![[Screenshot 2022-10-10 at 16.36.42.png]]
![[Screenshot 2023-07-05 at 21.35.32.png]]
## Market weighted rate of return?

## Money market yield
**Money market** is the short-term debt instruments which typically have 1 year of maturity or less. U.S. T-bills are quoted differently and quoted on a discount basis. **Face value of the bill** is the price of maturity. **Note:** Yield and rate can be used interchangeably.

### Method of expressing yields
There are 5 methods of expressing yields:
- **Bank discount yield** - assumed interest type is zero coupon and 360 days per year
- **Holding period yield** - does not have to be annualised, for annualisation look below for further information
- **Money market yield** - 
- **Effective annual yield** - assumed compound interest
- **Bond equivalent yield** - assumed compound interest, and which is 2 $\times$ effective semi-annual yield
 
- US T-bills are quoted in a discount rate 


![[Screenshot 2023-06-23 at 15.01.40.png]]

#### Bank discount yield
There are 3 steps to follow to find the bank discount yield:
1. Find the discount factor
2. Find the daily rate
3. Annualise it

The **discount factor** equation is as follows:
$$\mathrm{Discount\,factor=\frac{Discount}{Face\,value}}$$
and discount factor is cash gained/face value.

To find the **daily rate**, use this equation:
$$\mathrm{\frac{360}{t}}$$
where t: number of days to maturity, and 360 days is a bank convention for 1 year.

Therefore, the full equation for **bank discount yield** is as follows:
$$\mathrm{Discount\,factor=\frac{Discount}{Face\,value}\times\frac{360}{t}}$$
### Holding period yield
The **holding period yield (HPY)** can be used to calculate from the beginning and ending value with the cash flow (i.e. coupon and dividend).

The **holding period yield (HPY)** formula is as follow:
$$\mathrm{HPY = \frac{P_1+CF}{P_0}-1}$$
where $P_1$: Ending value; $P_0$: Beginning value; CF: cash flow received; and holding period yield does not have to be annualised figure.

The **holding period yield (HPY)** can then be annualised through simple or compounding method. 

### Money market yield
The **money market yield** is often used to compare T-bills with money market instruments that have simple interest over a **360** day year.

In assuming **simple interest**, the value would be the **money market yield**, which multiplies the same factor of daily rate:
$$\mathrm{Money\,market\,yield=HPY\times\frac{360}{t}}$$
where HPY: holding period yield.

### Effective annual yield
The other way is the **effective annual yield**, which is assumed **compound interest** during  the **holding period yield** by **365 days**.

The **effective annual yield** equation is as follows:
$$\mathrm{Effective\,annual\,yield=(1+HPY)^{365/t}-1}$$
where HPY: Holding period yield; and the effective annual yield calculation method is similar to the effective annual rate.

### Bond equivalent yield
**Bond equivalent yield** is closely related to effective annual yield. Bond equivalent yield is essentially the same as effective annual yield.

The **bond equivalent yield** equation is as follows:
$$\mathrm{Effective\,annual\,yield=(1+HPY)^{365/t}-1}$$
where HPY: holding period yield.

The **effective semi-annual yield** equation is the EAY converted to semi-annual yield:
$$\mathrm{Effective\,semi\,annual\,yield=(1+EAY)^{1/2}-1}$$
where EAY: effective annual yield.

The **bond equivalent yield** equation is:
$$\mathrm{Bond\,equivalent\,yield=2\times Effective\,semi\,annual\,yield}$$

The difference is that instead of compounding to a full year, we compound to half a year to obtain an effective semi-annual yield. To get the full year yield, simply multiply the semi-annual yield by two. This convention is due to the fact that most bonds are quoted as 2 $\times$ the semi-annual rate.

### Summary of different methods of expressing yields
![[Screenshot 2023-06-23 at 15.01.40.png]]

Sort these (highest at top) according to their calculated yield on the same T-bill with positive yield.
(1) Effective Annual Yield – highest because of full year compounding  
(2) Bond Equivalent Yield – next highest because of half year compounding  
(3) Money Market Yield – second lowest because it is non compounding but higher than BDY because denominator is invested amount  
(4) Bank Discount Yield – lowest because it is non compounding and denominator is face value (higher the invested amount)

### Convert between different yields
Simply remember that the inverse is to flip over the time adjustment factors.

For bond equivalent yield and effective annual yield: get back the semi-annual yield by dividing the bond equivalent yield by two, and then square the factor to obtain the full year yield.
![[Screenshot 2023-06-23 at 16.47.18.png]]
![[Screenshot 2023-06-23 at 16.54.18.png]]


---
## Questions before starting this section:
- [ ] what are the difference in NPV vs IRR?



## Codes to test understanding of objectives