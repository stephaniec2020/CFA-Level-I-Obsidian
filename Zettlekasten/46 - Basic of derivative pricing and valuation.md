# 46 - Basic of derivative pricing and valuation
202303042326
Status: #📥 
Tags: [[CFA Level I]]

## Objectives:
- [ ] explain how the concepts of arbitrage, replication, and risk neutrality are used in pricing derivatives.
- [ ] explain the difference between value and price of forward and futures contracts.
- [ ] calculate a forward price of an asset with zero, positive, or negative net cost of carry.
- [ ] explain how the value and price of a forward contract are determined at expiration, during the life of the contract, and at initiation.
- [ ] describe monetary and non monetary benefits and costs associated with holding the underlying asset and explain how they affect the value and price of a forward contract.
- [ ] define a forward rate agreement and describe its uses.
- [ ] explain why forward and futures prices differ.
- [ ] explain how swap contracts are similar to but different from a series of forward contracts.
- [ ] explain the difference between value and price of swaps.
- [ ] explain the exercise value, time value, and moneyness of an option.
- [ ] identify the factors that determine the value of an option and explain how each factor affects the value of an option.
- [ ] explain put–call parity for European options.
- [ ] explain put–call–forward parity for European options.
- [ ] explain how the value of an option is determined using a one-period binomial model.
- [ ] explain under which circumstances the values of European and American options differ.

---

## Derivative benefits
The **benefits** of **derivative** are as follows:
- alter exposure to price risk of underlying asset and transfer to another party
- create exposures not available in cash markets
- facilitate information discovery of the underlying asset
- operational advantages
- greater market efficiency

### Alter exposure to price risk of underlying asset 
There are several situations where derivatives are being used to transfer price risk from one party to another.
- Temporarily reduce exposure to US stock by shorting S&P500 futures - lower transaction cost than selling stocks (and buying back) and less impact on market price of underlying asset
- Korean manufacturer to expect US payment of $10M in 6 months, enter "buy KRW, sell USD" forward to eliminate the exchange rate risk
- Concerned about interest rate will increase, pay fixed interest and receive floating interest swap contract, then pay regular floating rate note

### Create exposures not available in cash markets
**Derivatives** allow exposure not available in cash market such as **call/put options**, where there are limited downside yet remaining with unlimited upside.

Also, if investor is already **long** in cash market, and worried about the downside risk, the investor might choose to have a **put option**. (i.e. long asset + long put)

![[Screenshot 2023-03-05 at 01.32.59.png]]

### Facilitate information discovery of the underlying asset
Derivatives also **facilitate information discovery of the underlying asset**. Forwards and futures prices are often seen as revealing information about the direction of cash markets in the future, particularly in low liquidity markets, or if the underlying market is closed.

For example:
- S&P 500 futures prices before market opening is a good indication of the direction of cash market prices in early trading
- Forward interest rates reflect investors expectations of future central bank benchmark rate decisions
- Option prices reflect the implied volatility of the underlying asset

This allows us to estimate the price risk of the underlying asset.

### Operational advantage
There are several operational advantage of derivative market:
- Easier to short - cash market requires borrowing the underlying asset or might not allow
- Lower transaction cost - commodities derivatives do not have to deal with transportation, storage and insurance add costs to transactions in physical commodities
- Less cash required to take a position - as derivatives are implicitly leveraged
- Higher volumes and liquidity - making it much easier to unwind positions; cash market positions may be difficult to unwind in a low liquidity situation, like when the market is closed or in a market collapse situation.

![[Screenshot 2023-03-05 at 01.37.29.png]]

### Greater market efficiency
The operational efficiency of derivative markets also leads to greater market efficiency, low transaction costs, greater liquidity and leverage and ease of short sales all make it less costly to exploit securities misplacing and improve the efficiency of market prices.

## Derivative risks
There are **5 risks** come with trading **derivatives**:
- **Implicit leverage**
- **Basis risks**
- **Liquidity risk**
- **Counter-party risk**
- **Systemic risk**

### Implicit leverage
Given an investor has just $100, he can only buy $100 worth of stocks in the cash market. However, for a stock with a required margin of 5%, he can potentially enter a $2,000 position in the stock with just $100 cash, 20 times that of the cash market transaction. The risk of investors taking over leveraged positions in the derivative market is much higher, amplifying losses in the event of an adverse market move.

![[Screenshot 2023-03-05 at 01.44.43.png | 600]]

**Structured notes** are a broad category of securities that **incorporate debt instruments with embedded derivatives** to **enhance the yield**.

The problem arises when such notes are **sold as low risk securities** to unsuspecting retail investors who may not understand the highly leveraged positions they undertake from the embedded derivatives.

![[Screenshot 2023-03-05 at 01.46.08.png | 400]]

### Basis risk
**Basis risk** refers to the risk that arises when a **hedged position does not perfectly align with the actual risk of the underlying asset**. Ideally a perfect hedge position should be perfectly opposite that of the underlying performance, such that the net change in value is zero when taken together. However, basis risk occurs when there is a divergence or mismatch between the hedge and the underlying asset, leading to potential differences in their performance or changes in value.

e.g., a manager with a portfolio of large cap U.S. stocks takes on some basic risk if he hedges the position with S&P 500 futures as the S&P 500 is a broad market index. So there are changes in portfolio value despite the hedge. The portfolio may still sustain some losses if the large cap stocks underperform the broad market.

**Basis risk of hedging large cap US stocks with S&P500 futures**
![[Screenshot 2023-03-05 at 01.47.46.png]]

**Basis risk** can also arise in a situation where an investor's horizon and the settlement date of the hedging derivative differ.

e.g. a company that wants to hedge against potential price fluctuations in a commodity it relies on for its operations. The company enters into a futures contract to lock in a specific price for the commodity at a future settlement date. However, the company's actual need for the commodity may occur before or after the settlement date of the futures contract. This timing mismatch can result in a basis risk, where the company may still be exposed to price volatility during the period between the futures contract settlement and the actual commodity purchase. 

**Basis risks of investor's horizon and settlement date**
![[Screenshot 2023-03-05 at 01.48.41.png]]

### Liquidity risk
**Liquidity risk in the context of derivatives** refers to a situation where the cash flows generated from a **hedge do not perfectly align with the cash flows of the investor's positions**. 

e.g., an airline may hedge the price risk of oil by buying oil futures. However, if oil futures price plunges in the midst of the contract such that a margin call is triggered, the airline may have **difficulty raising the liquidity to meet the margin call**. **If the requirement is not met, the position may be prematurely closed** and the airline makes a **loss and loses the hedged position**.

![[Screenshot 2023-03-05 at 02.01.19.png]]

### Counter-party risk
**Counter-party risk** is the risk of the opposite party not meeting the contractual obligation in a derivative contract. The level of counter-party risk varies depending on the type and position of the derivative.

The **counter party risk** with the type of derivatives:
- **Option** -  seller (SHORT) of an option faces no counter-party credit risk because his maximum upside is the option premium which he receives at contract initiation; buyer (LONG) of an option will be owed money at settlement if the option is in the money. So the buyer faces counter-party credit risk if the seller does not fulfil the obligations.
- **Swap** -  either the buyer or seller may be owed money at settlement
- **Forwards** -  either the buyer or seller may be owed money at settlement
- **Futures** - the deposit of initial margin, the daily mark to market and the guarantee of the central clearinghouse all served to reduce counter-party risk

![[Screenshot 2023-03-05 at 02.05.49.png]]

### Systemic risk
**Systemic risk** refers to the risk of widespread impact on financial markets and institutions from excessive speculation using derivative instruments.

## Derivative issuer and investor uses
**Derivatives issuers** are corporate uses derivative instruments. 

These are non-financial corporations that may have risks associated with changes in asset or liability values or cash flows, through:
- volatility from changes in underlying security prices
- market values
- exchange rates
- interest rates

