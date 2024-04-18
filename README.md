# Project-Three

Data Engineering: While we know that S&P 500 is the most famous financial benchmark in the world, we wanted to look closer at the data how ESG for these companies. We found two different datasets on Kaggle, SP500 Stocks and Public Company ESG Ratings dataset. Before we could merge the datasets, we had to change the date format to be consistent, change the name from "symbol" to "ticker", and lastly, we converted the lowercased tickers to uppercase. We, then, were able to outerjoin the two by "ticker/date".

We used Seaborn as our additional library to help us with statistical graphics.
We imported the CSV files into Python using Pandas.

ETL: 
After merging the two, in MongoDB, we created the new collection. 

Data sources:
https://www.kaggle.com/datasets/alistairking/public-company-esg-ratings-dataset
https://www.kaggle.com/datasets/andrewmvd/sp-500-stocks

