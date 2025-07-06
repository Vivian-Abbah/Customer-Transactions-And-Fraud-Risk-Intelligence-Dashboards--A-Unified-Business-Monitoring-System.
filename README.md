# Customer-Transactions-And-Fraud-Risk-Intelligence-Dashboards--A-Unified-Business-Monitoring-System.

Introduction
Banking and transactional ecosystems are more complex and vulnerable than ever in today's digital world. As financial institutions strive to improve service personalization and fraud prevention, business intelligence (BI) plays a central role in making sense of massive volumes of data.
This project combines two dashboards built in Power BI to reveal the dual pulse of financial behavior:
Transaction Trends and Customer Behavior: This view focuses on when, how, and where customers transact. It dives into transaction frequency, value distribution by occupation, customer segmentation by age, and usage patterns across digital and physical channels.
Fraud Risk and Operational Insights: This companion view explores the other side of the coin - anomalies, high-risk patterns, and fraud-prone behaviors across customer demographics, locations, and transaction types.

These dashboards create a composite business intelligence layer that allows stakeholders to detect threats, uncover habits, and design smarter operations across marketing, fraud detection, and service delivery.

![Transaction Dashboard](https://github.com/user-attachments/assets/2dacd29a-f38a-4193-96eb-09bd87ce767d)

![Fraud Risk Dashboard](https://github.com/user-attachments/assets/a236149c-ed85-4013-bf84-02a099530850)



Objective of the Project

Track and visualize transactional behavior across customer segments and time periods.
Detect early signals of fraud using risk scoring, anomaly tracking, and geolocation patterns.
Provide insights into customer preferences by age, occupation, channel usage, and transaction timing.
Recommend actionable strategies for reducing fraud and enhancing customer experience.

Executive Summary
This business intelligence project merges two dashboards into a comprehensive insight system - Transaction Trends and Customer Behavior and Fraud Risk and Operational Insights. From the customer behavior perspective, students and engineers emerge as highly active segments, with most transactions occurring online and during late-night hours. Branch and ATM channels follow closely, with high reliance on credit transactions.
From the fraud risk lens, high-risk transactions are clustered around certain cities (e.g., Atlanta, Detroit), occupations (students, retirees), and transaction types (debit).
The dashboards highlight key anomalies, such as spikes in risk during low-traffic periods, and provide actionable pathways to strengthen digital banking services and fraud prevention frameworks.
Solution Approach
Data Modeling: Merged transactional and demographic data for unified analysis.
Custom Measures: Created DAX metrics for MoM trends, login attempts, risk flags, and average values.
Time & Geo Analysis: Explored how risk and behavior vary across time and location.
User Segmentation: Analyzed transaction patterns by occupation, age, and channel.
Risk Flagging: Compared normal vs. high-risk customer segments.

Key Dataset and Methodologies

Story of the Data

The dataset simulates 3,000+ real-world financial transactions containing attributes such as:
Transaction Date & Time
Transaction Amount
Occupation, Age, Channel, and Risk Flag
Login Attempts and Account Balance

Data Source

Synthetic dataset modeled after real financial banking logs, anonymized for privacy.
Simulates CitiBank customer profiles and transaction details.

Data Structure

Field Description, Customer Age, Numeric field for segmentation, Transaction TypeDebit or Credit, ChannelOnline, ATM, Branch, RiskFlag, Binary indicator for fraud suspicion, Occupation, Job role classification, Location, Geographic city name, Login Attempts, Behavioral signal.

Key Metrics and Dimensions

Transaction Amount & Count
Account Balance by Age
Transaction Duration
Customer Risk Segmentation
Channel Performance
Login Attempts

Data Limitations and Assumptions

Does not contain multi-year trends or longitudinal risk behavior.
Lacks biometric authentication variables (e.g., Face ID).
Geolocation is limited to city level (not GPS-based).
Assumes every transaction can be linked to a valid occupation and risk flag.

Data Cleaning and Preprocessing

Filled null login attempt values with average estimates.
Removed duplicate transactions using Order ID.
Transformed date-time into separate fields for hour and day.
Created DAX columns for:
Transaction Time of Day (e.g., Morning, Late Night)
Transaction Speed Category
RiskFlag Category

Industry Context & Stakeholders

Industry Context
Digital Banking, Fraud Detection & Compliance
Shift toward intelligent banking dashboards for decision-makers

Stakeholders

Fraud Analysts & Compliance Teams
Customer Support Operations
Executive Board

Pre-Analysis Board

Goals
Identify core behavioral drivers of transaction volume.
Surface suspicious transaction trends across channels and cities.

Expected Outcomes

Segmentation of high-value users and high-risk users.
Strategy recommendations for fraud prevention and customer engagement.

Emerging Trends

Late-night transactions are surprisingly high.
Students and engineers are the most active customer groups.
Online channels dominate, yet high risk remains around ATM usage.

Preliminary Questions

Do login attempts correlate with transaction risk?
Which age group holds the highest account balance?
What transaction types are most susceptible to fraud?

In-Analysis Phase

Key Insights

From Transaction Behavior Dashboard

Peak Activity by Time: Transaction value peaked at 17:30 and 19:12, suggesting evening periods are most active. This can inform support staffing and system monitoring schedules.

Monthly Trends: April and August saw the highest transaction volumes (71K & 72K), pointing to possible seasonal or campaign-based spending surges.

Top Channels: Online and Branch channels dominate (34% each), followed closely by ATM. Hybrid models are clearly the future.

Occupation Impact: Retired and Engineer customers have the highest month-over-month (MoM) transaction frequencies, indicating more consistent transactional habits.

Age and Balance: Customers aged 40–60 maintain relatively higher account balances, showing a strong correlation between age and financial maturity.

From Fraud Risk and Operational Dashboard

High-Risk Count: 95 transactions were flagged as high-risk from a total of 3K, comprising 18.2% of customers.

High-Risk Occupation: Students and Doctors had the highest flagged risk counts, likely due to irregular transaction patterns or shared accounts.

Location Clusters: Risk-prone areas include Atlanta, Austin, El Paso, and Detroit, necessitating geo-specific alerts and interventions.

Transaction Type Risk: 77.3% of high-risk cases involved credit transactions, underscoring the need for enhanced credit monitoring.

Risk by Time: Risk spikes occur between 17:00 and 18:30, overlapping with peak transaction hours - this is a critical risk window.

Bonus Insights and Metric Correlations

Late Night + Debit Card = High Risk: A consistent pattern that can be flagged in fraud detection systems.

High Risk by Occupation: Students and retirees are more likely to be involved in flagged transactions, possibly due to weaker authentication habits.

Account Balance Stability: Older customers (60+) maintain steadier balances despite lower transaction volume.

Channel-Specific Risk: ATM transactions carry higher fraud rates than online or branch.

Post-Analysis Phase

Recommendations

Implement AI-Driven Risk Models: Use machine learning to detect risk anomalies in real time by training on transaction durations, time-of-day, occupation, and channel usage.

Geo-Targeted Monitoring: Enhance fraud alert systems in high-risk cities like Atlanta and Detroit. Consider cross-checking IP and device metadata for additional security.

Customer Segmentation Campaigns: Personalize outreach based on occupation (e.g., offer tailored services to engineers and retired users) who show stable behavior and high account balances.

Channel Optimization: Since branch and online channels account for over 65% of all transactions, invest in omnichannel enhancements, including secure logins and multi-factor authentication.

Peak Hour Staffing and Infrastructure Load Balancing: Reinforce systems and support teams between 16:30 and 19:00, which are the busiest and riskiest times.

Financial Literacy Programs: Students showed higher fraud risk; targeted digital education could improve financial hygiene and reduce exposure.

Balance-Based Tier Monitoring: Older adults with higher balances should have a personalized fraud-protection package to maintain trust and security.

Conclusion

The dual-lens analysis of transaction behavior and fraud detection revealed much more than isolated KPIs - it uncovered a living, breathing ecosystem of customer habits, vulnerabilities, and operational blind spots.
Behavioral segmentation by time, age, occupation, and geography enabled us to predict not only what customers are doing, but why they're doing it - and where the risks lie. The fraud detection layer, intertwined with behavior trends, offers a 360-degree protection and personalization strategy for any modern financial institution.
In essence, this project delivers a blueprint for any bank or fintech company aiming to evolve from reactive operations to intelligence-led strategy. From optimized customer journeys to stronger fraud defense, the road ahead is clearer, smarter, and data-empowered.

Key Learnings

Behavioral segmentation is powerful in identifying both customer preferences and risk factors.
Peak transaction windows are also peak vulnerability periods.
Location and channel-specific insights offer major optimization opportunities.
Merging fraud insights with transaction trends offers a more accurate, predictive framework than either alone.

Limitations

Only one year of data analyzed; seasonal trends could be deeper with multi-year data.
No multi-device/session tracking available - important for risk scoring.
Behavioral data lacks psychographic inputs like customer intent or motivation.

Future Research

Integrate biometric and device fingerprinting for advanced fraud profiling.
Add sentiment analysis from customer support logs to correlate complaints with fraud trends.
Incorporate financial wellness scores or credit ratings for holistic customer profiling.
Extend to other banking products like loans, mortgages, or investment accounts.

References & Appendices

Data Source: Simulated Financial Transaction Dataset (2023)

Visualization Tool: Power BI (Dashboards built using measures, pie charts, DAX columns, time series, and geographic clustering)
Appendix A: RiskFlag Measure Logic
Appendix B: Top 10 Merchants by Value - Filtered Table
Appendix C: Data Preparation Flow in Power Query
