# 34 - Security market index
202305012151
Status: #📥 
Tags: [[CFA Level I]]

## Objectives:
- [ ] describe a security market index.
- [ ] calculate and interpret the value, price return, and total return of an index.
- [ ] describe the choices and issues in index construction and management.
- [ ] compare the different weighting methods used in index construction.
- [ ] calculate and analyze the value and return of an index given its weighting method.
- [ ] describe rebalancing and reconstitution of an index.
- [ ] describe uses of security market indexes.
- [ ] describe types of equity indexes.
- [ ] describe types of fixed-income indexes.
- [ ] describe indexes representing alternative investments.
- [ ] compare types of security market indexes.

---
## Index definition and calculation of value and returns

A **security market index** is used to represent the performance of:
- **asset class** - e.g. HFRX Global Hedge Fund index represent performance of global hedge funds
- **security market** - e.g. Dow Jones Industrial Average represents US stock market
- **segment of a market** - e.g. Dow Jones Transportation Index represent transport sector of US stock market

Indices usually created by **selecting a number of representatives securities** in the market it seeks to represent. These elected securities are known as the **constituent securities** of the index. The market prices of the constituent securities are used to compute the numerical value of the index at that particular instance.

**Index return** is the % change in the index value over a period of time.

### Price index
**Price index** considers only the prices of the constituent securities are used in the calculation. **Price return** is the % change in the price index value over a period of time.

### Return index
**Return index** takes into account the interim cash flows, such as dividends or interest payments issued by the securities. The index return is known as **total return**.

### Multiple period
If there are multiple periods, the **aggregate return** for the entire period can be calculated by compounding the returns for each period. **Simply multiply the return factors**, for negative returns, the return factor should be less than one.

The equation of **multiple period aggregate return**:

$$\mathrm{Aggregate\,return=Multiply\,all\,return\,factors; (1-Return\,factor)\,if\,negative}$$ 


![[Screenshot 2023-05-02 at 00.03.49.png]]

## Index construction and management
There are 5 considerations in order to construct an index:
- Target market
- Security selection
- Weights
- Rebalancing
- Reconstitution

### Target market
The index provider needs to determine and intended to measure the **target market**.
It may be defined:
- **Broadly** vs **narrowly** (e.g. United States vs. small cap value stocks in US)
- **Asset class** (e.g. fixed income market)
- **Geography** (e.g. China market, emerging markets)
- **Economic sector** (e.g. cyclical stocks)
- **Company size** (e.g. large cap stocks)
- **Duration** (e.g. money market securities)
- **Credit quality** (e.g. high yield bond)

### Security selection
After identifying the target market, the index provider has to select securities from the target market as the **constituent securities** of the index, while it's possible to include all the securities in the market, it often makes more economic sense to select just a **representative sample**.

The S&P 500 and FTSE 100 are examples of indexes with a fixed number of constituents.
The selection process may be determined by:
- **Objective rule** (e.g. the number of shares outstanding, the number of shareholders and market capitalisation)
- **Subjectively by a committee**

### Weights
Once all the constituent securities have been selected, the index provider needs to determine the **weighting scheme**.

Weighting schemes for stock indexes include:
- **Price weighting** - arithmetic average of the prices of the securities included in the index
- **Market capitalisation weighting** - weights based on the market cap of each stock
- **Equal weighting** - arithmetic average **return** of the index stocks 
- **Fundamental weighting** - weights based on firm fundamentals

#### Price weighting
A **price weighted index** is the **arithmetic average of the prices of the securities** included in the index. (e.g. DIJA)

**Advantage of using price weighting**:
- Simple computation

**Disadvantage of using price weighting**:
- Stock splits, stock dividends and stock repurchases shift weight distribution of entire index
- Price of a stock has no bearing of how large a company actually is

**Replicate the price weighting returns**:
- maintain an equal number of shares in each of the constituent stocks
- the portfolio will have identical returns to the index, not considering dividends received and fees and commissions paid.

Note, however, that **certain market actions like stock splits can affect the price** of a stock.

##### Adjustment for stock split for price weighted index
For example, if ABC stock has a 2-for-1 split, the price for each share will be adjusted. Most index providers will adjust the denominator of the index such that the index value is unaffected by such changes. We want to maintain the index value points as before the split, so solving for the denominator. So from this point on, the index show use 2.8 as the denominator until another stock split occurs.

