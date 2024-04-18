# Project-Three

Data Engineering: While we know that S&P 500 is the most famous financial benchmark in the world, we wanted to look closer at the data how ESG for these companies. We found two different datasets on Kaggle, SP500 Stocks and Public Company ESG Ratings dataset. Before we could merge the datasets, we had to change the date format to be consistent, change the name from "symbol" to "ticker", and lastly, we converted the lowercased tickers to uppercase. We, then, were able to outerjoin the two by "ticker/date".

We used Seaborn as our additional library to help us with statistical graphics.
We imported the CSV files into Python using Pandas.

### ETL: 
After merging the two, in MongoDB, we created the new collection. 

### Import the dataset with:      
      "mongoimport --type csv -d SP500 -c SP500_ESG --headerline --drop sp500_esg_ceo_info-filtered.csv"      
      "mongoimport --type csv -d SP500 -c date --headerline --drop datefiltered_data.csv"      

### Ethics and Data: 
Ethical considerations in data analysis includes questioning sources, algorithmic bias, and method of collection amongst others. The data we analyzed seeks to provide a new method of analysis in the valuation of stocks. This data takes in to consideration aspects of a companies performance that is not typically included, such as their efforts to remediate environmental damage, representation and diverisification in their governance, and their efforts to positively impact the communities the businesses work in and serve. This data seeks to provide an ethical framework to investing that did not exist prior to its uprising. To this end, the data collected and merged provides, at worst, and ethically neutral ground to analyze a stocks value, and at its best provides an ethical framework while considering a stocks value.

### Data sources:
https://www.kaggle.com/datasets/alistairking/public-company-esg-ratings-dataset
https://www.kaggle.com/datasets/andrewmvd/sp-500-stocks

