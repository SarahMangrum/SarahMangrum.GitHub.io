# Burgers and Fries...Oh My!:  A Look at Food Delivery Sales

From deep within the pit of my stomach arose a grumble that shook the foundation beneath my feet. I had been tirelessly studying and was in such a groove, I didn't want to have to stop and lose my momentum by rummaging through the refrigerator and cupboards looking for something to quell the hangry beast festering inside. So...what's a girl to do? Insert >> local food delivery service to the rescue!
I ordered my favorite vegan burger and fries combo and in just under 30 minutes it was at my door and making its way into the cavernous pit of my empty stomach. This got me thinking...How many other people use food delivery services? What is their go-to meal? How much are people willing to spend on this convenient service? Are they just Gen Z's ordering their latest coffee concoction or Millennials running kids to soccer practice and Christmas concerts, too tired to even think about cooking when they finally make it home?
With the help of an online dataset and the analysis tool, *Excel*, I got to work analyzing the data. I discovered some interesting facts about how food delivery service sales and demographics, from companies like DoorDash, use marketing campaigns to attract their customer base and get us to spend our money.
So, if you want to learn more about companies like DoorDash and the people who spent over **$1.24 Million** on this service, keep reading...
 

## Let's Talk Data

**DoorDash** or, in this case, *iFood*, the Brazilian equivalent, is a leading food delivery option operating in Brazil and Columbia with over **80% market share** in its Brazilian sector.
Using a modified version of a DoorDash-like case study given to potential data analyst applicants during the interview process, I got started reviewing the data:

*Note that this project is actually modified from an iFood job interview case study given by the Brazilian equivalent of DoorDash, iFood. The data is 98% real but slightly modified for educational purposes. 

(https://www.kaggle.com/datasets/jackdaoud/marketing-data)

The 2018 dataset of iFood yearly sales consists of 2,205 unique customer rows and 36 columns. Luckily, a data dictionary exists, so I could immediately ascertain what each column represented.


### 2. You can add any images you'd like. 

<img src="images/DataDictionary?raw=true"/>

## The Analysis

Key *Excel* skills used:

* Create a new column + Fill
* Data Filtering
* Data Sorting
* Data Aggregation (min, max, sum, count, average, etc.)
* General Formulas (% of)
* Graphs
* Advanced Formulas (IF, SUMIF, COUNTIF, texts, dates, etc.)
* VLOOKUP and Data Validation

### How I Did It:

I began by adding a unique "CustomerID" **column** and then **sorting** and **filtering** the data for the various questions I wanted to ask:

1.  How many customers made purchases in Campaign 6?
2.  What was the total spent by each customer in Campaign 6?
3.  What was the highest total spent by a customer?
4.  How many customers were included in the entire analysis? And for Campaign 6?
5.  What was the age of the oldest customer?
6.  What was the average total amount spent by each customer?
7.  What was the total amount spent by all customers combined?
8.  Who was the most recently acquired customer?
9.  What was the percentage of income spent by each customer?
10. How many customers made purchases during Campaign 6? What were their ages? Do they have children?
11. How many customers joined monthly?

Focusing on Campaign 6 for a moment, I **filtered** the data to include only those customers that made a purchase.
Of the 2,205 customers, **333**, made a purchase during Campaign 6.
