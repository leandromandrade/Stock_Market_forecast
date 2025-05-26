<h1>Financial Forecasting Using Sentiment Analysis & Deep Learning</h1>
This project presents a full big data pipeline combining stock market data and social media sentiment to forecast stock prices using machine learning and deep learning models.

<h2>Tools & Technologies</h2>
Apache Spark (PySpark) for distributed data processing
MongoDB & MySQL for NoSQL and SQL data storage
HDFS for distributed file storage
Python (Pandas, TextBlob, Matplotlib) for data manipulation, sentiment analysis, and visualization
PyTorch for training LSTM and MLP models
ARIMAX as a traditional time series baseline

<h2>End-to-End Pipeline</h2>
Data Sources
Stock market prices from five companies (Tesla, Disney, Amazon, Apple, British Airways)
Twitter sentiment data related to the companies

<h2>Storage Strategy</h2>
Stock and tweet data stored in both MongoDB and MySQL
Benchmarking via YCSB revealed MongoDB as faster in all workloads (A/B/C)

<h2>Real-Time Streaming Component</h2>
Spark Streaming was used to collect and analyze Reddit comments in real-time.
Filtered for specific topics (e.g., “Trump”), stored results in HDFS, and applied TextBlob for sentiment analysis.
Output visualized using bar charts.
