<img src="images/worldbank_logo.png?raw=true"/>

---
## The World Bank: An Analysis of Finances Around the Globe
---


The **World Bank Group** is a unique global partnership of five institutions working for sustainable solutions that reduce poverty and build shared prosperity in developing countries consisting of **189 member countries**, **staff** from over **170 countries**, and over **130 office locations**. The **WBG** has helped over 100 developing countries and, those in transition, adjust to the many changes in the world economy over the last 70 years by offering loans and tailored knowledge & advice. 

~ worldbank.org


## My analysis covered insights in the following areas:
---

- The are over **1.24 Million** transactions with the IDA and the **total amount owed** is **over $19 Trillion US Dollars**
- There are currently over **639,000 loans** with balances due across **136 countries**.  Many countries have multiple loans extended with **India** having the most at **56,190** loans owed for various projects. The **top 5** countries include **India, Bangladesh, Pakistan, Tanzania, and Ghana**.
- **India** owes the largest single loan amount of nearly **800 Million US dollars** while **Mozambique** actually has a credit of just over **$5.00**.
- **India** has loans for over **39,500** different projects. The **IN: SSA III**, an elementary school education project, is the largest loan owed by India and the largest loan owed to the IDA at nearly **800 Million**.
- The **average service rate** is **0.78%**
-

## THE DATA
---

Using **SQL**, I conducted a comprehensive financial analysis of credits and grants issued by the International Development Association (IDA), 1 of the 5 institutions of The World Bank.  The IDA provides concessional financing to some of the world's poorest countries to help them lift themselves out of poverty. This financing lets countries work toward economic efficiency providing access to health, nutrition, social services, and a better quality of life. 

~worldbank.org

The data consists of over **1.24M rows** and **30 columns** provided from **November 2022**. It is also updated monthly by the 10th business day at [**TheWorldBank.org**](https://finances.worldbank.org/Loans-and-Credits/IDA-Statement-Of-Credits-and-Grants-Historical-Dat/tdwh-3krx). As noted on the site, the IDA credits are public and publicly guaranteed debt extended by the World Bank Group. The IDA provides development credits, grants, and guarantees to its recipient member countries to help meet their development needs.  Credits from IDA are at concessional rates and data are in U.S. dollars calculated using historical rates. The World Bank complies with all sanctions applicable to World Bank transactions.  You will also find a detailed data dictionary among other details.

To perform my analysis, I uploaded the data and ran SQL queries using [**csvfiddle.io**](https://csvfiddle.io), an open-source tool that allows its users to run SQL queries exclusively in-browser eliminating the need to download software like MySQL on their computer.


## THE ANALYSIS
---

**SQL commands used while performing my analysis include:**

✅SELECT* ✅FROM table_name ✅LIMIT ✅AS ✅WHERE ✅COUNT ✅GROUP BY ✅ORDER BY 
✅ MIN/MAX ✅SUM ✅AVG ✅AND/OR/NOT

---

The main purpose of the analysis was to look over the dataset of  IDA transactions consisting of loans in the form of credits or grants and provide insights on the following questions:

-What is the total number of transactions?✅

-What is the total amount owed to the IDA?✅

-What is the total number of transactions with balances due per country?✅ 

-How many loans per country?✅

-What country has the most loans?✅ 

-What is the MAX/MIN loan owed to the IDA?✅

-all transactions from India (the country)✅

-What is the total number of projects for India?✅

-How many loans did India receive for each project?✅

-Which project in India is responsible for the highest balance owed?✅

-What country was the most recent to pay their loan?

-What is the average service charge rate for a loan?

-ORDER BY

-AND/OR/NOT
 



✅I started with a simple **SELECT * FROM table_name** query to become more familiar with the data and get a feel for things.  There are over **1.24 Million** rows representing the total amount of transactions made with the IDA. Because the dataset consists of over **1M rows** I added a **LIMIT** clause to the initial query to only display the first several hundred rows.  **Note:**  I also had to add a **LIMIT** clause to other queries due to the large size of the dataset.

<img src="images/Code3.png?raw=true"/>
<img src="images/Code3Query.png?raw=true"/>

✅Next, I queried to find the total amount owed to the IDA using a **SUM** function. The total is over **19 Trillion US dollars** ($19,204,389,797,689.50).

<img src="images/Code9.png?raw=true"/>
<img src="images/Code9Query.png?raw=true"/>

✅I then wanted to take a look at the total number of transactions with balances due per country using the borrower, DueToIda, and country fields.  The initial query resulted in multiple borrowers with **zero dollars** owed and borrowers with the same or similar names listed so I filtered out the zero balances using a **WHERE** clause. Results showed that there were over **639,000 loans** with balances due at the time of my analysis.

<img src="images/Code2.png?raw=true"/>
<img src="images/Code2Query.png?raw=true"/>

✅Of those **639,000 loans**, how many loans are held by each country?  Using a **COUNT** function with **GROUP BY** and **ORDER BY** clauses, I ran another query. Results indicated there were **136 countries** with outstanding loans.  At the time of analysis, **India** held the top position with **56,190** outstanding loans.  Among the **top 5** countries were **India, Bangladesh, Pakistan, Tanzania, and Ghana**.

<img src="images/Code1.png?raw=true"/>
<img src="images/Code1Query.png?raw=true"/>
<img src="images/Code2Query2.png?raw=true"/>

✅Next, I set out to find which country owed the largest amount in loans to the IDA and which owed the least.  Using **MAX/MIN** functions, results showed that **India** owes the largest single loan amount just shy of **800 Million US dollars** coming in at $793,256,128.00. **Mozambique** appears to have a credit in the amount of **-$5.37**.

<img src="images/Code4.png?raw=true"/>
<img src="images/Code4Query.png?raw=true"/>
<img src="images/Code5.png?raw=true"/>
<img src="images/Code5Query.png?raw=true"/>

✅With **India** owing just shy of **800M US dollars** to the IDA, I wanted to dive a little deeper.  First, I listed all **56,190** transactions and their corresponding fields for the country.

<img src="images/Code6.png?raw=true"/>
<img src="images/Code6Query.png?raw=true"/>

✅Next, I filtered to find the total number of projects for **India**. There are over **39,500** different project names listed for **India**.

<img src="images/Code7.png?raw=true"/>
<img src="images/Code7Query.png?raw=true"/>
<img src="images/Code7Query2A.png?raw=true"/>

✅Some projects have multiple loans. For Example, there are **over 136 HIGHWAYS, 294 RAILWAYS, and 276 TELECOMMUNICATIONS** projects all of which have a **ZERO Balance**.

<img src="images/Code10.png?raw=true"/>
<img src="images/Code10Query.png?raw=true"/>

✅Next, I wanted to know which project in **India** was responsible for the highest balance owed.  Results revealed that the **IN: SSA III**, an elementary school education project focused on providing better outcomes for children, was the largest loan owed by India and the largest loan owed to the IDA at nearly **$800 Million US dollars**.


<img src="images/Code8.png?raw=true"/>
<img src="images/Code8Query.png?raw=true"/>