The price index value equation is as follows:
$$\mathrm{Index\,value=\frac{\sum prices}{Num\,of\,stocks}}$$
and the **number of stocks** are **adjusted for splits**.

![[Screenshot 2023-05-02 at 00.48.39.png]]

#### Market capitalisation weighting
A market cap weighted index has weights **based on the market cap** of each stock as a proportion of the total market cap of all the stocks in the index. (e.g. S&P 500)

The index is calculated by something, the market cap of all the stocks in the index and dividing by a similar sum calculated during the selected based period.

The market cap index value equation:
$$\mathrm{Index\,value=\frac{Total\,market\,cap}{Base\,year\,\,market\,cap}\times Base\,year\,index}$$
where market capitalisation is the number of stocks $\times$ price; base year index is normally 100.

**Advantage of using market cap weighting**:
- No adjustments for stock splits/stock dividends
- More closely represents changes in market wealth

**Disadvantage of using market cap weighting**:
- Relative impact of a stock's return on the index increases as its price rises or decreases as its price falls
- Maybe an overvalued stock given a high weight
	- This is similar to following a **momentum strategy** under which the most successful stocks are given the greatest weights and poor performing stocks are underweighted.
- Not all the outstanding shares are available to market investors

**Replicate the returns of market cap weighting** :
- match the value of each security position to its **market-cap weight** in the index

##### Float-adjusted market cap weighting
Typically, firms market float is the number of the shares that are actually available to the investing public and excludes the shares held by controlling stock holders because they are unlikely to sell their shares, shares held by large corporations or governments are often excluded as well.
$$\mathrm{Float=Num\,of\,shares\,outstanding-Stocks\,by\,controlling\,stockholders\,-Shares\,by\,large\,corp\,or\,govt}$$
Some indexes are designed to represent the investment opportunities of global investors, so they also exclude shares that are not available to foreign investors.

If we multiply the number of floating shares by the market price, we get the market float for each stock, we can observe that the weight distribution of unadjusted float has shifted after adjusting for market float.
Therefore, note, unadjusted market float market cap $\ne$ float adjusted market cap.

The reason for **float adjustment** is to **better match the index weights to the market value actually available to market investors**.

![[Screenshot 2023-05-02 at 01.02.38.png]]

#### Equal weighting 
An **equal weighted index** is calculated as the **arithmetic average return** of the index stocks .Index performance is calculated based on the relative price changes for each stock. (e.g. value line composite)

Equal weighting index value is simple if these are the prices of the stocks on the base period where the index value is 100, calculate the **holding period return** for each of the stocks and **the arithmetic average of the returns** is the return of the index for this period.

The equal weighting equation is as follows:
$$\mathrm{Index\,value=(\frac{\sum\,Stock\,returns}{Num\,of\,stocks}+1)\times Base\,year\,index}$$
where returns is calculated by new price/old price - 1.

Increase the index value by this amount and you get the current index value, which is 132 points.

>An equal-weighted index represents 3 stocks as shown. What is the index value today?
>Stock A returns = (77-56)/56 = 0.375  
>Stock B returns = (121-133)/133 = -0.09  
>Stock C returns = (34-20)/20 = 0.7
>Index value = (sum of returns/num of stocks + 1) x base year index  
>= ((0.375-0.09+0.7)/3 + 1) x 100 = 132.83

**Advantage of using equal weighting**:
- Simple computation
- All stocks have equal weight in the index, so higher priced stocks do not have a higher impact on the performance.

**Disadvantage of using equal weighting**:
- Portfolio managers need to adjust the portfolio periodically so that the values of all security positions are made equal
- Weights can be disproportional to size of firm

**Replicate the equal weighting returns**:
- Invest **equal dollar amounts** in each index stock

![[Screenshot 2023-05-02 at 01.07.13.png]]

#### Fundamental weighting
Fundamental weighting uses weights based on **firm fundamentals** such as earnings, dividends or cash flow. The weights can be based on a **single measure or some combination** of these measures.

For example, if this index is weighted by the earnings of the firm as a proportion of the total earnings of all the constituent stocks, the weights assigned to each stock will be as follows.
in contrast to the market cap index weights, these weights are unaffected by the share prices of the index stocks.

**Advantage of using fundamental weighting**:
- No bias towards the performance of overvalued firms
- A fundamental weighted index will actually have a value tilt, overweighting firms with high value metrics such as its earnings and dividends.

