# 55 - Fintech in investment management
202305051826
Status: #📥 
Tags: [[CFA Level I]]

## Objectives:
- [ ] describe “fintech”
- [ ] describe Big Data, artificial intelligence, and machine learning.
- [ ] describe fintech applications to investment management.
- [ ] describe financial applications of distributed ledger technology.
---
## Big data and artificial intelligence
### Introduction
**FinTech** broadly refers to **technology-driven innovation that is applied to the financial services industry**. Companies that are in the business of developing such technologies are referred to as fintech companies.

Some of the primary areas where fintech is developing:
- **Handling extremely large data sets** - assist in making investment decisions (e.g. security prices, financial statements, economic indicators and social media posts)
- **Analytic tools** - e.g. A.I. for analysing and making sense of a very large data sets
- **Automated trading** - investment decisions are made and executed through computer algorithms
- **Automated advice** - where robo-advisors provide investment advice and portfolio management services to retail investors
- **Financial recordkeeping** - based on distributed ledger technologies like block chain that reduces the need for intermediaries in order for individuals and firms to transact with each other.

### Big data
**"Big-data"** is a widely used expression that refers to all the potentially useful information that's generated in the economy.

This includes data from:
- **Traditional sources** - e.g. financial markets, company financial reports and economic data.
- **Alternative data from non-traditional sources**
	- **Individuals** - who generate usable data such as social media post online reviews, emails and web searches.
	- **Business processes** - generate potentially useful information, such as credit card transactions, direct sales information and **corporate exhaust** (corporate exhaust refers to the trail of data left by business activities and transactions; e.g. supply chain information, banking transactions and point of sales data)
	- **Sensors** - e.g. smartphones, cameras and RFID chips, which are increasingly being extended into a broad network known as the **Internet of Things** (Internet of Things is formed by a vast array of smart devices like home appliances, smart buildings and vehicles that are embedded with sensors and network technologies that allow them to interact and share information)

Characteristics of big data include:
- **Volume** - continues to grow by orders of magnitude, the units in which data can be measured have increased from MG, GB to TB and even petabytes (PB; i.e. 1 quadrillion bytes).
- **Velocity** - refers to how quickly data are communicated, increasingly, data such as stock market price feeds can be presented in close to real time. Such data feeds are said to have low latency.
- **Variety** - varying degrees of structure in which data may exist. These range from **structured forms** (e.g. spreadsheets and databases) to **semi-structured forms** (e.g. photos and web page code) to **unstructured forms** (e.g. video, social media posts and voice recordings).

### Data science
**Data science** concerns how we extract such useful information from big data data science describes methods for **processing** and **visualising** the data.

#### Processing data
Processing methods include:
- **Capture** - to collect data from various sources and transform them into usable forms.
- **Curation** - to ensure data quality by adjusting for bad or missing data.
- **Storage** - refers to the database design and how the data can be accessed.
- **Search** - how to query data. This is not a trivial task, as a large quantity of data requires complex and efficient search engines to quickly retrieve large chunks of data.
- **Transfer** - moving data from their source to where they're needed (could be through a direct data feed, such as a stock exchanges price feed)

Even after processing, the amount of data can be overwhelming and it's difficult to observe trends and patterns, and thus visualisation is important.

#### Visualising data
**Visualisation techniques** can help the data scientist **pick up and follow patterns more easily**.

There are several methods for visualisation:
- **Charts and graphs** - most suitable for traditional data, which are well-structured.
- **Interactive 3D visualisation tools** - allow the data scientist to rotate the data across 3 axes to help identify more complicated trends.
- **Word cloud** - displays frequently occurring words found in the data where the larger the text, the higher is its frequency to learn the predominant sentiment of market participants.
- **Mind map** - a variation of the word cloud, rather than displaying the frequency of the word, a mind map shows how different concepts are related to each other.

#### Challenges of using data science
Using data science to take advantage of big data presents a number of challenges:
- **Ensure high quality data** - accounting for the possibilities of outliers, bad or missing data or sampling biases
- **Ensure sufficient and appropriate data**

Besides, data science tends to be more suitable for traditional structure data, which can be plotted onto graphs. Qualitative and unstructured data are particularly difficult to process and organise using data science methods.

Information and conclusions depends much on the quality and skills of the data scientist:
- Extracting relevant data
- Observing trends and anomalies
- Translating them into useful information.

### A.I. and machine learning
**Artificial intelligence** is a field that seeks to replace humans **using computer systems that are programmed to simulate human cognition**.

