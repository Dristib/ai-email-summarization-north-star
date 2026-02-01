# AI Email Summarization – North Star Metrics

## Product Context
Professionals spend an average of **2–3 hours per day reading and triaging emails**, leading to cognitive overload, delayed decisions, and lower productivity. High-volume email users, including managers, analysts, and consultants, need a solution to quickly extract actionable insights from their inboxes.  

Our AI-powered Email Summarization tool generates **concise, contextually accurate summaries**, enabling users to triage and act faster while reducing cognitive load. This repo defines the **North Star Metric (NSM), input metrics, guardrails, and rationale** to measure success.


## Problem Statement
- Professionals are overwhelmed by email volume.  
- Existing email filtering tools fail to reduce reading time significantly.  
- AI summarization has potential, but needs measurable impact to ensure adoption and retention.  

**Goal:** Enable measurable productivity gains and high user satisfaction through accurate, actionable email summaries.


## North Star Metric (NSM)
**Weekly Active Summarized Emails (WASE)**  

**Definition:** Number of emails successfully summarized and actively consumed by users per week.  

**Rationale:**  
- Directly quantifies **value delivered to users** (time saved, decision acceleration).  
- Correlates strongly with **retention and engagement**: users who regularly consume summaries are more likely to stay.  
- Aligns with business outcomes: increased NSM → higher perceived product value → potential upsell or monetization opportunities.


## Input Metrics (Leading Indicators)
Metrics that drive the NSM and provide levers for product interventions:  

| Metric | Definition | Why It Matters |
|--------|------------|----------------|
| Active Users Performing Summarization (AUPS) | Number of unique users summarizing emails weekly | Adoption indicator; growth in active users is necessary for NSM scaling |
| Average Summaries per User (ASPU) | Average number of summaries generated per user per week | Engagement measure; increases in ASPU signal deeper product usage |
| Summary Accuracy Score (SAS) | Combined AI confidence and user validation of summaries | Ensures value delivered is meaningful; directly impacts NSM and retention |
| Time Saved per User (TSPU) | Estimated minutes saved per user per week | Quantitative measure of real user benefit and ROI from AI summaries |


## Guardrail / Safety Metrics
Guardrails ensure optimization of NSM does not compromise **quality or user experience**:

| Metric | Threshold / Consideration | Why It Matters |
|--------|-------------------------|----------------|
| AI Hallucination Rate (AHR) | <5% | Factually incorrect summaries reduce trust and adoption |
| Error Rate per Email (ERE) | <3% | High pipeline errors undermine reliability |
| User Churn Rate (CR) | Monitor trends weekly | Prevents NSM growth from masking declining retention |
| User Feedback Score (UFS) | Average post-summary rating ≥4/5 | Maintains qualitative experience and product credibility |


## Metric Rationale & Insights
- **NSM vs Vanity Metrics:** Metrics like total downloads, raw AI calls, or total emails in the system are misleading; they don’t reflect **actual value delivered**.  
- **Input metrics as levers:** ASPU, SAS, and TSPU are actionable. Increasing these metrics will directly influence WASE.  
- **Guardrails prevent false optimization:** Growth in NSM is meaningless if summaries are inaccurate, users churn, or satisfaction drops.  


## Scenarios & Examples
- **Scenario 1:** AI accuracy improves from 80% → 90% → NSM grows 15% because more users trust and consume summaries.  
- **Scenario 2:** Active users drop but NSM remains stable → indicates power users drive usage; consider strategies to expand adoption to casual users.  
- **Scenario 3:** Week 4 error spike → WASE drops → triggers investigation of pipeline reliability.  


## Mock Data Table (Illustrative)
| Week | Active Users | Avg Summaries | Summary Accuracy | WASE | Time Saved (min) |
|------|-------------|---------------|-----------------|------|----------------|
| 1    | 150         | 3             | 78%             | 390  | 780            |
| 2    | 160         | 3.2           | 80%             | 450  | 840            |
| 3    | 170         | 3.5           | 82%             | 485  | 912            |
| 4    | 180         | 3.6           | 85%             | 530  | 954            |
| 5    | 190         | 3.8           | 86%             | 610  | 1040           |
| 6    | 200         | 4             | 88%             | 660  | 1080           |

> Note: This is mock data for illustrative purposes; it simulates metric relationships over time.


## Execution & Next Steps
- **Monitor NSM weekly:** Align product releases or AI improvements with changes in WASE.  
- **Analyze input metrics:** Use ASPU, SAS, and TSPU to identify friction points and optimize feature adoption.  
- **Guardrails alerting:** Automate notifications if AHR, ERE, or UFS cross thresholds.  
- **Scenario planning:** Use metric simulations to forecast NSM growth from improvements in AI accuracy or engagement strategies.



## Why Not Vanity Metrics
Metrics like total downloads, total AI calls, or raw usage counts inflate activity signals without correlating to **actual user value**.  
> For example, high AI call volume does not guarantee accurate summaries or meaningful productivity gains. Focusing on WASE, input metrics, and guardrails ensures we optimize **outcomes over outputs**.
