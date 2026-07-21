# ApexLink Supply Chain Analytics

End-to-end data analysis project covering data cleaning, SQL querying, and Power BI dashboarding for a Nigerian supply chain and logistics company. Built to answer real operational and revenue questions, not just chart the data.

---

## The Business

ApexLink Supply Chain Ltd is a Nigerian logistics company handling procurement, warehousing, and distribution of consumer goods to wholesalers, retailers, and corporate clients across the country, through warehouses in Lagos, Abuja, Port Harcourt, and Kano.

## What This Project Does

Took a raw, messy 500-record order dataset through the full analytics pipeline:

1. **Cleaned it:** deduplicated, standardized inconsistent naming (suppliers, warehouses, products, regions), fixed data types, handled missing and negative values, resolved outliers.
2. **Queried it:**  34 SQL queries covering filtering, aggregation, `GROUP BY`/`HAVING`, `CASE` logic, and views.
3. **Modeled it:**  Power BI dashboard with 9 DAX measures, 10 visuals, and slicers for interactive filtering.
4. **Interrogated it:** answered 14 specific business questions management would actually ask, each with a driver, an impact, and a recommendation attached.

## Tools Used


1. Microsoft Excel : Data cleaning, calculated columns, PivotTables, first-pass dashboard 
2. MySQL: Database creation, querying, views 
3. Power BI: Data modeling, DAX measures, interactive dashboard 

## Key Numbers

- **500** orders analyzed, **₦62.95B** in total sales
- **6** suppliers, **5** warehouses, **6** product categories, **3** customer regions
- **58.8%** delivered order rate with cancelled, returned, and pending splitting the rest almost evenly
- **28.2%** of orders (₦12.01B) end in cancellation or return

## Top Findings


- **Revenue is concentrated, not diversified.** One supplier (Dangote Plc) drives 33% of sales, one warehouse (Port Harcourt) handles 47.5%, and one region (South-South) accounts for 76.5%. Three single points of failure carrying the business.
- **The top revenue product is the least reliable one.** Laptops generate 37% of total revenue but have the lowest delivered rate (55.9%) of any product nearly 1 in 3 laptop orders fails to complete.
- **Delivery times are bimodal, not just slow.** 62.8% of orders deliver in 6 days or less but 31.2% land on exactly 95 days, with nothing in between. That specific, repeated value looks more like a system artifact than natural delivery variance, and is flagged for verification rather than treated as confirmed fact.
- **Order failure is a bigger cost problem than logistics spend.** ₦12.01B in sales. Nearly a fifth of revenue is tied up in cancelled or returned orders that still consumed warehouse and staff time with zero return.


## Dashboard Preview

**Microsoft Excel Preview**
<img width="4090" height="1842" alt="ApexLink" src="https://github.com/user-attachments/assets/c9a16f3e-da39-4766-a56c-00949624114a" />

**Power Bi page 1 Preview**
<img width="673" height="380" alt="Screenshot 2026-07-20 183915" src="https://github.com/user-attachments/assets/29460349-46c5-49d1-9696-5577309bcc08" />

**Powwer Bi page 2 Preview**
<img width="673" height="378" alt="Screenshot 2026-07-20 183951" src="https://github.com/user-attachments/assets/6a18ad58-f1ea-4507-aa3b-ba1f209fc310" />

**MySql Preview**
<img width="960" height="497" alt="Screenshot 2026-07-21 235903" src="https://github.com/user-attachments/assets/3b88d598-13dd-40f5-bd7b-631378c90e23" />




## Business Questions Answered

1. Which supplier generated the highest sales?
2. Which warehouse handled the highest sales volume?
3. Which product generated the highest revenue?
4. Which customer region generated the most sales?
5. Which warehouse had the highest average delivery time?
6. Which supplier had the most late deliveries?
7. Which products should be restocked?
8. Which products should be discontinued?
9. What causes delivery delays?
10. How can operational costs be reduced while improving customer satisfaction?
11. Which order status occurred most frequently?
12. Which month recorded the highest sales?
13. What are the top five best-performing products?
14. What should management do next?

Every answer follows the same structure: what happened, why it likely happened, why it matters, what it costs or earns the business, and what to do about it.

## A Note on Data Integrity

Two things in this dataset are flagged rather than smoothed over, because a real analyst reports what the data says, not what makes the report cleaner:

- **60 orders (18% of sales) are attributed to an "Unknown" supplier**, and **49 orders (7.6% of sales) have no warehouse assigned.** These are real revenue but untracked — a genuine operational gap, not something to quietly exclude.
- **156 orders (31.2%) show an identical 95-day delivery time.** That level of repetition doesn't look like natural variance. It's presented in the analysis as a data quality question to verify, not a confirmed root cause — the honest move when a pattern looks more like a system default than a real measurement.

## About Me

Data analyst, recently completed a hands-on 6-month data analytics program covering Excel, SQL, and Power BI. This project reflects how I approach analysis: start from the business question, not the chart type, and don't present a finding as fact until it's actually verified.

**Joecliff Ayibabrakemi Wilson** — [www.linkedin.com/in/joecliff-wilson] · [joecliffayibabrakemi@gmail.com] 
