# 14 - Currency exchange
202304261521
Status: #📥 
Tags: [[CFA Level I]]

## Objectives:
- [ ] define an exchange rate and distinguish between nominal and real exchange rates and spot and forward exchange rates.
- [ ] describe functions of and participants in the foreign exchange market.
- [ ] calculate and interpret the percentage change in a currency relative to another currency.
- [ ] calculate and interpret currency cross-rates.
- [ ] calculate an outright forward quotation from forward quotations expressed on a points basis or in percentage terms.
- [ ] explain the arbitrage relationship between spot rates, forward rates, and interest rates.
- [ ] calculate and interpret a forward discount or premium.
- [ ] calculate and interpret the forward rate consistent with the spot rate and the interest rate in each currency.
- [ ] describe exchange rate regimes.
- [ ] explain the effects of exchange rates on countries’ international trade and capital flows.
---
## Foreign exchange rates
### Definition
**Exchange rate** is the price of currency X (1 unit of base currency) in terms of currency Y (i.e. price currency). It is the **price currency/base currency** (i.e. the slash can be read as per). 

For example, USD/GBP = 1.3 indicates price of 1 GBP is 1.3 USD. 
![[Screenshot 2023-05-01 at 18.30.03.png]]

### Direct vs indirect quotes
**Direct quote** is the point of view of an investor in **price currency** country. **Indirect quote** is the point of view of an investor in the **base currency** country. 

![[Screenshot 2023-05-01 at 18.30.26.png]]

When calculating the percentage change in one currency relative to another, you should be aware that the calculated change is only in terms of the base currency and should not be reciprocated to the price currency.

For example, if the U.S. dollar per great British pound rate falls from one point three to one point one, the percentage change in the dollar price of one GBP is simply minus fifteen point four percent

because one GBP now buys fifteen point four percent less dollars.

It's correct to say that the GBP has depreciated fifteen point four percent relative to USD. However, it's not correct to say that the dollar has appreciated by fifteen point four percent to calculate the percentage change in USD relative to GBP. We need to set USD as the base currency.

### Nominal vs. real exchange rates
Another key distinction for exchange rates is between the **nominal exchange rate** and the b, **nominal exchange rate** is what we've been talking about so far, which is the quoted exchange rate at a point in time.

The **real exchange rate**, however, takes into account the **relative price changes** between the **two countries from a base period**, you may wonder why would the relative price changes be important?


Assuming that the nominal exchange rate is unchanged for the period, but the price levels in the UK have gone up by 15 percent, but only by three percent in the US, you would be very worried if the

GBP price of the clocks go up by 15 percent while U.S. inflation is only three percent for the period. It probably means that your clocks wouldn't sell that well if American income only went up by 3 percent.

So as you can see, even though the nominal interest rate is unchanged, the real cost of import has increased for the U.S. importer.

Nominal interest rate is unchanged, the real cost of import has increased for the U.S. importer.

Let's see how the real exchange rate differs to calculate the real exchange rate, we multiply it by

the factor of the CPI of the base currency against the CPI of the price currency.

Do note that the base is on top in this case, even though the nominal exchange rate remains unchanged,

$$\mathrm{Real \,exchange\,rate = Nominal\,exchange\,rate \times \frac{CPI_{base\,currency}}{CPI_{price\,curreny}}}$$

$$\mathrm{1+\Delta Real \,exchange\,rate = 1+\Delta  Nominal\,exchange\,rate \times \frac{1+CPI_{base\,currency}}{1+ CPI_{price\,curreny}}}$$

**Real interest rate increase** - relative cost to import from UK to US is higher, relative purchasing power of American vs. British has declined.

![[Screenshot 2023-07-05 at 17.15.23.png]]

Change in rate has to be set in terms of the base currency.

![[Screenshot 2023-05-01 at 18.43.26.png]]

>Assuming no changes in the prices of a representative consumption basket in two currency areas over the measurement period, changes in the nominal exchange rate: are equal to changes in the real exchange rate.

![[Screenshot 2023-07-14 at 21.39.52.png]]


### Cross rates
So these market quotes are the most relevant.

For a pair of relatively less traded currencies like the Malaysian ringgit and the New Zealand dollar,

there may not be an active trade in the pair, so the exchange rate may not be that current.

If we want to have a more current exchange rate between the two, we can calculate the cross rate between them.

![[Screenshot 2023-05-01 at 18.50.22.png]]
![[Screenshot 2023-05-01 at 18.51.36.png]]
![[Screenshot 2023-05-01 at 18.51.52.png]]

## Forward exchange rates
### Spot vs forward rates
A **spot exchange rate** is the currency exchange rate for **immediate delivery, which for most currencies means the exchange of currencies takes place two days after the trade (i.e. T+2**).