**Replicate the fundamental weighting returns**:
- match the value of each security position to its weight in the index

![[Screenshot 2023-05-02 at 01.13.16.png]]
![[Screenshot 2023-05-02 at 01.13.39.png]]

### Rebalancing
**Rebalancing** is the process of **adjusting the weights of securities in a portfolio** to their **target weights** after **price changes have affected the weights**.

The weights in price and market cap weighted indexes are adjusted to their correct values by changes in prices, so rebalancing is not an issue for them (e.g. DJIA, S&P 500).

It's mainly an issue for **equal weighted portfolios** and **fundamental weighted indexes** may also need periodic rebalancing.

Note the **portfolio rebalancing creates high transaction costs on buying and selling** the shares as this **decreases portfolio returns**, some **portfolio managers may choose not to rebalance so frequently at a cost** of not being able to track the equal weighted index so closely.

### Reconstitution
**Index reconstitution** is the process of **adding and deleting constituent securities** that make up the index.

**Deleted** from the index due to:
- bankruptcy
- delisting
- no longer meet the criteria of the index
and **replaced** by securities that meet the index criteria.

#### Trading strategy?
When a **security is added to an index, its price tends to rise** as portfolio managers seeking to track that index in a portfolio by the security, the **prices of deleted securities tend to fall as portfolio managers sell them**.

Note that reconstitution also requires that the weights on the returns of other index stocks be adjusted to conform to the desired weighting scheme.

## Uses of market indices
There are 5 uses of market indices:
- **Gauge of investor confidence or market sentiment** - whether to overweight or underweight a market, broad market index might be more indicative of general sentiment
- **Measure of risk and return of asset class** - use the historical data to estimate the expected return and standard deviation of returns ⇒ portfolio distribution
- **Measure of beta and risk-adjusted return** - CAPM: $\mathrm{ E(R) = R_f +\beta(R_m-R_f)}$ to understand whether to include a certain stock in the portfolio to compare expected and actual return to understand the systematic risk
- **Benchmark manager's performance** - should depend on the portfolio manager's investment approach/style and  market to choose the benchmark to evaluate performance
- **Model portfolio for index funds/ETFs** - replicate performance of the index

## Types of equity indices
There are 4 main categories of equity indices:
- **Broad market index** - represents an entire equity market, includes >90% of stocks in the market (e.g. Wilshire 5000 index, as it contains > 6000 US stocks; good representation of US market performance)
- **Multi-market index** - comprise indices from different countries, based on geographical region, economic development, or world index (world index is important for investors on global approach to equity investments); the stocks in each country are weighted by **market cap**, then the multi-market is weighted by **fundamentals** (e.g. GDP)
- **Sector index** - represents a certain economic sector (e.g. consumer goods, energy, finance, healthcare, technology) in national, regional or global basis, since most sectors are cyclical, investors might want to overweight or underweight exposure based on economic cycle
- **Style index** - categorised according to market cap value or growth or a combination to suit the investment style
	- **Market cap indices** can be differentiated along the lines of small cap, mid-cap and large cap stocks. Classification can be based on absolute market or relative market capitalisation.
	- Value stocks and growth stocks can be differentiated based on their **price to earnings ratios** (P/E) or **dividend yields** (div/price). There's no universal definition regarding the classifications, indices use different criteria based on their own interpretations. So it may not be uncommon to find the same stock in indices of different styles. Secondly, as **valuation ratios and market cap** are the companies change over time, stocks frequently **migrate from one style index category to another on reconstitution dates**.
	- Market cap >$50bn -> large cap; Dividend yield >3% -> value

![[Screenshot 2023-05-02 at 12.20.23.png]]

## Types of fixed income indices
Fixed income securities vary widely with respect to the following dimensions:
- **Geographical location of the issuer**
- **Type of issuer** - a government, government agency, corporate (e.g. business sector of energy, finance, health care or technology etc.) or a structured finance (e.g. asset backed securities (ABS) and collateral debt obligations)
- **Credit quality of the security**, classified as investment grade or not-investment grade securities
- **Time to maturity** - range from a few days to 30 years or beyond.
- **Coupon structure and coupon rates** - zero coupon, fixed coupon and floating rate notes
- **Embedded options** such as convertibility to common stock, callable, putable options.

