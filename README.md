# Analyzing-Customer-Churn-and-Retention-Patterns-in-a-UK-Based-Multinational-Retail-Bank

# Project Background
Veritas Bank is a UK-headquartered retail bank operating across the UK, Germany, and France, serving over 3 million customers. Known for its strong digital banking capabilities and regional adaptability, the bank offers core retail services such as savings accounts, personal loans, and debit/credit card products.

In recent years, the bank has experienced rising customer churn, driven by growing competition from fintech challengers, declining engagement especially in Germany and France and the absence of targeted retention or early-warning systems. Without real-time segmentation or churn monitoring, the bank has struggled to address customer attrition proactively.

This project was initiated to help Veritas Bank understand why customers leave, identify who is most at risk, and support data-driven retention strategies. By uncovering churn drivers, comparing customer behavior across regions, and segmenting customers into risk tiers, the bank can make informed decisions to improve retention, enhance customer lifetime value, and refine acquisition strategies.

The analysis focuses on identifying churn patterns, understanding regional differences, grouping customers into actionable risk segments, and visualizing insights through interactive dashboards that enable leadership to quickly assess and respond to churn-related trends.

Insights and recommendations are provided on the following key areas:

1.	Customer Demographics & Segmentation	
2.	Customer Activity & Engagement
3.	Churn Patterns Across  Countries (Branches)
4.	Risk Profiling & Churn Drivers
5.	Customer Acquisition & Loyalty


# Data Structure & Initial Checks
Veritas Bank database structure as seen below consists of Four tables: Customers,Accounts, CustomerRisk,ChurnAnalysis with a total row count of 20,000 records.

A description of each table is as follows:

• Table 1: Customers

• Table 2: Accounts

• Table 3:CustomerRisk

• Table 4:ChurnAnalysis



<img width="863" height="340" alt="Bank -Data structure " src="https://github.com/user-attachments/assets/968ac637-a5bd-4863-8ed1-3bd5a9c95c79" />


# Executive Summary

The churn analysis highlights clear differences between active and inactive customers, with engagement level and credit score emerging as key churn indicators. Active customers despite having low to moderate product engagement and poor–fair credit scores generally remain with the bank, showing that activity alone is a strong retention driver.

 In contrast, inactive (or dormant) customers with similarly low engagement show mixed churn outcomes, indicating higher vulnerability. Older customers demonstrate the strongest loyalty, while younger segments show a more balanced mix of churn and retention.
 
Overall, improving engagement among inactive customers, strengthening onboarding for younger cohorts, and offering tailored credit-support programs will drive better retention outcomes.

# Insights Deep Dive

## Demographics & Segmentation



<img width="453" height="98" alt="bank demographics " src="https://github.com/user-attachments/assets/253cde91-0d93-455f-987e-5d58accd47bf" />

The bank has more male than female customers across all three markets.

The largest age groups are 26–35 and 36–45, representing the core customer base.( Young or mid-level Professionals )

<img width="449" height="94" alt="credit score   balance" src="https://github.com/user-attachments/assets/d3cb20f8-60ef-4397-9ca2-655978123f8f" />

Most customers fall into Poor, Fair, or Good credit score categories.(Average credit score: 650.60)

Customer balances vary widely, with concentrations in very low (<£1k) and high (£10k–£100k) ranges; mid-level balances are uncommon.(Average customer balance: £27.15k)

<img width="449" height="105" alt="products and tenure " src="https://github.com/user-attachments/assets/01aec3b0-880f-45d9-a36e-8a50cb3599b8" />

Tenure distribution shows:

Loyal customers (>5 years) are the largest group.

New customers (0–2 years) are the smallest;suggesting weak customer acquisition.

Product engagement remains low; Majority hold 0–2 products, with very few reaching high engagement (≥3 products) ; indicating difficulty in driving cross-sell.

## Churn Analysis

<img width="259" height="296" alt="churn and products " src="https://github.com/user-attachments/assets/93c6e8b9-b2b7-43a5-a27b-3a7ebc8c5eca" />

• Churn is high across all regions:

UK: 498, Germany: 453, France: 434 ;differences are small, showing churn is not region-specific.

• Credit card ownership does not appear to influence churn:

Non-churned without credit card: 1.5k

Churned without credit card: 1.4k

• Customer engagement remains flat regardless of tenure ; even loyal customers rarely progress beyond moderate engagement.


<img width="252" height="197" alt="balances and credit score " src="https://github.com/user-attachments/assets/ffa4220d-e92e-4ccf-92e4-ef2b172b880a" />

•Average balance of churned customers:

Germany: £15k

UK: £17k

France: £17k

•Germany’s retained customers have the highest average balance (£30k) compared to the UK (£29k) and France (£28k).

•Most churned customers fall within Poor/Fair/Good credit score bands, indicating mid and low quality credit profiles are more vulnerable to leaving.

## Risk Profile - High Churn Risk


