# Crypto Sentiment Pulse-Bitcoin Fear & Greed Analysis

The crypto market behaviour is very emotional. People tend to get greedy when the market is rising people often sell their coins in irrational reaction of seeing red numbers. There are two simple assumptions:First one is,
Extreme fear can be a sign that investors are too worried. That could be a buying opportunity and the second one is,
When Investors are getting too greedy, that means the market is due for a correction.Understanding market psychology is therefore essential for analysts, traders, and decision-makers.

The Bitcoin Fear and Greed Index is a tool used to analyze market sentiment in the cryptocurrency space. It helps identify when the market is experiencing excessive fear, which might indicate undervaluation, or excessive greed, suggesting potential overvaluation.


![Image](https://github.com/user-attachments/assets/daa5f7f9-2c98-464b-b762-9c0b584ea8f3)


## Project Overview

The project is designed to simulate an end-to-end cloud data architecture. Raw Bitcoin Fear & Greed Index data was ingested into Azure Data Lake Storage, processed through an Azure data warehouse layer, and refined into a Data Mart for analytics. The primary goal of the analysis is to understand how fear and greed sentiment values correlate with Bitcoin closing prices and trading volume. Additionally, the project aims to identify patterns such as periods of extreme fear leading to price drops or whether extreme greed aligns with market rallies.Here I am going to Analyze Bitcoin Market Emotions with Data-Driven Insight.

## Data Sources
[bitcoinfearandgreedindex.csv](https://github.com/user-attachments/files/23736622/bitcoinfearandgreedindex.csv)


This Dataset is being collected Two Sources

1.Yahoo Finance
2.Alternative.me

## Content

The dataset used for this project includes:

Date

Fear & Greed Index Value (0–100)

Sentiment Classification (Extreme Fear, Fear, Neutral, Greed, Extreme Greed)

Bitcoin Closing Price

Bitcoin Trading Volume

This dataset presents a unique opportunity for researchers and analysts to explore the relationship between the prices and volumes of Bitcoin, as well as the sentiment of the overall crypto market. By conducting thorough analysis of this dataset, researchers and analysts can gain valuable insights into the behavior and trends of the cryptocurrency market. This includes examining the daily closing prices and volumes of Bitcoin, as well as the Fear and Greed Index values for the overall crypto market. Through comprehensive analysis, potential patterns, trends, and correlations between price movements, trading volumes, and market sentiment can be identified. This data presents a unique opportunity for researchers and analysts to uncover valuable information that can contribute to a deeper understanding of the cryptocurrency market and its potential implications for investment decision-making.

## Tools are being used

#### Microsoft Excel

Used for initial data cleaning, chart creation, and validation

Enabled quick inspection of trends (e.g., sentiment vs. BTC price)

#### Azure Services

- Azure Data Lake Storage Gen2 – to store raw, transformed, and curated data

- Azure Synapse Analytics / Azure SQL Warehouse – ETL, data processing, and queries

- Data Mart – for simplified and optimized analytical consumption

- Power BI for dashboards and visual insights

## Technologies Being Used

The project utilizes modern cloud data engineering technologies and practices:

### Data Engineering Technologies

- Creating Azure Data Lake using data factory for scalable big-data storage

<img width="731" height="39 1" alt="image" src="https://github.com/user-attachments/assets/08194125-07a8-4648-8373-e176085d1a0f" />
Creating storage account

<img width="547" height="476" alt="image" src="https://github.com/user-attachments/assets/1b15f06c-e978-4674-bf1d-8548c1128029" />
creating container

- Creating Data warehouse using data bricks.

<img width="836" height="508" alt="image" src="https://github.com/user-attachments/assets/ad15506b-2aea-4d4a-bba8-879382d65d0f" />
Creating Data bricks

<img width="731" height="423" alt="image" src="https://github.com/user-attachments/assets/d3fdf5f3-5fe0-420c-82ab-f1dc36dbfdaf" />
Creating Data factory

- Azure Synapse SQL / Spark for data transformation

<img width="963" height="428" alt="image" src="https://github.com/user-attachments/assets/9c963ad8-cf7a-4a95-878a-6df42c031ff3" />
SQL queries under synapse analysis


<img width="945" height="414" alt="image" src="https://github.com/user-attachments/assets/7106c990-865a-427c-aa06-5579a4765f89" />
SQL QUeries under Chart view


- ETL pipelines for structured data flow (raw → transformed → curated)

<img width="706" height="388" alt="image" src="https://github.com/user-attachments/assets/fd38e91f-a617-45e4-bfd4-eb397498f57a" />

<img width="901" height="383" alt="image" src="https://github.com/user-attachments/assets/b2d74b0f-7c66-4ed0-bddf-2c5600acf94a" />

### Data Analytics Technologies

- Excel Pivot Tables, Charts & Functions for sentiment exploration

- Sentiment classification logic to map numerical values to categories

- Time-series analysis to compare sentiment with Bitcoin market movement

These technologies collectively enable a robust pipeline from raw data ingestion to final business insights.

## Data Cleaning

The dataset was initially collected in CSV form and later I converted it in Excel and cleaned it and also ingested into Azure Data Lake under the Raw-Data zone. After processing, the cleaned dataset was moved to Transformed-Data and finally into the Data Mart for analytics.

## Exploratory Data Analysis

Using python in Azure Data warehouse-

<img width="842" height="524" alt="image" src="https://github.com/user-attachments/assets/ed6e5776-74a2-4c86-850a-369e0a2c6dd8" />

<img width="851" height="560" alt="image" src="https://github.com/user-attachments/assets/a6861aa8-98c3-41ba-8b1d-f2b084635167" />

<img width="881" height="494" alt="image" src="https://github.com/user-attachments/assets/20b0c1aa-c272-49f4-82dd-7f1b2a296831" />

<img width="872" height="563" alt="image" src="https://github.com/user-attachments/assets/37eb892a-f89b-4983-ac0f-cac91177cc9f" />

<img width="873" height="491" alt="image" src="https://github.com/user-attachments/assets/1892cea6-6187-4e96-9717-34e8d7401f4d" />

<img width="881" height="497" alt="image" src="https://github.com/user-attachments/assets/e4b53cd8-b110-4b44-a2fc-1a6482ff9f07" />

## Power BI Dashboard

### Dashboard 1:Executive Dashboard on bitcoin fear & greed analysis

<img width="953" height="546" alt="image" src="https://github.com/user-attachments/assets/8fdf591c-cb29-4b89-baf2-4e2225e1fecb" />

<img width="952" height="463" alt="image" src="https://github.com/user-attachments/assets/c6c5862c-194e-4f08-8b62-0fd7e3aaa799" />

This chart shows Fear & Greed Index over time with a line chart where it shows on 59 th date the value classification is Extreme Fear.

<img width="963" height="451" alt="image" src="https://github.com/user-attachments/assets/ffc6c0b6-83d8-4213-bc47-f80ccb8c8675" />

This column chart shows Bitcoin closing price over time and its high in 2021.

<img width="966" height="448" alt="image" src="https://github.com/user-attachments/assets/6899b5e5-ba0f-41d9-985b-a13f81aa35cd" />

This Line and stacked column chart shows BTC value vs BTC price.

<img width="952" height="451" alt="image" src="https://github.com/user-attachments/assets/80ecba53-fd74-4be6-90bb-6dd4c03cbb57" />

This Donut chart Shows BTC value classification by count and percentage of value.

<img width="966" height="456" alt="image" src="https://github.com/user-attachments/assets/c7a61f14-9b8f-4416-8242-8e189a438e04" />

This Stacked bar chart shows average BTC price by sentiment when the average closing price goes high then the sentiment is Extreme greed and when goes lowest the sentiment is fear.


### Dashboard 2:Deep anlysis on bitcoin fear & greed index

<img width="968" height="544" alt="image" src="https://github.com/user-attachments/assets/055002b1-2be7-45b0-99b5-fa6f886daf87" />

<img width="958" height="455" alt="image" src="https://github.com/user-attachments/assets/69bf278a-7972-45b4-9552-ab892a59cf38" />

This Scatter chat shows BTC price vs Value.

<img width="965" height="458" alt="image" src="https://github.com/user-attachments/assets/4a61aca7-6948-40c4-ae47-f998a488294f" />

This Matrix chart shows analyze BTC price by value classification and date.

<img width="962" height="446" alt="image" src="https://github.com/user-attachments/assets/76dfa2f1-e042-47eb-b521-d6117a68ca3d" />

This Key influencers analyze-what influences BTC closing to increade or decrease.And when is BTC closing more likely to be low or high.


## Expected Outcomes

The expected outcomes of this project include:

Clear understanding of how sentiment values correlate with Bitcoin price movement

Identification of market behavior during Extreme Fear vs. Extreme Greed periods

Ability to visually track sentiment cycles and how they align with large price swings

Establishment of a complete cloud-based data architecture suitable for scaling

Foundational analytics for future dashboards that compare sentiment across countries or exchanges
## Recomendation

## Limitation What Would Be the “Ah-Ha” Things?

The project’s major discoveries or “ah-ha moments” include:

Strong alignment between sentiment and price

Extreme Fear often corresponds with price dips

Greed phases tend to precede price surges

Volume spikes appear during high fear or high greed periods, showing increased market activity

Sentiment shifts often occur before major price changes, making sentiment a potential leading indicator

The full Azure pipeline illustrates how enterprise systems manage, process, and analyze large datasets efficiently

These insights reveal that sentiment is more than just a numerical scale—it reflects emotional phases that heavily influence market behavior.

## Findings / Analysis

After cleaning and loading the data into the Azure environment, a detailed examination of the sentiment trends and Bitcoin pricing was performed. The analysis showed several notable patterns:

1. Extreme Fear Periods

Dates with sentiment values below 20 (e.g., 2/2/2018, 2/7/2018) often align with sharp declines in Bitcoin prices.

Trading volume increases during fear, suggesting panic selling or uncertainty.

2. Greed & Extreme Greed Periods

Values above 60–70 (e.g., 2/15/2018 onwards) correspond to price recovery and upward movement.

Investors appear more active during greed phases, often chasing rising prices.

3. Neutral Sentiment

Neutral periods show market stabilization, with fewer large swings.

4. Time-Series Trends

The sentiment index acts as a market psychology barometer, giving early hints at trend reversals.

Visual inspection of charts suggests sentiment changes precede price movements by a few days.

5. Data Engineering Validation

Lake → Warehouse → Mart pipeline ensures clean, reliable, and structured data, enabling smooth analytical queries.


## Conclusion

The project demonstrates both the technical architecture of a real-world Azure-based analytics system and the practical usefulness of sentiment data in understanding crypto markets. By integrating data engineering with financial analytics, the project provides valuable insights into Bitcoin’s behavior through the lens of investor psychology. The structured pipeline ensures the system can be extended into more complex analytics such as forecasting, country-by-country sentiment comparison, or real-time dashboards.


## Referances