**Aggregate or broad market indices** are designed to **represent the broad market of fixed income securities** of a geographic region.
e.g. The **Bloomberg Barclays US Aggregate Bond Index (the Agg)** is an example of a single country aggregate index, it **comprises more than 9200 U.S. based securities**, including US Treasury, government related corporate bonds under various business sectors and various types of **asset backed securities**. [Funds and ETF](https://www.investopedia.com/terms/l/lehmanaggregatebondindex.asp) that track the Agg.

![[Screenshot 2023-05-02 at 12.22.52.png]]

There are many dimensions for an index provider to construct an index. Most fixed income indices, however, have a **narrower focus**.

They can subdivide the universe of fixed income securities based on the **market sector**, the government, government, agency, corporate or securities bonds, and the business sector for corporate bonds. 

The **style** which can be distinguished by a bonds, credit quality and or maturity. A common distinction reflected in indices is between an investment grade. That is, those with a S&P credit rating of BBB or better and non investment grade securities also known as high yield securities.

Less commonly, some indices may also choose to distinguish themselves based on **other characteristics** like coupon structures and embedded options to create more narrowly defined indices.

![[Screenshot 2023-05-02 at 12.32.19.png]]

For example, the **Markit iBoxx EUR High Yield Indices** that tracks only euro denominated
corporate bonds which are non investment grade; it is a market-value-weighted index. It does not track bonds that have maturity greater than 10 years or zero coupon bonds. Convertible and portable bonds are also excluded.

### Issues in constructing fixed-income index 
There are several issues in constructive fixed-income index:
- **Very wide universe of securities** ⇒ security selection may not be easy
- **Bonds mature and must be replaced** ⇒ turnover is high
- **Prices of illiquid securities may have to be estimated** from prices of similar securities 
- **Challenges in replicating a fixed-income index** ⇒ illiquidity ⇒ high trading cost; and high turnover of constituent securities ⇒ difficult and expensive to replicate

## Alternative investment indices
**Alternative assets** are of interest to investors because of their potential diversification benefits.

**Alternative investments** include:
- Hedge funds
- Private equity funds
- Real estate
- Commodities
- Infrastructure
- Other rare items like fine wine and antiques.

### Commodities
**Commodity indices** represent **futures** contracts on commodities such as agriculture, metals and energy. 
**Commodity futures returns** include: 
- Roll yield - the yield capture when the futures price converge to the spot price
- Collateral yield
- $\Delta$ Spot price
  
Furthermore, the contracts mature and must be replaced over time by other contracts, for these reasons, therefore, the returns on commodities index $\ne$ returns based on spot prices.

Weighting methods of commodities indices:
- **Equal weighting**  - e.g. CRB Index (The Commodity Research Bureau Index)
- **Global production value** - e,g, S&P GSCI, combination of liquidity measures and global production values in its weighting scheme
- **Fixed weighting** - index provider determines as a result of the different weighting methods used.

Difference indices have significantly different commodity exposure and risk and return characteristics.

### Real estate indices
**Real estate** can be invested:
- **Direct investments** -  in physical, commercial and residential properties
- **Indirect investments** - securities such as real estate investment trusts or REITs.
REITs invest in properties or mortgages and then issue ownership interests in the pool of assets to investors, reach shares, trade like any common shares in the stock market, and many offer very good liquidity to investors.

For physical properties, real estate indices can be constructed using the returns based on appraisals of properties or repeat property sales.

For REITs, there are numerous rete indices that represent publicly traded Rete shares because rates are continuously traded in the market rates indices are updated much more frequently than appraisal and repeat sales indices.

Footsie International produces a family of rete indices that seeks to represent trends in real estate

![[Screenshot 2023-05-02 at 12.47.40.png]]

### Hedge fund indices
**Hedge funds indices**, hedge fund indices reflect the returns on hedge funds, which are private investment vehicles that manage portfolios of securities and derivative positions using strategies like leverage and long and short positions.

Most **hedge fund indices** equally wait in the returns of the hedge funds included in the index, hedge funds are largely unregulated and are not required to report their performance to index providers.

Consequently, some funds will report to one index, but not another, the **performance of different indices can thus vary substantially**.

Furthermore, it's often the case that those funds that report are the funds that have good performance, poorly performing funds do not want to publicise their performance.

The result is an **upward bias** in index returns, with hedge funds appearing to be better investments than they actually are.

## Comparing types of security market indices

![[Screenshot 2023-05-02 at 13.35.42.png]]
![[Screenshot 2023-05-02 at 13.35.58.png]]



---
## Questions before starting this section:
- [ ]