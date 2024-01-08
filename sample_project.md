<img src="images/worldbank_logo.png?raw=true"/>

---
## The World Bank: An Analysis of Finances Around the Globe
---


The World Bank Group is a unique global partnership of five institutions working for sustainable solutions that reduce poverty and build shared prosperity in developing countries consisting of 189 member countries, staff from over 170 countries, and over 130 office locations. The WBG has helped over 100 developing countries and, those in transition, adjust to the many changes in the world economy over the last 70 years by offering loans and tailored knowledge & advice. ~ worldbank.org

My analysis covered insights in the following areas:

- There are currently approximately **640,000 loans** with balances due across **136 countries**.  Many countries have multiple loans extended with **India** having the most at **56,190**. Top 5 countries include India, Bangladesh, Pakistan, Tanzania, and Ghana.
- 
-
-

## THE DATA
Using SQL, I conducted a comprehensive financial analysis of credits and grants issued by the International Development Association (IDA), an institution of The World Bank, using data consisting of over 1.24M rows and 30 columns provided from November 2022.  The data is also updated monthly by the 10th business day at [**TheWorldBank.org**](https://finances.worldbank.org/Loans-and-Credits/IDA-Statement-Of-Credits-and-Grants-Historical-Dat/tdwh-3krx). As noted on the site, the IDA credits are public and publicly guaranteed debt extended by the World Bank Group. The IDA provides development credits, grants, and guarantees to its recipient member countries to help meet their development needs.  Credits from IDA are at concessional rates and data are in U.S. dollars calculated using historical rates. The World Bank complies with all sanctions applicable to World Bank transactions.  You will also find a detailed data dictionary among other details.

To perform my analysis, I uploaded the data and ran SQL queries using [**csvfiddle.io**] (https://csvfiddle.io), an open-source tool.






## THE ANALYSIS

The main purpose of the analysis was to look over the dataset of loans consisting of credits or grants and provide insights on the following questions:



-Return all rows of the table, but only the borrower & due to IDA column

-Only show the first 5 rows of the previous query 

-Abbreviate one of the column names so it's easier to write 

-Show us all transactions from the Nicaragua (the country)?

-How many total transactions? 

-How many total transactions per country?? 

-What is the max owed to the IDA?

-Which was the most recent to pay?

-Who has the most loans? 



I started with a simple **SELECT * FROM table_name** query to become more familiar with the data and get a feel for things.  Because the dataset consists of over 1M rows I added a LIMIT to the initial query to only display the first several hundred rows.

<img src="images/Code3.png?raw=true"/>
<img src="images/Code3Query.png?raw=true"/>


<img src="images/Code2.png?raw=true"/>

<img src="images/Code2Query.png?raw=true"/>

<img src="images/Code1.png?raw=true"/>

<img src="images/Code1Query.png?raw=true"/>



<img src="images/Code1Query.png?raw=true"/>

<img src="images/Code1Query.png?raw=true"/>

<img src="images/Code1Query.png?raw=true"/>

<img src="images/Code1Query.png?raw=true"/>

<img src="images/Code1Query.png?raw=true"/>

<img src="images/Code1Query.png?raw=true"/>





Just like this. And you can even add internal coding blocks

```python
print('this is the python code I used to solve this problem')
```

### 2. You can add any images you'd like. 

<img src="images/dummy_thumbnail.jpg?raw=true"/>
