# 1 - Time Value of Money
202209072224
Status: #📥 
Tags: [[CFA Level I]], 

## Objectives:
- [x] interpret interest rates as required rates of return, discount rates, or opportunity costs
- [x] explain an interest rate as the sum of a real risk-free rate and premiums that compensate investors for bearing distinct types of risk.
- [ ] calculate and interpret the effective annual rate, given the stated annual interest rate and the frequency of compounding.
- [ ] calculate the solution for time value of money problems with different frequencies of compounding.
- [ ] calculate and interpret the future value (FV) and present value (PV) of a single sum of money, an ordinary annuity, an annuity due, a perpetuity (PV only), and a series of unequal cash flows.
- [ ] demonstrate the use of a time line in modeling and solving time value of money problems.

## Review:
- [x] Interest rate (including nominal, real, T-bills)
- [ ] What is risk?
- [x] Sharpe ratio
- [ ] Uneven cash flows (CF)
- [ ] Calculator usage for TVM questions
- [ ] Continuous compounding 
- [ ] Perpetuity
- [ ] Annuity due and ordinary annuity

## Codes to test understanding of objectives
1. Calculate interest rate (nominal)
	$$IR = RFR + RP + EIR$$
where IR: interest rate; RFP: Risk-free premium; RP: Risk premium; EIR: Expected interest rate

2. Generate a python script/ notebook for calculating future value with principal amount
	$$FV = PV(1+r)^N$$
where FV: Future value; PV: Present value; r: interest rate; N: Number of period for compounding

3. Answer the question of constant new injection of money (monthly, annually, bi-annually) vs lump-sum in index fund and their performance 

4. Calculate for the amount needed to invest annually for retirement ✅
5. Unequal cash flow of investment 

https://cs-people.bu.edu/azs/fe459/assignments/a1.html


## Definitions
**Interest rate** - A person/institute borrowed a certain amount of money from lender and the borrower has to return back a certain percentage of the borrowed money after a period of time along with the principal. 

> "In other terms, if you’re a borrower, the interest rate is the amount you are charged for borrowing money, shown as a percentage of the total amount of the loan. If you’re an investor/lender, the interest rate (*yield*) tells you how much money will be paid into your account, as a percentage of your savings." - Bank of England

**_Yield_** is the **percentage of earnings a person receives for lending money**. An **interest rate** represents money **borrowed**; **yield** represents **money lent**. Technically, they are two terms but they can use interchangeably in calculation but concept wise they are different.

- Also known as **discount rate**, when discounted the future value in order to understand the present/principal value needed to be invested
- It can be also viewed as **opportunity cost** and **required rate of return**
- Required rate of return - the sum of all considered factors for interest rate, including risk premium (default risk, liquidity risk, maturity risk) and nominal risk-free rate (real risk-free rate and inflation premium)

#### Opportunity cost

$$\mathrm{Opportunity\,cost = \frac{Interest\,foregone}{Principal\,value}}$$

**Real risk-free rate** - Rate that are risk-free **not** adjusted for inflation
**Nominal risk-free rate**  - Rate that are risk-free and adjusted for inflation
**Treasury bills (T-bills)** - IOU notes that are distributed by the FED and are normally set as the nominal risk-free rates because they contain an inflation premium
**Default risk** - The risk of the borrower not returning back the money

The equation is as follows:
**Nominal risk-free rate** = real risk-free interest rate + expected inflation rate (inflation premium)

Required interest rate on a security (required rate of return) = nominal risk-free interest rate (US T-bills) + default risk premium + expectation inflation rate + liquidity premium + maturity risk premium

## Risk-free interest rate
**Risk-free interest rate** is minimum expected return from any investment

### How to calculate?
- **Real risk-free rate**: 3 months T-bills is often used as the benchmark in the US, however, depending on each jurisdiction, they have their own risk-free rate
- **Inflation premium**: Expected inflation in the period of time where the debtor is borrowing the money 

## Types of risks
**Risk** is defined in financial terms as the chance that an outcome or investment's actual gains will differ from an expected outcome or [return](https://www.investopedia.com/terms/r/roys-safety-first-criterion.asp). Risk includes the possibility of losing some or all of an original investment. 
- **Default risk** ⇒ The risk that the borrower will not return the promised payment in a timely manner, often needs to consider the debt-taker’s financial’s and credit rating; to compensate for the possibility that the borrower is unable to make promised payment
- **Liquidity risk** ⇒ The risk of receiving less than fair value of an investment if sold for cash quickly, whether there’s a market to sell this debt agreement 
- **Maturity risk** ⇒ Longer-term bonds have more maturity risk than shorter-term bonds because of the volatility in risk/price, also forfeiting the opportunity cost of future increased in risk-free rate; to compensate the possibility for a change in market rate