**Neural networks** technologies have developed over the years and progressed into machine learning. Like humans, the cognitive skills of machine learning algorithms improve over time on their own as they're being used.

Machine learning algorithms typically have to go through a learning phase where it's given inputs of source training data and may be given outputs of target training data. The algorithm is designed to learn how to model the output data based on the input data or to learn how to detect and recognize patterns in the input data. The machine learning process typically requires vast amounts of data.

There are two types of machine learning:
- **Supervised learning**
- **Unsupervised learning**

#### Supervised learning
In **supervised learning**, the **inputs** and **output data** are **labeled** to allow the algorithm to learn how to map inputs to their **desired output**. The trained algorithms are then given new data to predict outcomes or recognise patterns. 

e.g. a stock prediction machine can be trained using past data like price history, company fundamentals and economic data as inputs and the past returns of various stocks as output training data. The trained model can then be used to predict future stock returns using the latest data.

#### Unsupervised learning
In **unsupervised learning**, the input data are not labeled, rather, the machine learns to describe the structure of the data.

e.g. the characteristics of various companies can be fed in as inputs, and the algorithm then tries to **group the companies into peer groups based on certain similarities** other than the standard sector or country groupings.

### Challenges in machine learning
Machine learning have challenges in terms of the way of learning:
- **Overfitting** - learns the input and output data too exactly, treat noise as true parameters, and identifies false or unsubstantiated patterns and relationships.
- **Underfitting** - fails to identify actual patterns and relationships, treating true parameters as noise, model is not complex enough to describe the data.
- **Black box** - A further challenged with machine learning is that its results can be a black box producing outcomes based on relationships that are not readily explainable.

### Deep learning
**Deep learning** uses layers of neural networks to identify patterns, beginning with simple patterns and advancing to more complex ones.

Deep learning may employ **supervised** or **unsupervised learning**, some of the applications of deep learning include image and speech recognition.

## Application of fintech to investment management
### Text analytics/NLP
**Text analytics** refers to the use of computers to analyze unstructured data in text or voice forms, such as:
- Company filings and financial reports
- Social media posts
- Email
- Quarterly earnings calls

This is done to aid in some decision making process. Analysing the frequency of words and phrases in the finance industry, to estimate indicators like consumer sentiment. (e.g. performing text analytics on recent Twitter feeds can help and identify shifts in consumer sentiment by monitoring the frequency of certain related key words or phrases.)

**Natural language processing** goes beyond just counting word frequency as it seeks to interpret and make sense of the data using artificial intelligence.

Speech recognition and language translation are among the uses of natural language processing.

e.g. **compliance monitoring** - check for regulatory compliance by monitoring the emails and phone conversations from employees. An employee compliance report can be generated and appropriate actions taken if there is any compliance breach.

e.g2. **Evaluate large volumes of research reports to detect more subtle changes in sentiment based on the language** used by the analyst, just beyond quantitative figures like EPS. If the tone of the majority of analysts report are found to be increasingly bearish, management may choose to take defensive actions to protect asset values.

The advantage of NLP is that it can process large amounts of data at a fraction of the time that humans would need to manually go through all the data.

### Risk analysis
Under **risk management**, financial regulators require firms to perform **risk assessments** and **stress testing**.

The simulations/scenario analysis and other techniques used for risk analysis require large amounts of **quantitative data**, along with a great deal of **qualitative information**.

Machine learning and other techniques related to big data **can be useful in modelling and testing risk quickly and comprehensively**.

Another advantage of using machine learning for risk analysis is that firms can use **real time data to monitor risk exposures**. This allows firm management to employ risk mitigation measures and hedging practices sooner to help preserve asset values.

### Algorithmic trading
**Algorithmic trading** refers to automated securities trading **based on a predetermined set of rules**.

e.g. algorithms may be designed to enter optimal execution instructions, continuously revising execution strategy for any given trade **based on real time price and volume data**.

e.g2. high frequency trading (HFT) that **identifies and takes advantage of intraday securities mispricing**, such trades are executed on ultra high speed networks in fractions of a second.

e.g3. useful for executing large orders by determining the best way to divide the orders across exchanges

### Robo-advisors
**Robo-advisors** are **online platforms that provide automated investment advice to retail investors**. 

The client usually begins by answering some survey questions to understand client's:
- financial position
- return objectives
- risk tolerance
- constraints such as time horizon
- liquidity needs.

Based on these factors, an optimal portfolio allocation is computed for the client. Such services may be fully automated or assisted by human investment adviser.