A **forward exchange rate** is a currency exchange rate for an **exchange to be done in the future, which can be 30 days, 60 days, 90 days, 180 days or one year**.

When a firm **buys or longs a currency forward**, it's **obliged** to **exchange a specific amount of the base currency for a specific amount of price currency on a future date specified in the contract**.

#### Forward exchange rate quote
A **forward exchange rate quote** can be expressed as an **absolute value**, or in terms of the difference between the spot exchange rate and the forward exchange rate (**relative exchange rate**; i.e. spot+pts or pip). Remember, **one pip** is 0.0001 or the 4th decimal place.

### Forward premium/discount
**Forward premium** is when the forward rate is **higher** than the spot rate, which is the **base currency is expected to appreciate**, and the **price currency expect to depreciate**. E.g. AUD/EUR, EUR buys more AUD in the future, then it is EUR is expected to appreciate and AUD expect to depreciate.

Conversely, **forward discount** is when the forward rate is **lower** than the spot rate, which is the **base currency expected to depreciate** and the **price currency expect to appreciate**. E.g. AUD/EUR, EUR buys less AUD in the future, then it is AUD is expected to appreciate and EUR expect to depreciate.

The forward exchange rate equation is as follows:
$$\mathrm{Forward\,premium\,or\,discount = \frac{Forward\,rate}{Spot\,rate}-1}$$
The forward exchange rate can be annualised through 
Annualise to number of years:
$$\mathrm{1/num.\,of\,yrs}$$
Annualise to number of months:
$$\mathrm{12/num.\,of\,months}$$
Annualise to number of days:
$$\mathrm{360/num.\,of\,days}$$
need to check whether 365 should be used or 360.

>Spot CNY/HKD = 0.9434  
>180-day CNY/HKD forward = Spot – 73pts
>
>What is the annualised premium/discount for the 180-day CNY/HKD forward?  **-1.55%**
>
>180-day CNY/HKD forward premium/discount = -73pts/0.9434 = -0.0073/0.9434 = -0.7738%
>Annualised discount = -0.7738% x 360/180 = -1.55%


### Arbitrage relationship
The **arbitrage relationship** determines the forward premium/discount.
An arbitrageur can 
This will continue to increase to the no-arbitrage spot rate. In the no-arbitrage opportunity situation, the forward exchange rate will be adjusted to be net-zero for arbitrageur profit.

The equation for the no-arbitrage relationship:
$$\mathrm{Forward\,rate=Spot\,rate \times \frac{1+r_price}{1+r_base}}$$
![[Screenshot 2023-05-01 at 19.27.48.png]]
![[Screenshot 2023-05-01 at 19.32.31.png]]

### FX market
In the forex market, there are several types of participants:
- Firms that are going to receive huge sum of foreign currency (reduce or eliminating its foreign exchange risk) - **risk hedge**
- Firms that wants to expose to foreign exchange risk - **speculation**
- Sell-side - large FX trading banks (e.g. citigroup, UBS, Deutsche bank)
- Buy-side - clients who buy FX products from sell-side banks
	- Corporations - that frequently engage in cross-border transactions - hedge risk of future receipt payment in foreign currency
	- Real money accounts - mutual funds, pension funds, insurance companies, institutional accounts - hedge currency risk or foreign securities
	- Leveraged account - hedge funds, HFT, trading desks at proprietary trading firm or banks - actively 
	- Retail market - FX transactions by households and relatively small institutions (tourism, cross-border investment, speculative trading) 
	- Government and government entities
		- Government - acquire foreign currencies for transactional needs
		- Central bank - engage in FX transactions to affect exchange rates
		- Sovereign wealth funds - use FX derivatives to hedge currency risks and speculate

## Exchange rate regimes
**Exchange rate regimes** refers to the policy framework that the central bank adopts to manage the exchange rate. 

The IMF categorizes exchange rate regimes into the following 2 types for countries that do not issue their own currencies and 7 types for countries that issue their own currencies:
**Countries that do not issue their own currencies**:
- Formal dollarisation
- Monetary union
**Countries that issue their own currencies**
- Currency board system
- Fixed peg
- Target zone
- Crawling pegs
- Crawling bands
- Managed float
- Independent float

### Countries that do not issue their own currencies
#### Formal dollarisation
**Formal dollarisation** uses the currency of another country. For countries uses formal dollarisation:
- it cannot have its own monetary policy
- have the credibility of the used currency
- do not have the creditworthiness of the used currency government
- do not have the insurance for the currency used for bank deposits (different interest rate than the currency used).

#### Monetary union
**Monetary union** is when several countries use a common currency. The most obvious monetary union is the **European Economic and Monetary Union**, although member countries **cannot have their own monetary policies**, they **jointly determine monetary policy** through their representation at the European Central Bank.

