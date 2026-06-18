# Business Memo: Initial Churn Risk Assessment

**To:** Product, Marketing, and Customer Support Teams  
**From:** Data Science Team  
**Subject:** Exploratory Data Analysis & Churn Risk Hypotheses prior to Modeling  

## Overview
Before deploying our machine-learning model or launching blind retention campaigns, an audit of our historical data was conducted to understand customer behavior and identify baseline churn risks. Based on the Exploratory Data Analysis (EDA), we have identified five key data-backed hypotheses regarding why customers are churning.

## 5 Churn-Risk Hypotheses (Based on EDA Charts)
1. **The "Lack of Loyalty" Hypothesis (Chart 3):** Customers who are not enrolled in any loyalty tier form the vast majority of our churned user base. Hypothesis: *Failing to capture users into the loyalty program early greatly increases their likelihood of churning.*
2. **The "Support Friction" Hypothesis (Chart 4):** Customers who churned show a noticeably higher median volume of support tickets. Hypothesis: *Frequent friction points requiring support interventions are driving customers away, indicating underlying product or delivery issues.*
3. **The "Habit Formation" Hypothesis (Chart 5):** Churned customers consistently show a lower total number of lifetime orders. Hypothesis: *Customers who do not reach a specific "habit-forming" threshold of repeat orders quickly abandon the brand.*
4. **The "Digital Disengagement" Hypothesis (Chart 6):** Churned customers exhibit significantly lower web/app engagement events. Hypothesis: *A drop in digital engagement (app opens, browsing) is a strong leading indicator of impending churn.*
5. **The "Product Fit" Hypothesis (Chart 2):** Customers with specific skin types (e.g., Sensitive or Unknown) show varied retention rates. Hypothesis: *We may be lacking adequate product lines or clear onboarding education for certain demographic groups, leading to dissatisfaction.*

## Strategic Recommendations
Before launching targeted retention campaigns, the company should investigate the following:
* **Proactive Support Interventions:** Do not wait for an at-risk customer to complain three times. We should trigger a specialized support outreach or discount after a customer's second ticket.
* **Loyalty Onboarding:** Marketing should investigate whether offering a sign-up incentive to convert "No Tier" customers into baseline loyalty members reduces 60-day churn.
* **Engagement Triggers:** The product team should investigate launching automated re-engagement push notifications for users whose web/app event counts drop below the median retained user's baseline.