Robo-advisory services tend to:
- Offer passively managed investments
- Low fees
- Low minimum account sizes
- Conservative recommendations

which may make investment advice more accessible to a larger number of investors.

One disadvantage of robo-advisers is that the reasoning behind their recommendations might not be apparent, without a human investment adviser to explain the reasoning, customers may hesitate to trust the appropriateness of a robo advisors recommendations, particularly in crisis periods.

As robo-advisers are still relatively new to the market, regulation is still emerging.

However, in many countries, robo advisory services are subject to the same regulations and registration requirements as any other investment adviser.

## Distributed ledger technology (blockchain)
### Distributed ledger technology
**Traditional ledgers** work through recording transactions with a bank, either deposits, withdrawals or paying a third party in the bank's ledger. This is a centralised ledger in which the bank is the central authority over the ledger, where it lack transparency and is one single point of vulnerability where hackers can attack.

In contrast, a **distributed ledger** is a **database that is shared on a network so that each participant has an identical copy**. To maintain the identicalness of all copies of a distributed ledger must have **a consensus mechanism to validate new entries into the ledger**.

**Creation of new record is**:
- Immutable
- Transparent
- Accessible to all participants
- Near real time basis

Distributed ledger technology uses cryptography to ensure only authorized network participants can access the data.

### Blockchain
A **blockchain** is a distributed ledger that **records transactions sequentially into blocks** and **links these blocks in a chain**, **each block has a cryptographically secured hash that links it to the previous block**.

In order to add a new block to the chain, the consensus mechanism requires some of the computers on the network known as miners to solve a cryptographic problem.

The solution has to be verified by all the other participants in the network. If the majority of the nodes verify that the solution is correct, the new block is added to the block chain and all copies of a distributed ledger are updated.

Mining requires vast resources of **computing power** and **electricity**. This imposes substantial costs on any attempt to manipulate a blockchain's historical record.

In order for a hacker to make a fraudulent transaction on the block chain, he would need to gain control of a majority of the nodes to gain consensus. For this reason, the more participants there are in the network, the more secure it is as it gets harder for a hacker to gain majority control.

Distributed ledgers or blockchains can take the form of **permission** or **permissionless networks**.

#### Permission network
In **permissions networks**, users have different levels of access.

e.g., a permission network might allow network participants to add new transactions (level 1) while giving government regulators permission to view all the transaction history (level 2).

##### Permissionsless networks
**Permissionsless networks**, all network participants, not just the regulators, can view all transactions.

These networks have no central authority, which gives them the advantage of having no single point of failure, the ledger becomes a permanent record visible to all, and its history cannot be altered. This removes the need for trust between the parties to a transaction.

### Application
There are several application of blockchain currently in use:
- **Cryptocurrency**
- **Post-trade clearing/settlement**
- **Smart contract**
- **Tokenisation**

#### Cryptocurrencies
Most crypto currencies, notably Bitcoin, are based on permissionless networks,  a cryptocurrency is a digital currency that allows participants to engage in real time transactions without a financial intermediary.

Many crypto currencies like Bitcoin have a self-imposed limit on the total amount of currency that can be mined, thus preserving their values versus fiat currency, which can be printed without limits.

However, cryptocurrency still suffer from low adoption rates and do not have backing from most governments.

Besides its applications as an alternative to traditional currencies, some startup companies issue their own cryptocurrency to investors to raise capital as an alternative to issuing equity. Rather than an IPO, such offerings are known as initial coin offerings (ICO).

ICO reduce the cost and time required to raise capital compared to carrying out a regulated IPO, however, ICO typically do not come with voting rights.  ICOs can be traded amongst investors.

Investors should note that fraud has occurred with ICOs and several regulators have already banned companies from issuing ICOs.

#### Post-trade clearing/settlement
Another possible application of **distributed ledgers** is in the area of **post-trade clearing/settlement** in the stock market.

Currently, it takes at least one business day for trades to be cleared/settled, this is because there are intermediaries to verify the trade with before clearance distributed.

Ledger technology has the potential to eliminate the need for intermediaries, bring about real time trade verification and settlement, possibly **reducing trading costs** and **counterparty risk**.

#### Smart contract
**Smart contracts** are **electronic contracts** that could be **programmed to self execute based on terms agreed to by the counter parties**.

#### Tokenisation
Tokenisation refers to **electronic proof of ownership of physical assets**, which could be maintained on a distributed ledger.

e.g. potentially replace the paper real estate deeds currently filed at government offices.

---
## Questions before starting this section:
- [ ]