Member nations inherit:
- credibility of euro
- not the creditworthiness of the Eurozone ⇒ government bonds of various Eurozone nations have different yields

### Countries that issue their own currencies
#### Currency board system
A **currency board** arrangement is an explicit commitment to exchange domestic currency for a specified foreign currency at a **fixed exchange rate.** The domestic currency is fully backed by foreign assets.

The Hong Kong dollar is a classic example of this, where U.S. dollar reserves are held to cover the entire monetary base.

This means that for every Hong Kong dollar issued by the central bank, the central bank holds an equivalent amount of U.S. dollars in reserve.

In contrast to dollarisation, the Hong Kong Central Bank can earn interest on its U.S. dollar reserves.

A fixed exchange rate means:
- the central bank gives up the ability to conduct independent monetary policy 
- In the long run, essentially imports the inflation rate of the US economy
- In the short run: there may be some leeway for the central bank to influence interest rates.

#### Fixed peg
In a **conventional fixed peg** arrangement, a country pegs its currency within margins of $\pm$ 1% vs. **another currency**, or **a basket that includes the currencies** of its major trading or financial partners.

Few ways of countries can maintain fixed peg:
- **Direct intervention** - the **central bank** **maintain** exchange rates within the band **by purchasing or selling foreign currencies** in the foreign exchange markets
- **Indirect intervention** 
	- adjusting the policy interest rate
	- regulating FX within its jurisdiction

As compared to the regimes we've discussed earlier, the **fixed peg regime** allows the central bank to retain **more flexibility to conduct monetary policy**. However, there are still limitations due to the requirement to maintain the peg.

![[Screenshot 2023-05-01 at 19.57.42.png]]

#### Target zone
Under a **target zone** regime, the permitted fluctuations in currency value relative to another currency or basket of currencies are wider around $\pm$ 2%.

Compared to a conventional peg, the central bank has **more policy discretion** because the bands are wider.

![[Screenshot 2023-05-01 at 19.58.01.png]]

#### Crawling peg
With a **crawling peg**, the exchange rate is adjusted periodically, typically to **adjust for difference in inflation against the currency used in the peg**.

**Passive crawling peg** is when the adjustments are made as and when there is a **need** to.
**Active crawling peg** is the adjustments are **planned and announced** in advance. An **active crawling peg** can influence inflation expectations, adding some predictability to domestic inflation.

**Monetary policy** is **restricted** in pretty much the same way it is with a **fixed peg arrangement**.

![[Screenshot 2023-05-01 at 19.58.18.png]]

#### Crawling bands
Under a **crawling bands** regime, the width of the bound that the central bank allows the exchange rate to fluctuate is increased over time.

The band is initially tight for a developing country to anchor expectations about future inflation to investors. When the country attains credibility, the bonds are widened such that the central bank has more flexibility and greater scope for monetary policy.

![[Screenshot 2023-05-01 at 20.01.02.png]]

#### Managed float
Under a **managed float** regime, the exchange rate target and band is typically not fixed and not explicitly made known to the public, the central bank decides whether to intervene **based on its policy objectives** like achieving trade balance, price stability or employment levels.

Under such a regime, the central bank has higher flexibility to implement monetary policy than all that we've discussed before.


![[Screenshot 2023-05-01 at 20.02.32.png]]


#### Independent float
The most hands off exchange rate regime is the **independent float**.

The **exchange rate is market determined**, so there's **no exchange rate target or trading band**. However, central banks do intervene at times to slow the rate of change and reduce short term volatility. The aim is not to keep exchange rates at a target level.

This regime allows the central bank to have the most flexibility in implementing monetary policy.

![[Screenshot 2023-05-01 at 20.04.37.png]]

## Exchange rates, international trade, and capital flow
### Balance of trade vs capital flows
When a country spends on **imports more than it earns from exports (i.e, X-M < 0)** , the **trade deficit** is financed either by **borrowing from foreign countries or selling assets to foreign countries**.

From the balance of payments point of view, a **current account deficit** must be exactly matched by an **offsetting capital account surplus**. We can study the impact of **changing exchange rates** on the balance of payments from two different angles:
- the impact on imports and exports (current account deficit) - **elasticity approach**
- the impact on capital flows (capital account surplus) - **absorption approach**

**Note**: Capital account = Capital account + financial account 

### Elasticities approach
The **elasticities approach** focuses on how **exchange rate** changes **affect total expenditures on imports and exports**. One shortcoming of elasticities approach is that it **only considers the microeconomic relationship between exchange rates and trade balances**, it **ignores capital flows**, which must also change as a result of a currency depreciation that improves the balance of trade.

If a country **wants to reduce its trade deficit**, it needs to **depreciate its currency**. **Depreciation** of the domestic currency will **make imports more expensive** in domestic currency terms and **exports less expensive in foreign currency terms**.

