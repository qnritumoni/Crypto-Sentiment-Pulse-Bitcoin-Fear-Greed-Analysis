# Crypto Sentiment Pulse-Bitcoin Fear & Greed Analysis

The crypto market behaviour is very emotional. People tend to get greedy when the market is rising people often sell their coins in irrational reaction of seeing red numbers. There are two simple assumptions:First one is,
Extreme fear can be a sign that investors are too worried. That could be a buying opportunity and the second one is,
When Investors are getting too greedy, that means the market is due for a correction.Understanding market psychology is therefore essential for analysts, traders, and decision-makers.

The Bitcoin Fear and Greed Index is a tool used to analyze market sentiment in the cryptocurrency space. It helps identify when the market is experiencing excessive fear, which might indicate undervaluation, or excessive greed, suggesting potential overvaluation.


![Image](https://github.com/user-attachments/assets/ec6d7304-5999-4f4e-b158-fe038653207b)

## Project Overview

The project was designed to simulate an end-to-end cloud data architecture. Raw Bitcoin Fear & Greed Index data was ingested into Azure Data Lake Storage, processed through an Azure data warehouse layer, and refined into a Data Mart for analytics. The primary goal of the analysis is to understand how fear and greed sentiment values correlate with Bitcoin closing prices and trading volume. Additionally, the project aims to identify patterns such as periods of extreme fear leading to price drops or whether extreme greed aligns with market rallies.Here I am going to Analyze Bitcoin Market Emotions with Data-Driven Insight.

## Data Sources
[bitcoinfearandgreedindex.csv](https://github.com/user-attachments/files/23736622/bitcoinfearandgreedindex.csv)


This Dataset is being collected Two Sources

1.Yahoo Finance
2.Alternative.me

## Content

This dataset specifically includes-
1.Date
2.Daily closing prices of Bitcoin, 
3.Daily volumes of Bitcoin, and 
4.The Fear and Greed Index values for the overall crypto market.

This dataset presents a unique opportunity for researchers and analysts to explore the relationship between the prices and volumes of Bitcoin, as well as the sentiment of the overall crypto market. By conducting thorough analysis of this dataset, researchers and analysts can gain valuable insights into the behavior and trends of the cryptocurrency market. This includes examining the daily closing prices and volumes of Bitcoin, as well as the Fear and Greed Index values for the overall crypto market. Through comprehensive analysis, potential patterns, trends, and correlations between price movements, trading volumes, and market sentiment can be identified. These insights can inform investment strategies and decision-making, providing a more nuanced understanding of the dynamics of the cryptocurrency market. This data presents a unique opportunity for researchers and analysts to uncover valuable information that can contribute to a deeper understanding of the cryptocurrency market and its potential implications for investment decision-making.

## Tools are being used

Microsoft Excel

Used for initial data exploration, cleaning, chart creation, and validation

Enabled quick inspection of trends (e.g., sentiment vs. BTC price)

Azure Services

Azure Data Lake Storage Gen2 – to store raw, transformed, and curated data

Azure Synapse Analytics / Azure SQL Warehouse – ETL, data processing, and queries

Data Mart – for simplified and optimized analytical consumption

 Power BI for dashboards and visual insights

## Technologies Being Used

The project utilizes modern cloud data engineering technologies and practices:

## Data Engineering Technologies

Azure Data Lake for scalable big-data storage

<img width="731" height="391" alt="image" src="https://github.com/user-attachments/assets/08194125-07a8-4648-8373-e176085d1a0f" />


<img width="547" height="476" alt="image" src="https://github.com/user-attachments/assets/1b15f06c-e978-4674-bf1d-8548c1128029" />

Parquet/CSV formats for optimized storage/analytics

Azure Synapse SQL / Spark for data transformation

<img width="963" height="428" alt="image" src="https://github.com/user-attachments/assets/9c963ad8-cf7a-4a95-878a-6df42c031ff3" />
SQL queries under synapse analysis


<img width="945" height="414" alt="image" src="https://github.com/user-attachments/assets/7106c990-865a-427c-aa06-5579a4765f89" />
SQL QUeries under Chart view
ETL pipelines for structured data flow (raw → transformed → curated)

Data Analytics Technologies

Excel Pivot Tables, Charts & Functions for sentiment exploration

Sentiment classification logic to map numerical values to categories

Time-series analysis to compare sentiment with Bitcoin market movement

These technologies collectively enable a robust pipeline from raw data ingestion to final business insights.

## Data Cleaning

The dataset was initially collected in CSV form and later I converted it in Excel and cleaned it and also ingested into Azure Data Lake under the Raw-Data zone. After processing, the cleaned dataset was moved to Transformed-Data and finally into the Data Mart for analytics.

## Exploratory Data Analysis

Using python

<img width="842" height="524" alt="image" src="https://github.com/user-attachments/assets/ed6e5776-74a2-4c86-850a-369e0a2c6dd8" />

<img width="851" height="560" alt="image" src="https://github.com/user-attachments/assets/a6861aa8-98c3-41ba-8b1d-f2b084635167" />

<img width="881" height="494" alt="image" src="https://github.com/user-attachments/assets/20b0c1aa-c272-49f4-82dd-7f1b2a296831" />

<img width="872" height="563" alt="image" src="https://github.com/user-attachments/assets/37eb892a-f89b-4983-ac0f-cac91177cc9f" />

<img width="873" height="491" alt="image" src="https://github.com/user-attachments/assets/1892cea6-6187-4e96-9717-34e8d7401f4d" />

<img width="881" height="497" alt="image" src="https://github.com/user-attachments/assets/e4b53cd8-b110-4b44-a2fc-1a6482ff9f07" />

## Data Analysis


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