<img width="630" height="341" alt="Active , High Risk" src="https://github.com/user-attachments/assets/bc8e6454-5e8a-4a56-b18e-da262849b92a" />


1. Active Customers ; High Churn Risk

Even among customers who are actively using the bank, certain segments show high churn risk:

Low product engagement (0–1 products)

Poor to Fair credit scores

Age groups: 26–35 and 36–45

These customers are active but not deeply committed, suggesting the bank is failing to convert activity into long-term engagement or loyalty.

Customers may be exploring alternatives, experiencing dissatisfaction, or not finding value that encourages deeper product adoption.


<img width="635" height="309" alt="Inactive ,High risk" src="https://github.com/user-attachments/assets/461b089a-1d6d-4ddb-941a-ec3ff3da9253" />


2.Inactive Customers ; High Churn Risk

Inactive customers show an even clearer risk pattern:

Low product engagement

Poor–Fair credit scores

Present across all age groups

Their inactivity combined with weak financial profiles makes them the most vulnerable segment.

Low engagement and inactivity usually signals customers who are disengaging from the bank’s ecosystem, making them likely to churn if not re-engaged quickly.


## Overall Takeaway

•Across both active and inactive customers, the common indicators of churn risk are:

Low product engagement

Poor–Fair credit quality

Younger to mid-age adults (26–45) for active users

All ages for inactive users

•This means engagement and activity is the strongest predictor of churn.

# Stratigic Recommendation

### 1.	Customer Acquisition & Onboarding

•Executives (C Suite) – Set acquisition KPIs (new customers per quarter, tenure growth). Approve budget for digital campaigns

•Regional/Country Managers- Localize onboarding flows to regional/country preferences (Germany/France).

•Product Teams- Design bundled starter packs (savings + card). 	Offer welcome bundles (e.g., fee waivers, starter savings + credit card combo) to encourage product adoption early.

•Marketing - Run targeted digital campaigns for 26–35 age group.

•Risk & Compliance - Ensure onboarding offers comply with lending regulations.


### 2.	Product Engagement & Cross-Sell
   
•	Executives (C Suite) -Mandate cross-sell targets (≥3 products per customer). Track engagement tiers in dashboards

•	Regional/Country Managers- Adapt cross-sell incentives to local product preferences.

•	Product Teams -Build tiered product bundles and loyalty rewards.

•	Marketing - Personalize offers via app/email nudges.

•	Risk & Compliance - Monitor credit score–linked offers for responsible lending.


### 3. Retention & Churn Prevention
     
•	Executives (C Suite) - Sponsor predictive churn system development. Allocate resources for proactive retention.

•	Regional/Country Managers- Deploy region-specific retention campaigns (e.g., reactivation bonuses).

•	Product Teams - Integrate churn flags into CRM workflows.

•	Marketing - Launch reactivation campaigns for inactive customers.

•	Risk & Compliance - Validate churn models against fair lending and data privacy standards.

3. Retention & Churn Prevention
- Early-warning churn system: Build predictive models around the strongest churn indicators (low product engagement + Poor/Fair credit).
- Flag customers with declining activity for proactive outreach.
- Segment-specific retention strategies:
- Active but at risk (26–45, low engagement) → Offer lifestyle-linked products (travel, digital wallets, BNPL) to deepen relevance.
- Inactive at risk (all ages, low engagement) → Launch reactivation campaigns (cashback, fee waivers, “return bonus” for re-engagement).
- Balance-based prioritization: Since retained German customers have higher balances (£30k), prioritize retention of high-balance segments with VIP service tiers and relationship managers.


4. Regional Strategy

•	Executives (C Suite) - Approve centralized churn dashboard with regional drill-downs.

•	Regional/Country Managers- Benchmark UK practices, adapt for Germany/France.

•	Product Teams - Adjust product mix to reflect local demand.

•	Marketing - Tailor messaging to cultural/market nuances.

•	Risk & Compliance - Ensure compliance with EU regulations across regions.


5. Customer Experience & Value Proposition
   
•	Executives (C Suite) - Endorse loyalty ecosystem (Veritas Loyalty Club). Track customer lifetime value metrics.

•	Regional/Country Managers- Implement local partnerships for perks (travel, retail).

•	Product Teams - Develop credit improvement tools and gamified score tracking.

•	Marketing - Promote financial health programs and loyalty benefits.

•	Risk & Compliance - Oversee responsible credit improvement initiatives and customer data protection.

5. Customer Experience & Value Proposition
- Financial health programs: Since churn risk is tied to Poor/Fair credit, launch credit improvement journeys (education, score tracking, gamified milestones).
- Loyalty ecosystem: Reward tenure and engagement with tiered benefits (e.g., “Veritas Loyalty Club” offering travel perks, fee waivers, or partner discounts).
- Feedback loops: Collect churned customer feedback systematically to refine product-market fit and service quality.












  
