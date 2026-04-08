# TripleTen Sprint X Project – EDA & Statistical Analysis
This project was part of the TripleTen Data Science program. It focused on analyzing customer behavior across two Megaline mobile plans — Surf and Ultimate — to understand usage patterns and revenue performance.

---

## Megaline Sales Analysis
The goal of the project was to explore how customers use call minutes, messages, and data across the two plans, and determine which plan generates more revenue. The analysis also identifies where customers exceed their plan limits and how that affects Megaline’s earnings.

---

## The Data
The dataset was provided by TripleTen and contains monthly usage information for Megaline customers. It includes the following files:

### users.csv  
Each row corresponds to one Megaline customer.  
- **user_id**: Unique customer identifier  
- **first_name**: Customer’s first name  
- **last_name**: Customer’s last name  
- **age**: Customer age  
- **city**: City of residence  
- **plan**: Mobile plan (Surf or Ultimate)  

### calls.csv  
Each row represents one phone call.  
- **id**: Unique call record ID  
- **call_date**: Date of the call  
- **duration**: Call duration in minutes  
- **user_id**: Customer who made the call  

### messages.csv  
Each row represents one text message.  
- **id**: Unique message record ID  
- **message_date**: Date the message was sent  
- **user_id**: Customer who sent the message  

### internet.csv  
Each row represents one internet session.  
- **id**: Unique session ID  
- **mb_used**: Megabytes used during the session  
- **session_date**: Date of the session  
- **user_id**: Customer who used the data  

### plans.csv  
Each row describes one of Megaline’s mobile plans.  
- **plan_name**: Surf or Ultimate  
- **usd_monthly_fee**: Monthly subscription cost  
- **minutes_included**: Monthly included call minutes  
- **messages_included**: Monthly included text messages  
- **mb_per_month_included**: Monthly included data  
- **usd_per_minute**: Cost per extra minute  
- **usd_per_message**: Cost per extra message  
- **usd_per_gb**: Cost per extra GB of data  

---

## The Process
I began by exploring each dataset to identify missing values, duplicates, and inconsistencies. After cleaning the data, I merged the tables into a single analytical dataset containing monthly usage per customer.

I then analyzed:

- Total monthly call minutes  
- Number of messages sent  
- Data usage in MB  
- How often customers exceeded their plan limits  
- Monthly revenue per customer  
- Revenue differences between Surf and Ultimate users  

Statistical tests were used to determine whether revenue differences between the two plans were significant.

---

## Results
This project helped me practice combining EDA with statistical analysis to answer a real business question. I wrote an introduction and conclusion summarizing the findings and provided recommendations for Megaline, including:

- Surf users frequently exceed their limits, creating unpredictable charges  
- Ultimate users generate more stable and consistent revenue  
- Megaline could benefit from encouraging Surf users to upgrade  
- Adjusting Surf plan limits or pricing may reduce churn  

Please have a look at the Jupyter Notebook included for a full description of results.