However, it is not always the case since the objective is the change in **total expenditures** on imports and exports. This means understanding the **price elasticity of demand for export and import goods** is needed determine if the desired change can be achieved.

#### Situation of inelastic import and export goods
Consider if both demand curves are inelastic, a depreciation in the domestic currency decreases the foreign price of exports, but the quantity demanded may only increase a little. This means that the total value of exports decrease instead of the intention to increase it.

Likewise, a depreciation in the domestic currency increases the domestic price of imports, but the quantity demanded may only decrease a little. This means that the value of imports increase instead of the intention to decrease it.

If both of these effects play out, the trade deficit actually widens instead of narrowing.

![[Screenshot 2023-05-01 at 20.46.27.png]]

This is the generalised Marshall-Lerner condition, which is based on the proportion of total trade that is exports and imports and the price elasticity of demand for exports and imports.

The Marshall-Lerner condition equation (general):
$$\mathrm{w_x\epsilon_x+w_m(\epsilon_m-1) >0}$$
where x: exports; m: imports; w: weights; $\epsilon$: price elasticity.
If this condition is satisfied, a depreciation of the domestic currency will decrease a trade deficit.

If the weights of the exports and imports are equal, the Marshall-Lerner condition equation:
$$\mathrm{\epsilon_x+\epsilon_m >1; (w_x=w_m)}$$
This is often cited as the **classical Marshall-Lerner** condition.

In general, the **higher the elasticity of demand for both export goods and import goods**, the **stronger is the effect of exchange rate changes on the trade deficit**.

The high elastic demand of goods are:
- good with close substitutes
- goods that represent high proportion of overall expenditure (e.g. car)
- some luxury goods

The low elastic demand of goods are:
- good that have few or no good  substitutes
- goods that represent small proportion of overall expenditure (e.g. household items)
- necessities

### Elasticities approach and effect after domestic currency adjustment 
Ideally, if the Marshall-Lerner condition is satisfied, we wish to see an immediate effect where the trade deficit narrows once the domestic currency is depreciated.

However, there may be a delay in the effect this is because the quantity of imports and exports have not adjusted **due to order contracts that were placed earlier**.

However, the domestic currency is now weaker. While quantities shipped may not have changed, import expenditures goes up as the weaker domestic currency means more units are required to pay for foreign goods. In the short run, during this delay, the **trade deficit may widen instead of narrowing**. 

Eventually, when changes in order quantities take effect, the Marshall-Lerner conditions take effect and the currency depreciation begins to narrow the trade deficit. This effect is called the **J-curve effect**.

![[Screenshot 2023-05-01 at 20.56.37.png]]


### Absorption approach
The **absorption approach** is a **macroeconomic technique** that **focuses on the effect of exchange rates on capital flows**.

From balance of payment, the equation of GDP:
$$\mathrm{(X-M)=(T-G)+S-I}$$
where (X-M): current account surplus/deficit (balance of trade); (T-G): government savings; S: private savings; I: private investments.

From this relationship, we can see that a trade deficit means the country does not save enough to fund its investment in plant and equipment, the additional amount to fund domestic investment must come from foreigners. So there's a surplus in the capital account to offset the deficit in the trade account.

Therefore, it is equivalent to:

$$\mathrm{Balance\,of\,trade=National\,savings-Private\,investment}$$
and 
$$\mathrm{Balance\,of\,trade=National\,income-Total\,expenditure}$$
where **national income** is the total domestic **production** of goods and services, and **total expenditure** is the total **adsorption** of goods and services.
There's a **trade deficit** when a country **absorbs more than it produces**.

![[Screenshot 2023-05-01 at 21.29.19.png]]

In order to reduce the trade deficit, a depreciation of the domestic currency must **↑ national income relative to expenditure** or **↑ national saving increase relative to domestic investment in physical capital**.

Whether a currency depreciation has these effects depends on the **current level of capacity utilisation** in the economy.

#### Capacity utilisation
##### Less than full employment situation
When an economy is operating at **less than full employment**, the **currency depreciation makes domestic goods and assets relatively more attractive** than foreign goods and assets. This can bring about a **reduction in the trade deficit**.

##### At full employment situation
In a situation where the economy is operating **at full employment**, an **increase in domestic spending will translate to higher domestic prices, which can reverse the relative price changes of the currency depreciation** resulting in a return to the previous deficit in the balance of trade.

**In the short run**: There can be another effect at play, which is the wealth effect, the currency depreciation does result in a decline in the value of domestic assets. Savers may initially want to **spend less and save more to rebuild wealth**. This can **improve the balance of trade initially**.

**In the long run**: as the real wealth of savers increases over time, the positive impact on saving will decrease, eventually returning the economy to its previous state and balance of trade.

---
## Questions before starting this section:
- [ ]