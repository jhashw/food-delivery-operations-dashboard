# Food Delivery Operations Dashboard

A Power BI project analyzing food delivery demand, customer retention, SLA performance, and restaurant-level operational bottlenecks using a synthetic transactional dataset.

## Project Overview

This dashboard was built to simulate how a food delivery operations team might monitor platform health across three lenses:

- **Executive performance tracking** through core KPIs like orders, revenue, average order value, ratings, SLA attainment, and P95 fulfillment time
- **Customer behavior analysis** through retention, order frequency, reorder timing, and day-hour demand patterns
- **Operational bottleneck diagnosis** through prep and delivery trends, late-order delay buckets, and restaurant-level contributors to delays
  
---

## Business Questions Answered

This dashboard was designed to answer questions such as:

- Is overall demand stable, or are orders and revenue shifting over time?
- How are customer ratings and SLA performance trending?
- Which cuisines and restaurants contribute most to revenue?
- Are late orders becoming more common, and when does performance worsen?
- How strong is customer retention quarter-over-quarter?
- When does demand peak by hour of day and day of week?
- Are repeat customers behaving differently from one-time customers?
- Which restaurants are driving operational delays in Q4?
- Are they delays primarily driven by preparation time or delivery time? 

---

## Dashboard Pages

### 1. Executive Overview
Focuses on overall platform performance and provides a high-level view of the most important metrics and trends

![alt text](https://github.com/jhashw/food-delivery-operations-dashboard/blob/main/images/overall_executive.png)

**Key Insight:**  
Demand remained stable, but ratings and SLA attainment declined toward year-end as delays increased, driven disproportionately by a few restaurants.

---

### 2. Customer Behavior Analysis (Q2)
Focuses on customer engagement, retention, and demand patterns.

![alt text](https://github.com/jhashw/food-delivery-operations-dashboard/blob/main/images/customer_behavior_q2.png)

**Key Insight:**  
Retention remains a challenge at ~21% QoQ with ~31% one-time customers, while demand peaks during lunch and evening hours, especially on weekends.

---

### 3. Q4 Operations Deep Dive
Focuses on identifying operational performance deterioration and restaurant-level bottlenecks in Q4.

![alt text](https://github.com/jhashw/food-delivery-operations-dashboard/blob/main/images/operations_q4.png)

**Key Insight:**  
In Q4, prep and delivery times rose across many restaurants, shifting more orders into late buckets despite slightly better delivery tail performance vs Q3.

---

## Key Findings

### Overall Performance
- Demand remained broadly stable across the year, with **101.3K total orders** and **$1.68M revenue**
- Customer experience softened toward year-end, with average ratings trending down and SLA attainment falling below target
- A small group of restaurants contributed disproportionately to late-order share
- American and Japanese cuisine together accounted for more than half of total revenue

### Customer Behavior
- Quarter-over-quarter retention was approximately **21.2%**
- Roughly **31% of customers placed only one order** in Q2
- Demand peaked during **lunch and evening hours**, with stronger activity on weekends
- Higher-frequency customer segments contributed a disproportionately large share of revenue

### Operations in Q4
- Average prep and delivery times increased versus Q3
- Prep-time deterioration appeared broader and more systemic than delivery-tail deterioration
- More orders shifted into longer delay buckets in Q4
- A small number of restaurants emerged as key contributors to late orders

---

## Data

This project uses a **synthetic food delivery dataset** which is based on the kaggle dataset https://www.kaggle.com/datasets/ahsan81/food-ordering-and-delivery-app-dataset.  

The dataset was expanded and augmented to simulate realistic platform behavior, including:
- lunch and dinner demand peaks
- weekend demand surges
- customer reorders
- restaurant-specific prep speed differences
- weak negative relationship between ratings and fulfillment time
- worsening late-order patterns in Q4

A sample dataset and data dictionary are included in this repository.