There are several **hedge accounting method** that can benefit from derivatives:
- **Fair value hedge** - aims to **offset the changes in the fair value** of a hedged item by recognising corresponding gains/losses on the hedging instrument (e.g. futures to smoothen the fluctuation of a firm's assets/liabilities; received fixed and pay floating swaps)
- **Net investment hedge** - to **protect the value of investments in subsidiaries or entities** from changes in foreign exchange rates (e.g. SHORT subsidiaries share forwards)
- **Cash flow hedge** - aims to mitigate the impact of future cash flow fluctuations by offsetting them with gains/losses on the hedging instrument (e.g. currency forwards/swaps)

Such companies may take positions in derivatives to hedge against such risks. Such hedges are based on the **assumption that hedge accounting is permitted**. Under this assumption, firms are allowed to recognised gains/losses of qualifying derivative hedges to offset changes in the values of assets, liabilities or cash flows being hedged. In other words, it means the gains/losses of hedged positions are permitted to be recorded to smoothen the fluctuation in value of a firm's asset/liabilities, investment or cash flow.

### Fair value hedge
**Fair value hedge** aims to **offset the changes in the fair value** of a hedged item by recognising corresponding gains/losses on the hedging instrument. 

e.g., a copper miner may carry its inventory at fair market value, which can lead to fluctuations in value as the spot price of copper changes. By selling copper futures, the returns of the futures have an inverse relationship with the value of the inventory, so total assets in the balance sheet will have **less variation from changes in copper price**.

Such is termed a fair value hedge where the gains and losses of hedged positions are permitted to be recorded to smoothen the fluctuation in value of a firm's assets or liabilities. A fair value hedge for liabilities can look like this.

![[Screenshot 2023-03-05 at 02.10.13.png]]

e.g. some companies use fair value reporting for their fixed rate debt in their balance sheet, which means that the reported value of the debt can increase when interest rate decreases. To hedge the interest rate risk, the company may enter an interest rate swap where it receives a fixed rate and pays the floating rate.

![[Screenshot 2023-03-05 at 02.16.43.png]]

### Net investment hedge
**Net investment hedge** is an accounting method used by a parent company to manage the risk associated with fluctuations in the value of its investment in a foreign subsidiary or entity. The investment is typically represented by the equity value of the subsidiary, which is reported on the parent company's balance sheet. 
  
e.g. as the market price of the subsidiary's shares fluctuate, the asset value on parent's balance sheet will vary accordingly. The parent may choose to sell forwards in the subsidiary's shares to hedge against changes in the reported value of the subsidiary.   
When short forwards reach their expiration, the seller of the forward contracts is obligated to fulfil their contractual obligations. At expiration, the short position must deliver the underlying asset to the buyer of the forward contract at the predetermined price and in accordance with the terms of the contract.

![[Screenshot 2023-03-05 at 02.20.53.png]]

### Cash flow hedge
**Cash flow hedge** aims to mitigate the impact of future cash flow fluctuations by offsetting them with gains/losses on the hedging instrument.

e.g., a multinational corporation may have sales in a foreign currency, which are translated to its domestic currency for earnings reporting. Such foreign currency cash flows are subject to exchange rate fluctuations to hedge against exchange rate risk. The company may use currency forwards or swaps. This can potentially smooth earnings in a volatile exchange rate situation.

![[Screenshot 2023-03-05 at 02.21.13.png]]

### Derivative investors
**Derivative investors** are mostly **temporarily hedge against** or **modify certain portfolio risk**.

There are several types of investors who would take advantage of derivatives:
- **Equity portfolio manager** - temporarily increase/decrease exposure by buying/selling index futures; decrease downside risk and preserve upside potential by buying put options
- **Fixed income portfolio manager** - increase duration of bond portfolio by entering an interest rate swap as pay floating, receive fixed party (similar to issuing floating-rate debt and using the proceeds to buy fixed rate bonds)
- **Speculator** - gain exposure to risk of underlying asset at low cost; to buy crude oil forwards to gain long exposure to the price of crude oil (little or no initial funds required)

## Pricing the underlying asset of derivatives
The **pricing of the underlying asset mainly determine by 4 factors**:
- **Expectation**
- **Risk**
- **Benefit** 
- **Cost**

### Expectation and derivatives pricing
For assets that **assumed do not have benefits and costs of holding**, its **expected future price** is simply the spot price multiplied by the discount rate compounded over t periods (i.e. $\mathrm{E(S_T)=S_0\times(1+k)^T}$).

The **future pricing of asset equation** is as follows:
$$\mathrm{E(S_T)=S_0\times(1+k)^T}$$
and by rearranging the **future pricing of asset equation**:
$$\mathrm{S_0=\frac{E(S_T)}{(1+k)^T}}$$
where $E(S_T)$: expected futures price; $S_0$: spot price; $k$: discount rate; $T$: time periods. 
However, there is an element of risk/uncertainty in future price. 

### Discount rate of spot price
**Discount rate** is composed of two parts, which is the **risk-free rate** and **risk premium**.

The **discount rate equation** is as follows:
$$\mathrm{k=R_f+R_p}$$
where $k$: discount rate; $R_f$: risk-free rate; $R_p$: risk premium.

### Risk and derivatives pricing
#### Risk aversion
In order to understand the **risk premium**, we must understand **risk aversion**.

Upon 2 assets with same yield but different levels of risk, **investors** can be:
- **risk neutral** - would be indifferent between the 2 assets
- **risk averse** -  would opt for the risk-free (or less risk) as there is no incentive to take on additional risk
- **risk seeking** - would prefer the risky asset despite both assets having the same expected return

Most investors exhibit risk aversion, implying that they demand an additional return in the form of a risk premium to compensate them for the risk they undertake by selecting a risky asset over a risk-free asset (i.e. $\mathrm{k=R_f+R_p}$). The magnitude of this risk premium must be adequate to sufficiently offset the perceived risk associated with the investment decision.

![[Screenshot 2023-03-05 at 02.50.24.png]]

### Benefits and cost and derivatives pricing
For assets that do come with interim benefits or costs. Such factors should be considered in the valuation of the asset as well.

**Benefits** to holding an asset can be:
- **monetary**
	- dividend payments (stocks)
	- interest pay (bonds)
- **non-monetary**
	- convenience yield (commodities)

**Costs** to holding an asset can be:
- **cost of storage** (commodities)
- **protection/insurance cost** (commodities)

The **net cost of carry** is the **present value of benefits** minus **present value of costs** 
(i.e. $\mathrm{PV(benefits)-PV(cost)}$).

Considering all the aspects, the **spot price (underlying asset) equation** is as follows:
$$\mathrm{S_0=\frac{E(S_T)}{(1+R_f+R_p)^T}+PV(benefits)-PV(cost)}$$
where $E(S_T)$: expected future price; $S_0$: spot price; $R_f$: risk-free rate; $R_p$: risk premium; k: discount rate; $T$: time periods; $PV$: present value

Taking into account all of these costs and benefits, we can describe the relationship between the current stock price of an asset with these four elements as such. Understanding how underlying assets are priced in the stock market is critical to understanding how derivatives are priced.

To understand derivative pricing, it's necessary to establish a linkage between the derivative market and the spot market of the underlying.

![[Screenshot 2023-06-29 at 16.31.47.png]]

## Principle of arbitrage
**Arbitrage** is based on **'the law of one price'**. This law states that **two securities, all portfolios that have identical cash flows in the future, regardless of future events, should have the same price**.

An **arbitrage opportunity** arises when **identical securities**, such as X and Y, are **traded at different prices**. e.g., if X is priced at $5 and Y is priced at $4, an arbitrageur can sell X for $5 and use the proceeds to buy Y for $4, resulting in an immediate profit of $1.

![[Screenshot 2023-03-05 at 03.11.24.png]]

According to **law of one price**, as more arbitrage trades take place, the actions of **arbitrageurs cause prices to converge**. The price of X decreases while the price of Y increases until they reach the same price, **eliminating the arbitrage opportunity**.

![[Screenshot 2023-03-05 at 03.14.55.png]]

In **derivatives**, the **payoffs may not be identical to the underlying asset**, **but they are directly derived from its value at the derivative's expiration**.

The value of a derivative at expiration becomes certain once the value of the underlying asset is determined, even though the underlying asset's value at expiration cannot be predicted with certainty.

This property of derivatives allows investors to **construct hedged portfolios by taking a position in the underlying asset and the opposite position in the derivative simultaneously**. Such portfolios have no uncertainty regarding their value at a future date.

![[Screenshot 2023-03-05 at 03.15.34.png]]

## No-arbitrage pricing
**No-arbitrage pricing** is a pricing principle that ensures the **absence of riskless profit opportunities** in financial markets. 

e.g. A **hedged portfolio** can be illustrated by considering an asset traded at $100 initially, with a forward contract expiring in one year priced at $103. 

An investor can simultaneously:
- **a long position in the asset** at $100: net cash outflow -$100
- **a short position in the forward contract** at $103: no cash flow at initiation; sell at $103 at expiration (3% return without risk)

Referring back to the asset pricing equation, assuming negligible costs and benefits of holding the asset Y, the expected future price is calculated as the spot price compounded by the risk-free rate plus the risk premium.

![[Screenshot 2023-03-05 at 03.18.45.png]]

**Assuming there is no benefit and cost in holding this asset, the expected future asset price**:
$$\mathrm{E(S_T)=S_0\times{(1+R_f+R_p)^T}}$$
where $E(S_T)$: expected future price; $S_0$: spot price; $R_f$: risk-free rate; $R_p$: risk premium; $T$: time periods
If the risk free rate is 3%, the risk premium is 0%  (i.e. $\mathrm{E(S_T)=S_0\times{(1+3\%+0\%)}^T}$)

As risk premium shouldn't be 0%, so **is there a pricing error of the forward at t=0?**

e.g. If the forward contract is priced at $105 with a 2% risk premium

An arbitrageur can:
- **borrow $100 at the risk-free rate of 3%** to buy the asset: net cash outflow: $0, because borrowed money at risk-free rate
- **enter a short position in the forward contract** of $105: at expiration, the arbitrageur sells the asset for $105 to fulfil the contract and uses $103 from the proceeds to repay the loan; earns $2 without investing any cash, taking advantage of the price discrepancy

**The law of one price** states as more arbitrageurs exploit the opportunity, the buying pressure on the asset and the increase in short positions push the asset's price up and the forward price down (i.e. convergence of forward price), converges to the risk-free rate of 3%, eliminating any arbitrage opportunity and reducing the risk premium to zero.

![[Screenshot 2023-06-29 at 16.34.59.png]]

### Pricing of assets vs pricing of derivatives
**Asset pricing** and **derivative pricing** operate on **different principles**. Where **asset pricing assumes risk premium**, while **derivatives pricing relies on arbitrage and risk-neutral pricing principles**.

Asset pricing assumes risk-aversion where risk premium > 0, therefore the **equation of future asset price** is as follows:
$$\mathrm{E(S_T)=S_0\times{(1+R_f+R_p)^T}}$$
where $E(S_T)$: expected future price; $S_0$: spot price; $R_f$: risk-free rate; $R_p$: risk premium; $T$: time periods.

**Derivatives pricing is risk-neutral pricing** ensures that **derivatives do not have a risk premium**, as any priced risk premium would be exploited by arbitrageurs, bringing the price back to its no-arbitrage level, therefore **equation of derivatives price** is as follows:
$$\mathrm{F_0(S_T)=S_0\times{(1+R_f)^T}}$$
where $F_0(S_T)$: expected future price; $S_0$: spot price; $R_f$: risk-free rate; $T$: time periods.

**No-arbitrage derivative price** is unique price for a derivative, determined based on the assumption of no benefit or cost associated with holding the underlying asset.

![[Screenshot 2023-06-29 at 16.32.37.png]]

### No-arbitrage derivative price
**No-arbitrage derivative price** has to satisfy this equation, where the **initial asset position**, combined with the **opposite position taken at the same time**, equals the **net payoff at the expiration of the derivative, discounted by the risk-free rate**.

**No-arbitrage derivative price** equation is as follows:
$$\mathrm{Asset\,position_{(t=0)}+Opposite\,position\,in\,derivative_{(t=0)}=\frac{Net\,payoff_{(t=T)}}{(1+R_f)^T}}$$
where $t$: time; $R_f$: risk-free rate; $T$: expiration

Apply the no-arbitrage derivative price to an example, e.g. long asset, short forward, the **no-arbitrage derivative price** equation would be as follows:
$$\mathrm{Asset\,purchase_{(t=0)}+Short\,forward_{(t=0)}=\frac{Net\,payoff_{(t=T)}}{(1+R_f)^T}}$$
where $t$: time; $R_f$: risk-free rate; $T$: expiration.

![[Screenshot 2023-03-13 at 16.18.00.png]]

## Replication
**Replication** is a strategy that aims to recreate the cash flow and risk attributes of various financial instruments. 

When an investor holds the underlying asset while simultaneously entering into a short position of derivative contract, it enables the replication of a risk-free bond-like position. This means that at the time of expiration, the investor will receive both the principal amount and the associated interest, mirroring the characteristics of a risk-free bond.

![[Screenshot 2023-03-13 at 16.26.23.png]]

**Replication** is the process of creating an asset or portfolio from another asset portfolio and or derivative.

1. In other words, an asset combined with a derivative on the asset can produce a position equivalent to a risk free asset.
2. It follows that the asset and the risk free asset can be combined to produce the derivative.
3. Alternatively, the derivative and the risk free asset can be combined to produce the asset.


In summary of **replication**:
- **Asset - Derivative = Risk-free asset**: This equation suggests that by buying an asset and simultaneously selling a derivative, an investor can replicate the risk-free asset. This means the combination of the asset and derivative produces a position that has similar cash flow and risk characteristics to a risk-free asset.
- **Asset - Risk-free asset = Derivative**: In this equation, an investor can replicate a derivative by subtracting the value of a risk-free asset from the value of the asset. This implies that the combination of the asset and risk-free asset can produce a position that behaves similarly to the derivative.
- **Derivative - Risk-free asset = -Asset**: This equation shows that a derivative can be replicated by taking a short position in the derivative and simultaneously buying a risk-free asset. This means the combination of the derivative and risk-free asset creates a position that is equivalent to being short on the asset.
- **Derivative + Risk-free asset = Asset**: Lastly, this equation suggests that a derivative can be replicated by adding the value of a risk-free asset to the value of the derivative. By doing so, the combination of the derivative and risk-free asset creates a position that is equivalent to being long on the asset.

+asset: Buying an asset. This indicates taking a long position in the asset, expecting its value to increase.
-asset: Selling an asset. This represents taking a short position in the asset, anticipating its value to decrease.
+derivatives: Going long on derivatives. This means buying derivatives, such as options or futures, to benefit from potential price movements.
-derivatives: Going short on derivatives. This involves selling derivatives, aiming to profit from declining prices or hedging against potential losses.
+risk-free asset: Buying a risk-free asset. This refers to investing in an asset, such as a government bond, with a guaranteed return and no risk of default.
-risk-free asset: Borrowing at the risk-free rate. This implies taking a loan or borrowing funds at the risk-free rate, typically using the asset as collateral.
Using this notation, the equations for replication can be understood as follows:

Asset - Derivative = Risk-free asset: By buying an asset and subtracting the value of a derivative, the resulting position is equivalent to holding a risk-free asset.
Asset - Risk-free asset = Derivative: Subtracting the value of a risk-free asset from the asset replicates the derivative position.
Derivative - Risk-free asset = -Asset: Subtracting the value of a risk-free asset from a derivative replicates a short position in the asset.
Derivative + Risk-free asset = Asset: Adding the value of a risk-free asset to a derivative replicates a long position in the asset.

**Asset - Derivative = Risk-free asset (for the sake of exam, just remember this)**

where +asset: buy asset; -asset: sell asset; +derivatives: long derivatives; -derivatives: short derivatives; +risk-free asset: buy risk-free asset; -risk-free asset: borrow at risk free rate.

![[Screenshot 2023-03-05 at 03.22.43.png]]

### Replication example
e.g. a **long forward position** in an asset can be replicated by borrowing at the **risk-free rate** to **purchase the asset** (i.e. $\mathrm{Asset-R_f=Long\,forward}$)

The investor:
- enter into a long forward contract of $103: net $0 cash outflow
- at expiration, under the forward contract, the investor buys the asset at $103 and sell at market price (\$S1); the net profit/loss is $S1 - $103.

Alternatively, the investor can:
- enter the long forward position by borrowing $100 at the risk-free rate using the borrowed funds to buy the asset: net $0 cash outflow
- at expiration, sells the asset at market price (\$S1) and repays the loan by returning $103, resulting in the same net cash flow of $S1 - $103.

This demonstrates that the net cash flows for both portfolios are identical, showcasing how a long forward position can be replicated by purchasing the asset and borrowing at the risk-free rate.

![[Screenshot 2023-03-13 at 16.27.39.png]]

## Price and valuation of Forwards contracts
### Price vs valuation of Forwards
**Price ($F_0$)** refers to the **agreed contract price at which the underlying asset will be bought or sold on the settlement date** in a forward contract. It is a predetermined price that both parties have agreed upon.

**Value ($V$)** represents the actual gain/loss experienced by a party involved in the forward contract **on the day of settlement**.

The **Value ($V$) equation** is as follow:

$$\mathrm{V_{short}=-V_{long}}$$
where V: value.

The **value ($V$) of the contract on expiration date**:
$$\mathrm{V_{T}=S_{T}-F_0}$$
where $V_T$: value on settlement date; $S_T$: underlying spot price; $F_0$: price/contract price for payment on settlement date.
Assumption: No benefits or costs associated with holding the underlying asset.

![[Screenshot 2023-03-13 at 16.33.04.png]]

According to **risk-neutral pricing**, the forward (derivative) price is as follows:
$$\mathrm{F_0= S_0 \times(1+R_f)^T}$$
where $F_0$: price/contract price for payment on settlement date; $S_0$: underlying spot price on day 0; $(1+R_f)^T$ is the compounded risk-free rate; $T$: settlement date.

The **spot price** is through rearranging the equation: 
$$\mathrm{S_0= \frac{F_0}{(1+R_f)^T}}$$
where $F_0$: price/contract price for payment on settlement date; $S_0$: underlying spot price on day 0; $(1+R_f)^T$ is the compounded risk-free rate; $T$: settlement date; as spot price is the present value of forward price.

The **present value of the forward price** can be generalised through any time at **time=t**: 
$$\mathrm{\frac{F_0}{(1+R_f)^{T-t}}}$$
where if the spot price follows this line to expiration, the **value ($V$) of the contract is 0 for both the long and short contract party**.

![[Screenshot 2023-03-13 at 16.43.05.png]]

However, the spot price ($S_t$) fluctuate along the line and the **value ($V$)** of the contract is the **difference** between the **spot price** and the **present value of forward price**.

The value ($V$) of the contract equation of **LONG position** is as follows:
$$V_t=S_t-\frac{F_0}{(1+R_f)^{T-t}}$$
where $V_t$: value of the contract at time t; $S_t$: spot price at time t; $\frac{F_0}{(1+R_f)^{T-t}}$: present value of forward price at time t  $T$: settlement date; $t$: time t; ; whereas the value of the **SHORT** will be the **negative** of **LONG** 
(i.e. -$V_t$).

![[Screenshot 2023-03-13 at 16.48.21.png]]

At the settlement date, if the value ($V_T$) of the contract is as follows:
$$\mathrm{V_T=S_T-F_0}$$
where $V_T$: value of contract at expiration; $S_T$: spot price at expiration date $F_0$: forward price at expiration date (i.e. previously set price at initiation of contract).

![[Screenshot 2023-06-29 at 17.34.28.png]]

### Relationship of value of the forward contract at initiation, during contract and expiration
Therefore, the **value of forward contract** can be summarised as:
- **Initiation** - $V_0=0$
- **During contract** - $\mathrm{V_t = S_t-\frac{F_0}{(1+R_f)^{T-t}}}$
- **Expiration** - $V_T = S_T - F_0$

![[Screenshot 2023-03-13 at 16.52.05.png]]

### Relationship of value of the forward contract at initiation, during contract and expiration (without the assumption of no benefits/cost associated with holding underlying)
When there is a costs and benefits of holding onto the asset, such as **dividends**, **convenience yield** and **interest** as benefits, whereas **insurance** and **storage** as costs. The **shorts** are holding the underlying asset, therefore it **receives the benefits** but **bears costs**. The **longs** have to compensate the **shorts** for not bearing costs.

The **forward contract pricing (considering with costs and benefits of holding the assets)** at different time points of the contract:
- **Initiation**
- **During the contract**
- **Expiration**

A **convenience yield** is a premium associated with holding an underlying asset, rather than the associated derivative security or contract.


The **value ($V$) at initiation of the contract** is:
$$V_0=S_0-S_0=0$$
and the full equation of the **spot price at initiation** with **benefits and costs** is:
$$\mathrm{S_0= \frac{F_0}{(1+R_f)^T}-PV_0(Costs)+PV_0(Benefits)}$$
where $F_0$: price/contract price for payment on settlement date; $S_0$: underlying spot price on day 0; $(1+R_f)^T$ is the compounded risk-free rate; $T$: settlement date; as spot price is the present value of forward price.

The equation of the **present value of forward price** with **benefits and costs** at time **t** is:
$$\mathrm{V_t=S_t-\frac{F_0}{(1+R_f)^{T-t}}+PV_t(Costs)-PV_t(Benefits)}$$
where $V_t$: value of the contract at time t; $S_t$: spot price at time t; $\frac{F_0}{(1+R_f)^{T-t}}$: present value of forward price at time t; $T$: settlement date; $t$: time t; whereas the value of the **SHORT** will be the **negative** of **LONG** 
(i.e. -$V_t$) **Note:** There's a change in sign for costs and benefits.

At last, the equation of the **forward price** with **benefits and costs** at **expiration** is:
$$\mathrm{V_{T}=S_{T}-F_0}$$
where $V_T$: value of contract at expiration; $S_T$: spot price at expiration; $F_0$: Forward price at expiration. since there is no benefits and costs of holding onto the underlying asset anymore.


### Forward rate agreements (FRA)
**Forward rate** is the rate for a loan to be made at some future date. 
e.g. 2y3y means 2 years later borrowing a 3-year loan; 1m4m: 1 month later borrow 4-month loan.

The **spot rate** and **forward rate** ("implied forward rate") should be at **no-arbitrage**.

The general **spot-forward pricing** relationship can be summarised at:
$$(1+S_B)^B = (1+S_A)^A\times(1+Ay(B-A)y)^{B-A}$$
where $(1+S_B)^B$: the value of an investment at time B, where $S_B$ is the rate of return for that period. $(1+S_A)^A$ represents the value of an investment at time A, where $S_A$ is the rate of return for that period. $(1+Ay(B-A)y)^{(B-A)}$ is a factor that adjusts the value from time A to time B. Ay is the average rate of return over the period (B-A), and y represents the compounding frequency within that period.

The **implied forward rate** since it is calculated from the spot rate and not the actual market rate.

![[Screenshot 2023-06-29 at 21.28.54.png]]

**Implied forward rate** is important for entering the contract of **forward rate agreement (FRA)** so that the party can borrow the loan at a fixed rate in the future.

![[Screenshot 2023-03-13 at 17.17.33.png]]

In a **Forward Rate Agreement (FRA)**, there are two parties involved: 
- **long** - believes that the interest rate will increase in the future and wants to secure a fixed rate for future and commence the loan when FRA expires
- **short** -  believes that the interest rate will decrease and wants to lend money at a fixed rate for future, and commence the loan when FRA expires.

At the **initiation of the FRA**, **no payments are exchanged** between the parties. The **FRA contract expires** on the same date that **the loan agreement begins**. The net difference in payments is settled in cash at FRA expiry. This settlement represents the **present value of the interest paid at the end of the loan**. Since the cash is already settled at FRA expiry, it's important to note that **neither party is obligated to enter into a loan agreement**; the FRA contract is settled separately before the loan commencement date. 

Because payments on forward rate agreements are discounted to the beginning of the loan period at the realised rate, they exhibit convexity, whereas payments on interest rate futures are linear (no convexity).

Differences may exist between forward and futures prices for otherwise identical contracts if futures prices are correlated with interest rates. If futures prices are negatively correlated with interest rates, daily settlement of long futures contracts will require cash when interest rates are increasing and produce cash when interest rates are decreasing. As a result the futures price will be lower than the forward price. The difference in price does not provide an arbitrage opportunity or suggest that investors should prefer forward or futures contracts.

The investor in the swap will pay the reference rate and receive fixed-rate payments (on a notional principal amount). The net payments can be replicated by borrowing at a floating rate and investing the proceeds in a fixed-rate bond. The payments could also be replicated by taking a floating-rate loan (or issuing a floating-rate bond) and entering a series of FRAs, but these would not necessarily (or likely) be zero-value FRAs; zero-value FRAs would typically not all have the same fixed rate as swap payments do.

The **price of a swap contract is set such that the contract has a value of zero at initiation**. The **_value_ of a fixed-for-floating interest rate swap contract may vary over its life as the floating rate changes**.

> When interest rates are negatively correlated with the price of the underlying asset, it means that as interest rates increase, the price of the underlying asset tends to decrease, and vice versa. In this scenario, let's consider the implications of this correlation on futures contracts compared to equivalent forward contracts:
> 
> **Mark-to-Market Feature of Futures**:
> - Futures contracts have a mark-to-market feature, which means that the contract's value is adjusted daily based on the current market price of the underlying asset. If the price of the underlying asset decreases (lower price), additional margin deposits are required to maintain the contract's value at the initial margin level.
> - With negatively correlated interest rates and asset prices, when the price of the underlying decreases, the futures contract's value decreases, requiring additional margin deposits. Since interest rates are negatively correlated with the asset price, the interest cost on the additional margin deposits will be higher.
> 
> **Margin Withdrawals in Futures**:
> - Conversely, if the price of the underlying asset increases (higher price), the futures contract's value increases, and excess margin may be available in the account. Traders can withdraw this excess margin as cash.
> - With negatively correlated interest rates and asset prices, when the price of the underlying increases, the futures contract's value increases, allowing margin withdrawals. However, the interest earned on the cash withdrawn will be lower due to the negative correlation with interest rates.
> 
> Considering the above points, when interest rates are negatively correlated with the price of the underlying, the mark-to-market feature of futures results in higher interest costs when additional margin deposits are required, and lower interest earnings when margin can be withdrawn. In contrast, equivalent forward contracts do not have the mark-to-market feature, and the interest cost and earnings remain unaffected by changes in the asset's price. Hence, in this situation, forward contracts may be perceived as more desirable than futures contracts.
> On the other hand, When interest rates are positively correlated with the price of the underlying, the mark-to-market feature of futures means that when additional margin deposits are required (lower price of the underlying), interest cost is lower. When margin can be withdrawn from the account (higher price of the underlying) the interest earned on the cash withdrawn will be higher. This makes futures more desirable than equivalent forward contracts.

![[Screenshot 2023-03-13 at 17.23.33.png]]

Difference in **interest amount**:
$$\mathrm{Diff.\,\,interest\,amount=(S_T-F_0) \times (\frac{L}{360})\times Notional\,principle}$$
 where difference in interest amount: what the long has to pay the short at the expiry of FRA (commenced with the loan); $S_T$: spot rate at expiration date; $F_0$: implied forward rate;  $L$: loan period.
 With that the **difference in interest amount has to be discounted back to the PV**:
 $$\mathrm{\frac{Diff\,interest\,amount}{(1+r)^{L/360}}}$$
where $r$: interest rate at time T (i.e. expiration); $L$: loan period.

## Pricing and valuation of future contracts

### Futures vs Forwards
There are some notable differences between **futures** and **forwards**:
**Forwards**:
- have **fixed constant price** at the **expiration date**
- both parties enter to the contract on the **initiation date**
- **value** fluctuates with spot price

**Futures**:
- future price **fluctuates with spot price** (**no-arbitrage principle (i.e. $V_t$=0)**
- both parties can enter the future contract at any time before expiration
- the value of the contract resets to 0 on a daily basis, since daily gain/loss as realised value in the trader's margin account (i.e. the **mark to market process**) The mark to market adjustment to futures contracts resets the price of the futures contract to the new settlement price, which returns the value of the contract to zero each day.


![[Screenshot 2023-03-13 at 17.30.27.png]]

### The mark to market process:
**At initiation date**, the **futures price** is:
$$\mathrm{F_0=S_0\times(1+R_f)^{t/365}}$$
where $F_0$: future price; $S_0$: underlying spot price on day 0; $t/365$: adjusted to the $R_f$ is expressed (i.e. t/365) as the $R_f$ is reported on an annual basis.  

**After one day**, the **future price** is:
$$\mathrm{F_1=S_1\times(1+R_f)^{t-1/365}}$$
where $F_1$: future price; $S_1$: underlying spot price on day 1; ${(t-1)}/365$: as 1 day has passed and this is the discount value to PV of future price.

The **mark to market process** will then **realised** the trader's **gain/loss**:
$$\mathrm{Realised\,gain\,or\,loss=F_1-F_0}$$
immediate use the future value minus spot price, and the value of the contract is 0 to all traders after the mark to market process.

Therefore, it can be generalised into these formula, **future price equation** is:
$$\mathrm{F_0=S_0\times(1+R_f)^{T-t/365}}$$
where $T$: expiration date; $t$: at time t;$F_0$: future price; $S_0$: underlying spot price on day 0; $t/365$: adjusted to the $R_f$ is expressed (i.e. t/365) as the $R_f$ is reported on an annual basis.  

The **mark to market process** will then **realised** the trader's **gain/loss**:
$$\mathrm{Realised\,gain\,or\,loss=F_{t}-F_{t-1}}$$
where $F_{t}$: future price at time t; $F_{t-1}$: future price at time t-1.

![[Screenshot 2023-03-13 at 17.38.18.png]]

### Margin account maintenance
**Margin account**:
- Traders who engage in futures trading utilise a margin account.
- When trading futures, traders are obligated to deposit an initial margin into their margin account.
- If there is any excess amount in the account beyond the initial margin, it can be withdrawn by the trader.
- However, if the balance in the margin account falls below the maintenance margin level, traders are required to add funds to the account to bring it back up to the **initial margin requirement**.

**Forwards and margin requirements**:
- Unlike futures, forwards typically do not have margin requirements.
- This means that when entering into a forward contract, traders are not required to deposit an initial margin or maintain a margin account.
- Despite this difference in margin requirements, the initial pricing of forwards and futures contracts usually does not differ significantly in practice.

The **relationship** between forwards price vs. futures price in the **change of interest rate** and **correlation between IR and futures**:
![[Screenshot 2023-03-13 at 17.40.35.png]]

### Interest rate futures vs FRA
**Interest rate futures** are traded on exchanges and involve standardised contracts for speculating on or hedging against future interest rate movements.

**Forward Rate Agreements (FRAs)** are customised agreements between two parties in the over-the-counter (OTC) market to fix an interest rate for a future period, commonly used for hedging or speculation.

### Interest rate futures
**Market reference rate (MRR)** is the **forward rate** that applies between A and B.
**Interest rate futures** are quoted on a **price basis** as per the following general formula where traders can long or short at the quoted price.
The **interest rate future** price equation is as follows:
$$\mathrm{FP=100-100\times MRR_{A,B-A}}$$
where $FP$: future price; $MRR$: market reference rate; A: in how long the contract expiry; B: time of the contract. There is an **inverse** relationship between the **forward price (FP)** and the **market reference rate (MRR)**.

**Interest rate future** **LONG** expect the MRR ↓ and the **SHORT** expect MRR ↑. On the other hand, **Forward Rate Agreement (FRA)** **LONG** expect MRR ↑ and **SHORT** expect MRR ↓.

There are differences of **interest rate futures** and **forward rate agreement (FRA)**:

|Features|Interest rate futures|FRA|
|---|---|---|
|Cash settlement|based on settlement date|discounted by MRR|
|Long|expect MRR ↓|expect MRR ↑ (floating  rate receiver)|
|Short|expect MRR ↑|expect MRR ↓ (fixed rate receiver)|

When interest rates are negatively correlated with the price of the underlying, the mark-to-market feature of futures means that when additional margin deposits are required (lower price of the underlying), interest cost is higher. When margin can be withdrawn from the account (higher price of the underlying), the interest earned on the cash withdrawn will be lower. 

![[Screenshot 2023-03-13 at 17.45.34.png]]

**Interest rate futures** are marked to market, meaning their value is **recalculated daily** based on prevailing interest rates, and the calculation is performed using the concept of **basis point value**.

**Basis point value** represents the monetary value of a one basis point (0.01%) change in the futures contract price, allowing traders to quantify their gains or losses based on small fluctuations in interest rates.

The **basis point value (BPV)** equation is as follows: 
$$\mathrm{BPV=NP\times0.01\%\times period}$$
where BPV: basis point value; NP: notional principal., the changes in contract price for 1 bp move in MRR.

To calculate the interest rate future price,
$$\mathrm{FP=100-100\times 2.5\%=97.5}$$
When the MRR decrease from 2.5% to 2.2% 
$$\mathrm{FP=100-100\times 2.2\%=97.8}$$
which is 30 basis points.

For that, using the basis point value:
$$\mathrm{BPV=NP\times0.01\%\times period}$$
$$\mathrm{BPV=$1,000,000\times0.01\%\times 3/12=$25}$$
The MTM will then be:
$$\mathrm{MTM=BPV\times BP}$$
$$\mathrm{MTM=$25\times30=$750}$$
where MTM: marked to market value; BPV: basis point value; BP: basis point
![[Screenshot 2023-03-13 at 17.51.34.png]]

### Forward Rate Agreements (FRAs)
In the context of **Forward Rate Agreements (FRAs)**, the term **"convexity bias"** refers to the impact of convexity on the pricing of FRAs. **Convexity** is a measure of how the relationship between bond prices and bond yields curves, and it introduces a bias in the calculation of forward rates in FRAs.

**Convexity bias in FRAs:**
- In FRAs, the assumption of a linear relationship between interest rates and cash flows ignores convexity effects.
- The omission of convexity in FRA calculations introduces a bias in the calculated forward rates.
- This bias can lead to overestimation or underestimation of actual future interest rates implied by FRAs.
- Considering convexity effects is essential for accurately assessing interest rate risk and making informed financial decisions based on FRA-derived forward rates.

![[Screenshot 2023-03-13 at 17.55.46.png]]

## Pricing and valuation of Swaps
**Swaps** involves **a series of forward contracts**, between two parties to **exchange a series of cash flows over a specified period**. These cash flows are typically based on underlying assets, such as interest rates, currencies, or commodities. **Swaps** are custom, non-standard contracts, less regulated and exposed to counter-party risk. 

### General principles of Swap pricing
There are 4 types of swaps traded OTC:
- Interest rate
- Currency
- Commodity
- Equity

![[Screenshot 2023-03-13 at 18.02.57.png]]

e.g. both parties enter to a swap agreement where there are 3 settlement dates and the price of the forwards are the same.

![[Screenshot 2023-03-13 at 18.08.00.png]]

The **swap price equation** is as follows:
$$\mathrm{F_0(1)=F_0(2)=F_0(3)=FS_0}$$
where $FS_0$: swap fixed price. 

**Note, very important**: The **price** of a **swap initiation may not be zero (i.e. $P \ne 0$)**, but its **value (i.e $V_0=0$)** is zero.

An **off-market forward** is a forward contract that starts with a non-zero value. A **swap** with a fixed swap price **can be decomposed into a series of off-market forwards initiated at time zero with the same settlement price**.

The compensation in a swap is calculated by **discounting** the difference between the actual and **expected cash flows to its present value**. The value of a swap is the sum of the individual values of the off-market forwards used to represent the swap (i.e. $\sum V=0$). The price of a swap is obtained through the replication process.

 ![[Screenshot 2023-03-13 at 18.08.35.png]]


### Pricing of interest rate swaps
Under the **replication rule**, the following equation holds true:
$$\mathrm{Asset + (- Risk\,free\,asset) = Derivatives}$$
where the individual buy the asset through borrowing at risk-free rate equals to long forward.

The cash flow of these two portfolios are equivalent.

This can be applied into swaps as well, where the investor **buy floating rate bond**, borrowed at **fixed rate**, equals to **swap (fixed rate payout)**. The fixed rate payout is denoted as **F**, whereas the floating rate bond is **market reference rate (MRR)**.

![[Screenshot 2023-03-13 at 18.11.40.png]]

In this situation, all of the present value of the fixed rate (**F**) must equate to the Market reference rate (**MRR**) of the floating rate bond, which is the **par swap rate**, this is the no-arbitrage fixed rate. Although unlikely required to calculate for the exam, the concept understanding is important.

![[Screenshot 2023-03-13 at 18.11.54.png]]

> To best replicate the position of the floating rate payer in a swap, the investor can create a synthetic position using other financial instruments. The objective is to mimic the cash flows and risk exposure of the floating rate payer in the swap. Here's how the investor can achieve this replication:

> 1. **Borrow at a Floating Rate**: The investor can borrow funds at a floating interest rate from a bank or the market. This means that the interest payments on the borrowed amount will be based on a floating benchmark rate, such as LIBOR or the prime rate.
> 2. **Invest in Fixed-Rate Securities**: The investor can use the borrowed funds to invest in fixed-rate securities, such as bonds or other debt instruments. Fixed-rate securities pay a fixed interest rate, which will generate predictable cash flows for the investor.
> 3. **Enter into Interest Rate Swaps**: To further manage the interest rate risk, the investor can enter into interest rate swaps. By doing so, the investor can exchange the fixed interest payments received from the fixed-rate securities for floating interest payments, effectively converting the fixed-rate investments into floating-rate investments.
> 
> Through this synthetic position, the investor replicates the cash flows of the floating rate payer in a swap. They will receive variable cash flows from the floating rate investment (borrowed funds) and offset the interest rate risk using the interest rate swap.
> 
> It's important to note that while this synthetic replication can closely match the cash flows of the floating rate payer, there may still be slight differences due to market spreads, transaction costs, and other factors. However, in general, this approach allows investors to achieve a reasonable replication of the floating rate payer's position in a swap.


## Pricing and valuation of Options

### Basics of options
There are 2 types of options:
- **American option ('a')** - maybe exercised **anytime** up to and including the expiration date
- **European option ('e')** - can only be exercised **on** **expiration** date

![[Screenshot 2023-03-14 at 16.50.38.png]]

### European Call Option
The equation of the **LONG CALL**:

$$\mathrm{C_T = max(0, S_T-X)}$$
where $C_T$: call option value, $X$: exercise price; $S_T$: spot price.

On the day of expiration, the long call option can exercise right to buy at the exercise price if the spot price is higher than the exercise price, however, if the spot price is lower than the exercise price, the LONG CALL can let the option expires, resulting in 0 profit, the loss is the option premium (i.e. value of the option).

![[Screenshot 2023-03-14 at 16.54.49.png]]

### European Put Option
Whereas in the situation of **LONG PUT**, if the spot price is below the exercise price, the **LONG PUT** can buy it at the market spot price and sell it to the **SHORT party**. If the spot price is higher than the exercise price, then the **LONG PUT** can let the option expires.

Therefore the equation of **LONG PUT** is as follows:
$$\mathrm{P_T = max(0, X-S_T)}$$
where $P_T$: put option value, $X$: exercise price; $S_T$: spot price.


![[Screenshot 2023-03-14 at 16.57.06.png]]

### Moneyness of options
There are 3 outcomes of the moneyness of the **CALL options**, if immediate exercise of option generates:
- +ve payoff ⇒ in-the-money (i.e. $S_t$ > $X$)
- -ve payoff ⇒ out-of-the-money  (i.e. $S_t$ < $X$)
- 0 payoff ⇒ at-the-money  (i.e. $S_t$ = $X$)
where $S_t$: spot price at time t; $X$: exercise price.
and vice versa for **PUT options**.

![[Screenshot 2023-03-14 at 17.03.35.png]]

**Intrinsic (exercise) value** is the **present value (PV) of the exercise price discounted by the risk-free rate**.

The **present value of exercise price** discounted by the risk free rate is as follows:
$$\mathrm{PV(X)=\frac{X}{(1+R_f)^{T-t}}}$$
where $PV(X)$: present value of exercise price; $X$: exercise price: $R_f$: risk-free rate; $T$: time of expiration; $t$: time now.

The **intrinsic (exercise) value at time t** of the **LONG CALL**:
$$\mathrm{E_t = max(0, S_t-PV(X))}$$
where $E_t$: intrinsic exercise value at time t; $PV(X)$: present value of exercise price; $S_t$: spot price at time t.

The **intrinsic (exercise) value at time t** of the **LONG PUT**:
$$\mathrm{E_t = max(0, PV(X)-S_t)}$$
where $E_t$: intrinsic exercise value at time t; $PV(X)$: present value of exercise price.



![[Screenshot 2023-07-01 at 11.25.36.png]]

### Intrinsic vs time value
The option value/premium is the **intrinsic value + time value (i.e. speculative value)**.

The **LONG CALL** contract value is as follows:
$$\mathrm{C_t = Intrinsic\,value+Time\,value}$$
which differs from the forwards and futures, where at initiation, options have values (which is the option premium paid), since it has time value.

At initiation, since there is no intrinsic value, the option premium that the LONG paid to the SHORT is the time value. Therefore, the **LONG Call option value equation at initiation** is as follows: 
$$\mathrm{C_t =  Intrinsic\,value+Time\,value=0+Option\,premium}$$

As the time progresses, the  time value of a long call option decreases and eventually  to 0 (i.e. time value decays to 0), then the LONG CALL option value is completely the intrinsic exercise value of the contract (i.e. $E_T$). The intrinsic value represents the potential profit if the option is exercised, which is equal to the spot price at expiration if it exceeds the strike price  (i.e. $S_T = E_T$). However, if the spot price is lower than the strike price, the option's value becomes zero if the holder chooses not to exercise it (i.e. $E_T = 0$). 

The intrinsic value serves as the theoretical lower bound for the option's value ($E_t$), as it represents the value of being able to buy the underlying security at the strike price upon expiration. On the other hand, the spot price ($S_t$), represents the upper bound, indicating the value of immediately buying the security in the market.

![[Screenshot 2023-03-14 at 17.29.06.png]]

As for the **put option**:

At initiation, a long put option has no intrinsic value, so the option premium paid by the long to the short consists solely of time value. Therefore, the **equation for the long put option value at initiation** is as follows: $$\mathrm{P_t=Intrinsic\,value+Time\,value=0+Option\,premium}$$
As time progresses, the time value of a long put option decreases and eventually decays to zero. At this point, the value of the long put option is solely determined by its intrinsic value, which represents the potential profit if the option is exercised. If the spot price at expiration is below the strike price ($S_T < X$), the intrinsic value is positive and equal to the difference between the strike price and the spot price ($E_T = X - S_T$). However, if the spot price is higher than the strike price, the option's intrinsic value becomes zero if the holder chooses not to exercise it ($E_T = 0$).

The intrinsic value serves as the theoretical lower bound for the option's value ($E_t$), representing the value of being able to sell the underlying security at the strike price upon expiration. Conversely, the strike price ($X$) represents the upper bound, indicating the value of immediately selling the security in the market.

![[Screenshot 2023-03-14 at 17.30.40.png]]

![[Screenshot 2023-07-01 at 11.58.31.png]]

### Factors that affect value
There are 6 factors which can affect the value of options:
1. **Spot price of underlying asset**
2. **Strike price (exercise price)**
3. **Time to expiration**
4. **Risk-free rate**
5. **Volatility of the underlying asset**
6. **Costs and benefits of holding underlying asset**

#### Spot price of underlying asset
The **current market price of the underlying asset** has a direct impact on the value of both call and put options. 

For call options, as the spot price increases, the option becomes more valuable because the holder has the right to buy the asset at a lower price (i.e. $C_t$ ↑ when $S_t$ ↑). Conversely, for put options, as the spot price decreases, the option becomes more valuable as the holder has the right to sell the asset at a higher price (i.e. $P_t$ ↑ when $S_t$ ↓).

![[Screenshot 2023-03-15 at 13.56.13.png]]

#### Strike price (exercise price)
The **strike price** is the price at which the underlying asset can be bought or sold upon **exercising the option**. 

For call options, a lower strike price increases the value of the option, as it allows the holder to buy the asset at a cheaper price (i.e. when $X$ is low, $C_t$ ↑). In contrast, for put options, a higher strike price increases the value, as it enables the holder to sell the asset at a higher price. (i.e. when $X$ is high, $P_t$ ↑)

![[Screenshot 2023-03-15 at 13.57.24.png]]
![[Screenshot 2023-03-15 at 13.57.39.png]]

#### Time to expiration
The **time remaining until the option's expiration date affects its value**. As time passes, **time decay** determines the value of the option, as the option may decline due to the diminishing chance of favourable price movements. The longer the time to expiration, the greater the potential for the option to gain value.

![[Screenshot 2023-03-15 at 13.59.33.png]]

On the other hand, options with a shorter time to expiration date, there will be less opportunity to fluctuate further from the current spot price ($S_t$).

![[Screenshot 2023-03-15 at 13.59.45.png]]

However, for European put options, the time to expiration might not always be of the case where the value of the option is good with long period of time for expiration. The **LONG PUT** would hope for the option expire sooner since there will be a greater maximum downside compare to maximum upside. Under this case, then the shorter time to expiration **PUT OPTION** is actually more time valuable compared to longer time.

![[Screenshot 2023-03-15 at 14.00.06.png]]

#### Risk-free rate
The **risk-free interest rate** influences the value of options. Higher interest rates increase the value of call options and decrease the value of put options, as they increase the cost of carrying the underlying asset. Conversely, lower interest rates have the opposite effect.

**Long Call Option**: If the risk-free rate is high, the amount of cash that the long call holder needs to set aside to buy the underlying asset at expiration has a lower present value. This increases the time value of the long call option. Conversely, if the risk-free rate is low, the present value of the required cash is higher, leading to a decrease in the time value of the long call option.

![[Screenshot 2023-03-15 at 14.00.22.png|350]]![[Screenshot 2023-03-15 at 14.00.35.png|350]]

**Long Put Option**: The long put option allows the holder to sell the underlying asset at the exercise price upon expiration. If the risk-free rate is high, the present value of the expected proceeds from selling the asset is lower. This disadvantageous effect reduces the value of the long put option. Conversely, if the risk-free rate is low, the present value of the exercise price is higher, benefiting the long put option and increasing its value.

![[Screenshot 2023-03-15 at 14.00.49.png|350]]![[Screenshot 2023-03-15 at 14.01.01.png|350]]

Therefore, the **LONG CALL OPTION** is directly correlated to the risk-free rate, whereas the **LONG PUT OPTION** is inversely related to the risk-free rate.

#### Volatility of the underlying asset
Option prices are influenced by the **volatility** of the underlying asset's price. **Higher volatility leads to increased option premiums**, as there is a higher probability of significant price movements that can benefit option holders.

As such, high volatility means a high time value for both European call and put options. A highly volatile asset is useful for both hedgers and speculators. Hedges can hedge the risk of their exposure to the underlying asset, and speculators can bet on the rise or fall of its price.

![[Screenshot 2023-03-15 at 14.11.03.png]]
![[Screenshot 2023-03-15 at 14.11.13.png]]

#### Costs and benefits of holding underlying asset
Any **costs or benefits associated with holding the underlying asset**, such as dividends or interest payments, can impact the value of options. For example, dividends reduce the value of call options and increase the value of put options, as they decrease the value of holding the underlying asset.

The full equation of the **present value of forward price** with **benefits and costs** at time **t** is:
$$\mathrm{V_t(T)=S_t-\frac{F_0}{(1+R_f)^{T-t}}+PV_t(Costs)-PV_t(Benefits)}$$
In the **CALL OPTION**, the **SHORT** bears the cost but receives the benefits. Therefore, the option value increases to compensate the **SHORT** with the costs, and decrease the option value to compensate the **LONG**.

The reverse hold true to the **PUT OPTION**, where the **LONG PUT** bears the cost, receives the benefits. Therefore, the option value decrease to compensate the **LONG** and increase the option value to compensate the **SHORT**.


![[Screenshot 2023-03-15 at 14.12.52.png]]

#### Summary of factors that affect value of Options
1. Spot price of underlying asset
2. Strike price (exercise price)
3. Time to expiration
4. Risk-free rate
5. Volatility of the underlying asset
6. Costs and benefits of holding underlying asset

![[Screenshot 2023-03-15 at 14.34.15.png]]


## Pricing of Options based on Put-Call Parity
**Put-call parity** is a fundamental concept in options pricing that establishes a relationship between the prices of put options, call options, the underlying asset, and risk-free bonds. It states that the sum of the value of a long call option and the value of a risk-free bond is equal to the sum of the value of a long put option and the current price of the underlying asset.

In order to understand the **put-call parity**, must explain what is:
- **protective put** - underlying asset + long put
- **fiduciary call** - long call + risk-free bond

### Protective put
**Protective put** is a strategy in options trading where an investor holds a **long position in an asset** (such as stocks) and also **purchases a put option on the same underlying asset**. 

The purpose of the **protective put is to limit potential losses on the underlying asset** in case its price declines. If the asset's price decreases, the put option will increase in value, offsetting the loss in the underlying asset.

e.g. suppose an investor owns an asset that has a current price of $S_0$. We shall assume the asset makes no cash payments and has no carrying costs. The end of the holding period is time t at which point the asset will be worth $S_T$. Fearing the possibility that spot price ($S_T$) will decline, the investor buys a put option with an exercise price of $X$.

This put option has a premium of $P_0$. Combined with the value of the asset, the investor's initial position is worth $S_0 + P_0$, which is the investor's money at risk at expiration. 

Based on this value, the value of the put ($P_T$) will be either 0 or $X - S_T$. It can be written down as the equation:
$$\mathrm{P_T = max(0,X-S_T)}$$
where $P_T$: put option value at expiration; $X$: exercise/strike price; $S_T$: spot price at expiration.

There are 2 scenarios at expiration date:
- spot price ($S_T$) > exercise price ($X$)
- spot price ($S_T$) < exercise price ($X$)

#### Spot price ($S_T$) > exercise price ($X$)
If $S_T$ is greater than $X$ at expiration, the asset has performed well and the investor will let the put option expire out-of-the-money, the investor keeps the asset which is worth (i.e. sell at $S_T$).

![[Screenshot 2023-03-15 at 14.54.25.png]]

#### Spot price ($S_T$) < exercise price ($X$)
If $S_T$ is lower than $X$ at expiration, the investor would exercise the put in-the-money. The investor will sell the asset for $X$ dollars.

![[Screenshot 2023-03-15 at 14.53.57.png]]

#### Payoff relationship of protective put
**Protective put** is when the investor receives the benefit of **unlimited upside potential** with the **downside performance** truncated at $X$. (i.e. $S_T$ if $S_T$ > $X$; $X$ if $S_T$ < $X$).

![[Screenshot 2023-03-15 at 14.59.50.png]]

### Fiduciary call
**Fiduciary call** strategy involves purchasing a **call option** on an asset with an exercise price of $X$ that expires at time $T$, along with a **long position in a risk-free zero coupon bond**.

The call option, denoted as $C_0$, has a cost associated with it, while the bond has a present value of $X$ discounted by the risk-free rate, represented as $\frac{X}{(1+R_f)^T}$. By implementing this strategy, the investor allocates funds amounting to $C_0 + \frac{X}{(1+R_f)^T}$.

![[Screenshot 2023-03-15 at 15.08.14.png]]

If spot price at expiration ($S_T$) exceeds the exercise price ($X$), the investor will want to exercise the call option expires in-the-money, the investor sells the bond and uses the proceeds to buy the underlying asset and the investor's ending position is represented by $S_T$.

If spot price at expiration ($S_T$) is lower than the exercise price ($X$), the call expires worthless out-of-the-money and the bond is worth $X$ and the investor ending position is $X$. 

The fiduciary call strategy is designed to take advantage of **potential gains if the call option expires in the money**, while **limiting losses to the cost of the call option and the bond**.

### Payoff of the fiduciary call
The **fiduciary call strategy** combines a **risk-free bond**, whose **payoff remains constant at $X$** regardless of the spot price ($S_T$) of the underlying asset. At expiration, the bond's payoff remains fixed at $X$, represented by a horizontal line on the payoff diagram. 

With a long position in a call option, which exhibits a more complex payoff structure, the call option's payoff starts at 0 when the spot price ($S_t$) is at or below the strike price ($X$), and increases as the spot price ($S_t$) rises to ($S_T$) at expiration. This results in an upward-sloping line on the diagram, representing the increasing payoff of the call option.

When these two positions are combined, the overall payoff follows the shape of the combined lines, creating an orange line that captures the combined payoff of the **fiduciary call strategy** (i.e. $S_T$ if $S_T$ > $X$; $X$ if $S_T$ < $X$).


![[Screenshot 2023-03-15 at 15.14.39.png]]

## Put-Call Parity
Since the payoff **protective put** and **fiduciary call** is essentially the same, the two equations can equate one to another, generating this **put-call parity equation**:
$$\mathrm{S_0+P_0 = C_0 + \frac{X}{(1+R_f)^T}}$$
where $S_0$: spot price at initiation; $P_0$: put option premium at initiation; $C_0$: call option premium at initiation; $\frac{X}{(1+R_f)^T}$: Present value of risk-free bond (discounted) at price $X$.

e.g. At the beginning $t_0$, the underlying asset is priced at \$90. We have both a call option and a put option available for this underlying asset, both with an exercise price ($X$) of $100. The options have a three-month expiration period.

To calculate the present value of the exercise price ($X$):
$$\mathrm{PV(X)=\frac{X}{(1+R_f)^T}=\frac{100}{(1+4\%)^{3/12}}=\$99.02}$$
$\frac{X}{(1+R_f)^T}$: Present value of risk-free bond (discounted) at price X. The risk-free bond that the investor needs to purchase at the initiation is $99.02.

By rearranging the put-call parity formula, 
$$\mathrm{S_0+P_0 = C_0 + \frac{X}{(1+R_f)^T}}$$
$$\mathrm{P_0-C_0 = + \frac{X}{(1+R_f)^T}-S_0}$$
$$\mathrm{P_0-C_0 = + 99.02-90=9.02}$$
The difference between the asset price and the call price is $9.02. This establishes the relationship between the put and call options with the same exercise price.

If, in the market, the put option is trading at $15,
$$\mathrm{C_0= 15-9.02=5.98}$$
The call option should be priced at $5.98 to satisfy the put-call parity equation. However, if there is a significant mispricing between the two options, an arbitrage opportunity may arise, taking into account transaction costs.

![[Screenshot 2023-03-15 at 15.22.11.png]]
![[Screenshot 2023-07-01 at 13.33.59.png]]

### Example of put-call parity
Let's consider the scenario where **Jimmy wants to short a stock but is unable to find a way to take a short position**. In this case, we can use **put-call parity** to create a synthetic equivalent of a short position in the stock.

The **put-call parity equation** is as follows:
$$\mathrm{S_0+P_0 = C_0 + \frac{X}{(1+R_f)^T}}$$
where $S_0$: spot price at initiation; $P_0$: put option premium at initiation; $C_0$: call option premium at initiation; $\frac{X}{(1+R_f)^T}$: Present value of risk-free bond (discounted) at price $X$.

By rearranging the put-call parity formula, 
$$\mathrm{-S_0 =P_0- C_0 - \frac{X}{(1+R_f)^T}}$$
This means that the **short position** in the stock can be **replicated** by taking a **long position in a put option**, a **short position in a call option**, and **borrowing the present value of the exercise price ($X$) at the risk-free rate**.

By constructing this synthetic position, Jimmy can achieve a similar risk and payoff profile as a direct short position in the stock, even if he is unable to find a way to short the stock in the traditional sense.

![[Screenshot 2023-03-15 at 15.27.15.png]]



![[Screenshot 2023-03-15 at 15.29.09.png]]

## Put-Call-Forward Parity
The **Put-Call-Parity** can be extended to **Put-Call-Forward Parity**.

Before explaining, one must remember asset can be created with the **replication method** with risk-free bond and derivative as follows:
$$\mathrm{Asset-Risk\,free\,bond=Derivative}$$
By rearranging the equation, the asset can be created as follows:
$$\mathrm{Asset=Risk\,free\,bond+Derivative}$$
where the derivative can be a forward (i.e. long forward).

### Synthetic protective put
**Synthetic protective put** uses the **risk-free bond** and **long derivative (i.e. forward)** to create long position of underlying asset with minimised risk (i.e. $S_T$ if $S_T$ > $X$; $X$ if $S_T$ < $X$).

**Synthetic protective put** is created by not using cash outlay to buy the asset but has the same strategy as protective put, therefore the equation of **synthetic protective put** is as follows:
$$\mathrm{Risk\,free\,bond+Derivative+Long\,put}$$
where the original protective put equation is as follows:
$$\mathrm{S_0+P_0}$$
where $S_0$: spot price of underlying asset at initiation; $P_0$: long put price. 

The strategy involves a long position in a forward contract with of $F_0(T)$ at expiration and a long position in a risk-free bond, redeemable for exercise price ($X$) at expiration to acquire the asset.

If the put option expires in-the-money (i.e. where the spot price $S_T$ is lower than the $F_0(T)$ price), it is exercised, and the investor's ending position is $X$ (i.e. $X$ if $S_T < X$)

![[Screenshot 2023-03-15 at 15.35.57.png]]

If the put option expires out-of-the-money (i.e. $S_T > X$), the option is not exercised, and the ending position is determined by the value of the asset (i.e. $S_T$ if $S_T > X$).

![[Screenshot 2023-03-15 at 15.36.23.png]]

#### Initiation of synthetic protective put
Since there is no cash outlay for the initiation for forwards, the cash outlay for this strategy is only the put option premium ($P_0$) and the amount to purchase the risk-free bond at present value  (i.e. $\frac{F_0(T)}{(1+R_f)^T}$). 

![[Screenshot 2023-03-15 at 15.37.02.png]]

Since the **synthetic protective** put is essentially similar to a **protective put**, we can derive the equation of the **put-call-forward parity**.

The equation of the **put-call-forward parity** is as follows:
$$\frac{F_0(T)}{(1+R_f)^T}+P_0=C_0+\frac{X}{(1+R_f)^T}$$
where $\frac{F_0(T)}{(1+R_f)^T}$: the forward price discounted to present value; $P_0$: put option premium at initiation; $C_0$: call option premium at initiation; $\frac{X}{(1+R_f)^T}$: Present value of risk-free bond (discounted) at price $X$.

## Valuing a derivative using one-period binomial model
A **binomial model** is based on the idea that over the next period a value will change to one of 2 possible values **one for the up move and the other for the down move.**

In order to value the derivative, we need all **5 factors** to price the derivative:
1. Beginning asset value
2. Up factor
3. Down factor
4. Probability of up move
5. Probability of down move

![[Screenshot 2023-03-15 at 15.47.03.png]]

### Estimate the size of the up or down move
The up-and-down factor (i.e. the size moved from respective movement) is based on the past volatility. However, it is not required to know in the CFA level I curriculum.

### Estimate probability of up move or down move
The **risk-neutral pseudo probability** is a way to estimate the probability of an up move or a down move in the context of option pricing. 

Specifically, the **risk-neutral pseudo probability of an up move** is calculated as follows:

$$\mathrm{\pi_U = \frac{1+R_f-D}{U-D}}$$
where $\pi_U$: risk-neutral pseudo probability of an up move; $R_f$: risk-free rate; $U$: up factor; $D$: down factor.

The **risk-neutral pseudo probability of a down-move** is calculated as follows:
$$\mathrm{\pi_D=1-\pi_U}$$
where $\pi_D$: risk-neutral pseudo probability of a down move; $\pi_U$: risk-neutral pseudo probability of an up move.

Both calculations are based off from the **arbitrage relationship** and **risk-neutral probability** with **risk-free rate**. 

Also, **the size of the down move if knowing the up move** is calculated as follows:
$$\mathrm{D=\frac{1}{U}}$$

### Binomial model to price options
Since the price of the derivatives solely derives value from underlying asset price, the estimated price of the underlying asset would give out an estimate price of options.

Binomial model to price options in 3 steps:
1. Calculate option payoff
2. Calculate expected option value through weighted average
3. Discount the price back to today at $R_f$ rate

![[Screenshot 2023-03-16 at 18.22.40.png]]
![[Screenshot 2023-03-16 at 18.23.09.png]]

Ricky Fernandes, CFA, would like to estimate the intrinsic price of a 1-year call option with an exercise price of $160. The underlying stock was last traded at $180. Ricky estimated the following parameters for the binomial pricing model.

U=1.6  
D=0.625  
Pi_U=0.436  
Pi_D=0.564

Assuming a risk-free rate of 5%, calculate the price of the call option using the binomial model.

Expected price in up move = 180*1.6 = 288  
Expected price in up move = 180*0.625 = 112.50

C+ = 288-160 = 128  
C- = 0

E(C1) = 128 * 0.436 = 55.81

C0 = 55.81/1.05 = $53.15


Another way is to use to **put-call parity approach**.

### Put-call parity approach in option pricing
Since the **protective put** and **fiduciary call** is essentially the same, the two equations can equate one to another, generating this equation:

$$\mathrm{S_0+P_0 = C_0 + \frac{X}{(1+R_f)^T}}$$
where $S_0$: spot price at initiation; $P_0$: put option premium at initiation; $C_0$: call option premium at initiation; $\frac{X}{(1+R_f)^T}$: Present value of risk-free bond (discounted) at price $X$.

![[Screenshot 2023-03-16 at 18.25.22.png]]

## One-period binomial model
The **one-period binomial mode**l is a simplified mathematical model used in options pricing to estimate the value of an option over a single time period. The model **assumes that the price of the underlying asset can either go up or down during that period**.

The **hedge ratio**, also known as **the delta** or the **options elasticity**, is a concept used in the **one-period binomial model to determine the number of shares of the underlying asset needed to hedge the risk associated with an option position**. The hedge ratio tells us the proportion of the underlying asset that should be held to offset changes in the value of the option.

### Hedge ratio in CALL option
The **hedge ratio** is an important ratio where the investor want to be indifferent whether the stock price goes up or down. The hedge ratio only requires the strike price and future spot price to calculate, it does not require probability. By going long on the underlying shares, you effectively mitigate the risk associated with your short position in the call option. In general, to fully hedge a short call position, you should take a long position in hedge ratio ($h$ units) of the underlying asset.

The **hedge ratio equation for CALL option** is as follows:
$$\mathrm{h=\frac{C^+-C^-}{S^+-S^-}}$$
where h: hedge ratio; $C^+$: payoff of the call option when increase (in-the-money); $C^-$: payoff of the call option when decrease (out-of-the-money); $S^+$: spot price increase ; $S^-$: spot price decrease.

and the equation to $C^+$ and $C^-$ is as follows:

The **CALL option is executed at times where spot price** is higher than exercise price:
$$\mathrm{C^+=max(0,S^+-X)}$$
where $C^+$: call option value at expiration; $S^+$: spot price increase in future; $X$: exercise price/strike price of the option.

The **CALL option is voided/not used when spot price is lower** than exercise price
$$\mathrm{C^-=max(0,X-S^-)}$$
where $C^-$: call option value at expiration; $S^-$: spot price decrease in future; $X$: exercise price/strike price of the option.

e.g., in our example of a call option with an exercise price of $45, the calculated hedge ratio is 0.7778. This ratio holds significance when you have a short position in one call option and wish to hedge your exposure. The objective is to reach a state where you are indifferent to whether the stock price rises or falls by expiration.

To achieve this, you would go long on a quantity of shares equal to the hedge ratio for each unit of the call option you have shorted. Suppose the stock price rises to $62.50 at expiration. With the long shares, your position value becomes $48.61. By calculating C plus, the value for the long position, your short option position equates to -$17.50. Consequently, the total value of your portfolio amounts to $31.11.

Similarly, if the share price drops to $40, your share position remains at $31.11, while C minus becomes zero due to the absence of value for the short option position. Thus, the portfolio value remains $31.11 even if the share price decreases to $40.

The name "hedge ratio" becomes clear when you realize that by going long on the underlying shares, you effectively mitigate the risk associated with your short position in the call option. In general, to fully hedge a short call position, you should take a long position in "h" units of the underlying asset, where "h" represents the hedge ratio.

For example, if you have shorted 100 call options, you would need to go long on 778 shares to achieve complete hedging of the position.

![[Screenshot 2023-03-16 at 18.33.46.png]]

### Hedge ratio in PUT option
The **hedge ratio equation for PUT option** is as follows:
$$\mathrm{h=\frac{P^+-P^-}{S^+-S^-}}$$
where h: hedge ratio; $P^+$: payoff of the PUT option when increase (in-the-money); $P^-$: payoff of the PUT option when decrease (out-of-the-money); $S^+$: spot price increase; $S^-$: spot price decrease. **Note:** the hedge ratio should be negative.

![[Screenshot 2023-03-16 at 18.33.58.png]]

## No-arbitrage value of the portfolio
The concept of the **no-arbitrage value** of a portfolio is fundamental in finance and is based on the principle of **eliminating risk-free profit opportunities**. In the context of the **hedge ratio and the one-period binomial model**, the no-arbitrage value of the portfolio refers to the value that **eliminates the possibility of riskless profit by perfectly offsetting the risks associated with the underlying asset and the option position**. By constructing a portfolio that replicates the payoff of the option, investors can ensure that the portfolio's value remains consistent regardless of the future price movements of the underlying asset.

The value of the arbitrageur portfolio at **initiation** is:
$$\mathrm{V_0=hS_0-C_0}$$
where the $V_0$: value at initiation; h: hedge ratio; $S_0$: spot price at initiation; $C_0$: call price at initiation.

The hedge ratio can also allow us to determine the no arbitrage value of the relevant option. Going back to our example, we first look at the investor's position as a portfolio of one short call and long 0.7778 units of shares.

The value of this portfolio is not minus C, not the value of the call option at this point. Let's say the value of the call option is $10 at initiation. So an arbitrageur will receive $10 for writing the contract. 

The price of each share is $50, so the arbitrator will need 38.80 $0.09 to buy 0.7778 shares. In total, the arbitrage power will need $28.89 to fund the portfolio.

Now, remember, one of the rules of arbitrage is that the arbitrage law does not use his own money. As such, he will have to borrow this amount at the risk free rate of 7% at the expiration of the call option.

The value of the portfolio is the value of the stock position minus the value of the call option. We've determined that the value of the portfolio would be 31.11 cents regardless of an up move or down move. 

The value of the arbitrageur portfolio on **expiration date** is:
$$\mathrm{V_T=hS^+-C^+}$$
where the $V_0$: value at initiation; h: hedge ratio; $S^+$: spot price increase on the date of expiration; $C^+$: short call payoff on expiration date.

Since the arbitrageur takes no risk as the hedge ratio is adhered. The portfolio value will be the same regardless of whether the stock goes up or down.

![[Screenshot 2023-03-16 at 18.37.59.png]]

In efficient market, the arbitrage opportunity does not exist, where the value of the portfolio is equal to the loan repayment for no-arbitrage opportunity.

In the no-arbitrage opportunity, the equation is as follows:
$$\mathrm{V_T=hS^+-C^+=Loan\,repayment}$$
where $V_T$: value of contract at expiration; $h$: hedge ratio; $C^+$: call option price when the increase spot price is higher than call exercise price. 

Therefore, the loan amount is the present value of the $hS^+-C^+$:
$$\mathrm{Loan\,value = PV(hS^+-C^+)}$$
and under no-arbitrage opportunity, at initiation, the value should be:
$$\mathrm{V_0=hS_0-C_0 = PV(hS^+-C^+)}$$
After rearranging the price of $C_0$, the price of the CALL option:
$$\mathrm{C_0 = hS_0-PV(hS^+-C^+)}$$
and it is the same **price** as calculated using **1-period binomial model**.

![[Screenshot 2023-03-16 at 19.10.42.png]]

In essence, you should use this formula to calculate the no arbitrage value of a call option. If you prefer to make use of the **hedge ratio** instead of using **probabilities**.

![[Screenshot 2023-03-16 at 19.21.19.png]]


### Arbitrageur example

![[Screenshot 2023-03-16 at 19.30.16.png]]



### What to do in each scenario?
Airline should enter into an option contract, such that if oil prices increase, it can exercise the option to buy at the fixed price.

Copper miner should enter into a swap as this ensures that it can receive periodic fixed payments for the copper that it sells.

Speculator should short gold futures contracts such that when the price of gold drops, the futures contracts will be in-the-money.






---
## Questions before starting this section:
- [ ]


> An investor calculates that the premium of a European put option is less than its value based on put-call parity. In exploiting this arbitrage opportunity, the investor is _most likely_ to: Put-call parity indicates that P = C + PV(X) – S. With P < [C + PV(X) – S], the arbitrage transaction is to buy the put and sell the call, borrow the PV of the exercise price (X), and buy the stock.