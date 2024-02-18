# 45 - Derivatives market & instruments
202303040154
Status: #📥 
Tags: [[CFA Level I]]

## Objectives:
- [ ] define a derivative and distinguish between exchange-traded and over-the-counter derivatives.
- [ ] contrast forward commitments with contingent claims.
- [ ] define forward contracts, futures contracts, options (calls and puts), swaps, and credit derivatives and compare their basic characteristics.
- [ ] determine the value at expiration and profit from a long or a short position in a call or put option.
- [ ] describe purposes of, and controversies related to, derivative markets.
- [ ] explain arbitrage and the role it plays in determining prices and promoting market efficiency.

---
## Derivative definition and feature
**Derivative** is a financial instruments where it derives the value from performance of underlying asset. 
There are several types of derivatives:
- **Forwards** - Financial contracts between two parties to buy or sell an asset at a specified future date and price, with no obligation to trade on an exchange (i.e. OTC).
- **Futures** - Standardised contracts traded on exchanges that obligate the buyer to purchase and the seller to sell an asset at a predetermined future date and price.
- **Swap** - Agreements between two parties to exchange cash flows or other financial instruments based on predetermined terms, often used to manage interest rate or currency risks.
- **Options** - Contracts that give the buyer the right, but not the obligation, to buy (call option) or sell (put option) an asset at a specified price within a predetermined time period.
- **Credit derivatives** - Financial instruments used to manage credit risk, allowing investors to transfer or hedge credit exposure associated with debt securities or loans.

### Basic features of a forward derivative
There are two parties entering into a forward contract, where there is an **underlying asset**.
It is settled in the future at the **settlement date (expiry date)**. At the same time, there is a **forward price** in which both parties agree to transact the asset on the **settlement date**, and the **contract size** is the quantity of the asset that is going to be transacted.

![[Screenshot 2023-03-04 at 02.06.03.png]]
There is a difference in **price** and **value** of the forward contract. The **price** is the **forward price** stated in the contract, where as the **value** is the **gain/loss to the contract party** when entering into the contract, and it will depend on the **spot price** of the underlying asset on the **settlement date**. **Spot price** is the price of the underlying asset for immediate delivery. 

The contract can either be **deliverable** or **cash-settled** contract. The **deliverable** contract requires physically deliver of the asset. In a **cash-settled** contract, the party which loss money has to settle the contract in cash and transfer the money to the party which gained from this contract. Both are delivery method are economically equivalent. 

## Derivatives Underlying and use
**The underlying use of derivatives** are for **risk transfer**. In the example of transport company, the operational cost ↑ when the fuel price ↑. When the fuel price ↑, the transport company can profit from long position, which can offset higher operational costs. On the other hand, the oil producer might want to enter a short, as the revenue ↓ when oil price ↓. When fuel price ↓, the oil company can profit from short position and can offset lower profits from sales. This is known as **risk hedging**.

![[Screenshot 2023-03-04 at 02.20.54.png]]

To remember what to do in forward market, **buy** the underlying asset ⇒ **long** forwards; **sell** the underlying asset ⇒ **short** forwards.

There are other types of commodities for trading:
- Hard commodities (mined/extracted) - precious metals, industrial metals
- Soft commodities (grown/reared) - cotton, coffee, wheat, cattle

Besides commodities, there are other **assets** can be traded as derivatives:
- Stocks/bonds
- Indexes
- Cryptocurrency

Also, **variables** can be traded as derivatives:
- Interest rate
- Exchange rate
- Weather

There are several needs for using derivatives:
- Hedge portfolio exposure
- Hedge interest rate risk of debt obligation
- Hedge currency exchange uncertainty on future cash flow

### Hedge portfolio exposure
Investors sometimes hedge their exposure to stocks and bonds they own through futures contracts, which are very much like forward contracts.

For example, a portfolio manager may be concerned that the US stocks in his portfolio are overvalued and that a correction is imminent.

He can hedge the risk of a deep correction in U.S. stocks by shorting futures on the S&P 500 index. The advantage of making this derivative trade instead of selling first and buying back later is that the transaction cost is likely to be lower. Also, initiating positions in the derivative market may have less impact on market prices of the underlying.

### Hedge interest rate risk of debt obligation
Interest rate swaps allow participants to hedge the interest rate risk of their debt obligation. e.g, if a floating rate borrower expects interest rates to increase, he may enter into a swap to pay regular fixed rate payments in the future and receive floating rate payments to satisfy his floating rate obligations.

### Hedge currency exchange uncertainty on future cash flows
An exchange rate forward allows global trade participants to hedge currency exchange uncertainty on their future cash flows. For example, a European manufacturer may be expecting to receive a large payment in Australian dollars in six months, but is concerned that the exchange rate may be unfavourable in six months. It can enter into a forward contract to sell Australian dollars for euros at a fixed forward rate. 