## Future value of a single cash flow
**Future value** is the amount to which investment grows after one or more compounding periods.
- Interest rate are normally reported as annual rate, be mindful of the interest per period depending on the compounding period time (which is known as the periodic rate) 
- Slightly higher of future value if the compounding times increase, as the interest rate increases 5% annual rate ⇒ 2.5% bi-annual rate (bi-annual PV > annual PV)
- **Note:** The EAR increases as the compounding frequency increases

### Future value of multiple cash flows of same rate
Calculating **future value with principal amount**, the equation is as follow:
$$FV = PV(1+r)^N$$
where FV: Future value; PV: Present value; r: interest rate; N: Number of period for compounding

### Effective annual rate (EAR)
**Effective annual rate (EAR)** is how much interest is effectively given out in a year, allow us to compare interest rate with different compounding period, and here is the equation:

$$EAR = (1+r)^N -1$$
where EAR: Effective annual rate; r: periodic interest rate; N: number of compounding period $(1+r)^N$: Future value factor 

and 

**Periodic interest rate ($r$)** = annual interest rate ($IR$)/compounding frequency in a year ($n$), and the equation is as follows:
$$r = \frac{IR}{n}$$
where r: periodic interest rate; IR: annual interest rate; n: number of compounding frequency in a year

### Continuous compounding
**Continuous compounding** is compounding to the (dividing the compound into infinitely small amount and reinvest in that), and the equation is as follows:
$$EAR_{cont} = e^r -1$$
where EAR: Effective annual rate; r: periodic interest rate 

$$FV_{cont} = PV \times e^{rN}$$
where FV: Future value; PV: Present value; r: periodic interest rate; N: number of compounding period


The total interest earned equation is as follows:
$$FV_{cont} - PV$$

or **continuous compounding** can be expressed as: 
$$PV \times(e^{rN}-1)$$
where PV: present value, r: periodic interest rate; N: number of compounding period.
**Note**: In all of the scenario, *r* and N must correspond to the correct time period.

**Understand the difference between simple, compound, and continuous interest:**
https://betterexplained.com/articles/a-visual-guide-to-simple-compound-and-continuous-interest-rates/

![[Pasted image 20220913163112.png]]

**The general principle:** When investing, get interest paid early, so it can compound. When borrowing, pay debt early to _prevent_ that interest from compounding.

eg. 
>John plans to invest $2,500 in an account that will earn 8% per year with quarterly compounding. How much will be in the account at the end of two years?
>
>Answer:
>
>There are eight quarterly compounding periods in two years, and the effective quarterly rate is 8 / 4 = 2%. The account will grow to $$2500\times(1.02)^8 = \$2,929.15$$. Alternatively, since the EAR is $$(1.02)^4 – 1 = 0.082432$$, we can grow the $2,500 at 8.2432% for two years to get $$2500\times(1.082432)^2 = \$2,929.15$$, which is the same result.

#### Present value of a single cash flow
The **present value** of single cash flow equation is as follows:
$$PV=\frac{1}{(1+r)^N}$$is commonly referred as **present value factor**, **present value interest factor**, **discount factor**, where the current value of future cash flow.

>Alice would like to have $5,000 saved in an account at the end of three years. If the return on the account is 9% per year with monthly compounding, how much must Alice deposit today in order to reach her savings goal in three years?
>
>Answer:
> IR = 9%, n = 12, r = 0.075; N = 36, FV = 5000
> FV = PV $\times (1+r)^N$ 
>The effective monthly rate is 9% / 12 = 0.75%, and we can calculate the present value of $5,000 three years (36 months) from now as 5,000 / (1.0075)36 = $3,820.74. Alternatively, since the EAR is 1.007512 – 1 = 0.093807, we can calculate the present value by discounting 5,000 at the EAR for three years. 5,000 / 1.0938073 = $3,820.74, which is the same result.


## Series of cashflows

### Regular cashflows
If a person input a certain amount regularly in investment, there are 3 methods in calculating this:
1st method: 
Future value is the sum of present value after each investment period 
$$FV=PV*(1+r)^{N+1} + PV*(1+r)^N +  [...]$$


2nd method:
$$FV_{N}= A[\frac{(1+r)^N-1}{r}]$$
where FV: future value; A: regular cashflow; r: periodic rate; N: number of times in compounding during the investment period

**Notice: the method assumes cash flows made at the end**

again, we must re-iterate the fact that 
$$r=\frac{IR}{n}$$
where r: periodic rate; IR: annual interest rate; n: compounding frequency within a year

and the 3rd method requires a calculator.

## Time Value of Money functions for BA II Plus Calculator
PV: Present value
FV: Final value
N: Number of compounding period
I/Y: interest rate (periodic rate) in % **Note: do not need to key in % (i.e. 8%, key in "8"; and 5% quarterly = 5/4 = 1.25)**
PMT: annuity **payment** constantly cash flow or constant periodic cash flow of single periodic payment
CPT = Compute

### Uneven cashflows
It is not uncommon to have applications in investments and corporate finance where it is necessary to evaluate a cash flow stream that is not equal from period to period. The time line in Figure 1.2 depicts such a cash flow stream.

![[Screenshot 2022-10-07 at 11.43.08.png]]

This three-year cash flow series is not an annuity since the cash flows are different every
year. In essence, this series of uneven cash flows is nothing more than a stream of annual
single sum cash flows. Thus, to  ind the PV or FV of this cash flow stream, all we need to
do is sum the PVs or FVs of the individual cash flows.

> EXAMPLE: Computing the FV of an uneven cash flow series
> 
> Using a rate of return of 10%, compute the future value of the three-year uneven cash flow stream described above at the end of the third year.
> 
> Answer:
> The FV for the cash flow stream is determined by first computing the FV of each individual cash flow, then summing the FVs of the individual cash flows.
FV1: PV = –300; I/Y = 10; N = 2; CPT → FV = FV1 = 363
FV2: PV = –600; I/Y = 10; N = 1; CPT → FV = FV2 = 660
FV3: PV = –200; I/Y = 10; N = 0; CPT → FV = FV3 = 200
>
FV of cash flow stream = Σ$FV_{individual}$ = 1,223

>EXAMPLE: Computing PV of an uneven cash flow series
Compute the present value of this three-year uneven cash flow stream described previously using a 10% rate of return.
>
Answer:
This problem is solved by first computing the PV of each individual cash flow, then summing the PVs of the individual cash flows, which yields the PV of the cash flow stream. Again the signs of the cash flows are preserved.
>
PV1: FV = 300; I/Y = 10; N = 1; CPT → PV = PV1 = –272.73
PV2: FV = 600; I/Y = 10; N = 2; CPT → PV = PV2 = –495.87
PV3: FV = 200; I/Y = 10; N = 3; CPT → PV = PV3 = –150.26
>
PV of cash flow stream = Σ$PV_{individual}$ = $918.86

## How to calculate uneven cashflow using the BAii Plus Calculator?
https://www.youtube.com/watch?v=tVCJpIq86LI


## Annuity 
**Annuity** is stream of ***equal cash flows*** that occurs at ***equal intervals*** over a ***finite period***. 
Bond price is a typical type of calculation for annuity payment with future set value, and coupon payment is of a (certain rate, periodic cash flow)

There are 3 major types of annuities:
- **Ordinary Annuities** - have the cash flow **at the end** of each time period. 
- **Annuities due** - have the cash flow **in the beginning** of each time period.
- **Perpetuities** - it is like an annuity but it is never ending. (i.e. value of a perpetual bond (a bond with no maturity/due date))

The future value for perpetuity is as follows:
$$FV_{Perp} = \frac{PMT}{r}$$
where FV: future value; perp: perpetuity; PMT: payment; r: interest rate or discount rate .


---
## Questions before starting this section:
- [ ] What is interest rate?
- [ ] What is real vs nominal?
- [ ] Is index fund same as mutual fund?
- [x] What is discount rate?
- [x] What is required rate of return?
- [ ] What is opportunity cost?
- [ ] What is risk?
- [ ] Why is risk important in all calculation?
- [ ] Is the financial market a zero-sum gam?
- [ ] How do banks determine the compounding interest rate?
- [ ] Why does time add/decrease the value of money?
- [ ] What is money?
- [ ] How do borrowing/lending generate money?
- [ ] Why do investment make money?
- [ ] Where do all the money go if a company goes bankrupt?

##  Concept Application
- stock valuation, valuing bonds, and valuing real estate investments.