![[Screenshot 2023-03-04 at 02.25.57.png]]

Besides passing on risk they are exposed to as hedgers, derivatives attract another party, speculators. The speculators require little/no cash at initiation, it can gain exposure at a low cost and create high leveraged investment in the underlying. 

## Derivatives market
**Derivatives** can be created and traded over a **central exchange** or **over the counter (OTC)** at decentralised locations.

In OTC markets, participants enter into custom contracts directly with each other.

![[Screenshot 2023-03-04 at 02.33.56.png]]


After the 2008 global financial crisis, regulators worldwide instituted a central clearing mandate that required a central counter-party to take on the counter-party credit risk for both sides of a contract similar to the role of a clearinghouse. 

When a dealer enters into a swap contract with a counter-party, he is required to send the information to a swap execution facility. The CCP replaces the trade with two trades and acts as the counter-party to both of them, thereby reducing counter-party risk for both. However, the downside of this structure is that counter-party risks are concentrated on a single entity rather than distributed among financial intermediaries.

![[Screenshot 2023-03-04 at 02.35.23.png]]

## Forward commitment vs Contingent claim
The derivative can be subdivided by the nature of the contract:
- **Forward commitment** - A **forward commitment** is a contract where the parties are **obliged** to perform some action at a specific time in the future.
  e.g. Futures (Central exchange), forwards (OTC), swaps (OTC)
- **Contingent claim** - A **contingent claim** is only **claimable** by the contract buyer if a **particular event happens before the expiry** of the contract, somewhat like an **insurance** contract. 
  e.g. Option (Central exchange), credit derivatives (Central exchange)

**Note:** **Credit default swap**, although named as a swap, is actually a contingent claim option, as the payoff is contingent based on the event of a default.

![[Screenshot 2023-03-04 at 02.40.21.png]]

## Forwards
In **forwards** contract, the **long** commits to **buy** the underlying at the forward price while the **short** commits to **sell** the underlying on the **settlement date**.

The **payoff** equation is as follows:

$$\mathrm{Payoff=Spot\,price-Forward\,price}$$


If the spot is higher than the forward price, this amount is positive, so the long makes a gain.
the short is the opposite of that for the long. So if the spot price is below the forward price at settlement, the short makes a gain.

The payoff profile is a useful graph to help us understand the characteristics of a derivative.
**Forwards** is a linear derivatives.
![[Screenshot 2023-03-04 at 02.46.03.png]]

**Forwards** are traded OTC, they are subjected to counter-party risk. The contracts are normally custom and negotiated, which are non-standard form of contract. They are tend to be less regulated.

## Futures
**Futures** is traded through central exchange. The clearinghouse enforces margin requirements on both the long and the short, which is the primary tool to reduce counter-party risk.

To facilitate trading Futures are **standard** contracts where traders either take the long or short position with **standard contract sizes** and **standard terms** to expiration. Futures markets are usually regulated by authorities

**Futures price** is not like stock price where the stock buyer pays the quoted price to the seller for the stock. Rather, futures price is the price that the long and the short agree on for the **settlement in the future**. No cash is paid between the long and the short at this point.

**Settlement price** is the **closing price for a futures contract at the end of the trading day**, but is not simply the price of the final trade of the day. It is an **average of the prices of the trades during the last period** of trading called the **closing period**. This specification of the settlement price makes it harder for traders to manipulate the settlement price.

![[Screenshot 2023-03-04 at 02.54.12.png]]
Be very clear that for futures, the requirement in a margin call is to top up to the initial margin,

![[Screenshot 2023-03-04 at 02.54.50.png]]

## Swaps
**Swaps** are very similar to **forwards**, where swaps can be view as series of forwards. Forwards have custom, non-standard contracts, less regulated, have counter-party risk. **Swap** is known as **exchange** a series of payments on **periodic** settlement dates over a **certain period**.

![[Screenshot 2023-03-04 at 02.56.46.png]]

![[Screenshot 2023-03-04 at 02.58.39.png]]

## Options
**Options** give the **buyer the right** to buy (call option) or sell (put option) an asset at a specified price within a predetermined time period, while the **seller is obligated** **to fulfil the contract if the buyer decides to execute it**.

When the risk-free rate is high, a call option will be valued higher, while a put option will be valued lower.

The short put is obliged to buy the underlying if the long put decides to exercise the put option.

Storage costs increases the value of a call option, but decreases the value of a put option.


 >Harvey is holding on to a bond as he is confident that its price will continue to rise. However, he would prefer some protection from a drop in price in the event that the company’s credit rating deteriorates. Which derivative is most appropriate for his situation?  **Credit spread option on the bond**
> Forward contract is not that appropriate as he would not be able to participate in the upside of the bond price.  Credit default swap is not that appropriate as it only pays out in the event of a default.





---
## Questions before starting this section:
- [ ]