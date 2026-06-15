# arielrenara-source-albertus-ariel-oca-client-segmentation-business-analysis
Business analytics project analyzing enterprise communication behavior, revenue contribution, and customer segmentation for OCA Indonesia.

# 📊 OCA Indonesia - Active User Behavior & Client Segmentation Analysis

## Project Overview

This project was developed as part of the **Rakamin Academy x Telkom Indonesia Virtual Internship Program**.

The objective of this analysis is to understand enterprise client behavior on OCA Indonesia's communication platform and identify actionable customer segments to support business growth, customer retention, and upselling strategies.

Using transactional data from multiple communication channels (WhatsApp, SMS, Email, and Call), clients were segmented based on their usage frequency and revenue contribution using an FM-based RFM approach.

---

## Business Background

OCA Indonesia is a Communication Platform-as-a-Service (CPaaS) owned by Telkom Indonesia that enables businesses to send communications at scale through:

- WhatsApp
- SMS
- Email
- Call (IVR)

The company generates revenue from successfully delivered communications, making delivery performance and client engagement critical business metrics.

---

## Business Problems

The company needs to:

1. Understand differences in communication behavior among clients.
2. Identify high-value and low-value customers.
3. Develop data-driven personalization and upselling strategies.
4. Detect potential churn risks through engagement patterns.

---

## Project Objectives

- Segment enterprise clients based on communication behavior.
- Identify the most profitable customer groups.
- Detect potential churn risks.
- Discover upselling opportunities across communication channels.
- Provide strategic recommendations for each customer segment.

---

## Dataset Information

### Dataset Scope

| Dataset | Rows |
|----------|---------:|
| WhatsApp Transactions | 50,000 |
| SMS Transactions | 20,000 |
| Email Transactions | 40,000 |
| Call Transactions | 12,749 |
| Users | 20 |

**Analysis Period:** January – March 2025

**Total Transactions:** ~122,700

---

## Tools & Technologies

- Google BigQuery
- SQL
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab

---

## Methodology

### 1. Data Extraction

- Queried four communication channel datasets
- Joined transaction tables with user information
- Calculated user-level metrics

### 2. Feature Engineering

Created:

- Total Revenue
- Total Transactions
- Delivery Rate
- Revenue per Channel
- Dominant Channel
- Active Days
- Last Active Date
- Revenue per Transaction

### 3. FM-Based RFM Scoring

Since all users had similar recency values, segmentation focused on:

- Frequency (F)
- Monetary (M)

Scoring thresholds were created using percentile-based categorization.

### 4. Rule-Based Segmentation

| Segment | FM Score |
|----------|----------|
| Power User | 6 |
| Active User | 4 - 5 |
| Regular User | 2 - 3 |

### 5. Insight Generation

Visualization and business interpretation were performed to identify:

- Revenue contribution
- User behavior patterns
- Channel effectiveness
- Upsell opportunities
- Churn indicators

---

## Key Findings

### 💎 Power Users

- 6 clients
- Average Revenue: Rp3.24M
- Average Transactions: 15,349
- Contribute approximately 65% of total platform revenue
- Most active during 08:00 – 11:00

**Characteristics**
- High-volume enterprise users
- Utilize all communication channels
- Strong operational efficiency

### 🚀 Active Users

- 7 clients
- Average Revenue: Rp0.61M
- Average Transactions: 2,867
- Contribute approximately 22% of platform revenue
- Most active during 11:00 – 15:00

**Characteristics**
- Consistent platform usage
- Significant growth potential
- Similar channel preferences to Power Users

### 📈 Regular Users

- 7 clients
- Average Revenue: Rp0.32M
- Average Transactions: 1,512
- Contribute approximately 13% of platform revenue
- Most active during 12:00 – 16:00

**Characteristics**
- Lower communication volume
- Higher Call RNA (Ring No Answer) rate
- Opportunity to improve ROI through channel optimization

---

## Root Cause Analysis

### 1. Usage Volume Gap

Power Users generate approximately:

- 4x more revenue than Active Users
- 16x more revenue than Regular Users

### 2. Channel Effectiveness

- SMS contributes approximately 46% of total revenue.
- WhatsApp contributes approximately 39%.
- Call channels show a 76% RNA rate, indicating lower effectiveness.

### 3. Behavioral Timing

Different customer groups exhibit distinct communication schedules:

| Segment | Peak Activity |
|----------|--------------|
| Power User | 08:00 – 11:00 |
| Active User | 11:00 – 15:00 |
| Regular User | 12:00 – 16:00 |

---

## Business Recommendations

### Power Users

- Implement Enterprise Loyalty Program
- Assign Dedicated Account Managers
- Provide Early Access to New Features
- Offer Premium SLA Packages

### Active Users

- Upsell Higher Volume Packages
- Introduce Automated Blast Scheduling
- Cross-sell WhatsApp Marketing Templates

### Regular Users

- Offer Starter Growth Bundles
- Reduce dependency on Call channels
- Shift communication toward WhatsApp and SMS
- Provide campaign scheduling consultation

---

## Business Impact

This segmentation framework helps OCA Indonesia:

- Prioritize high-value customers
- Improve customer retention
- Optimize resource allocation
- Increase upselling effectiveness
- Improve communication channel ROI

---

## Project Structure

```
├── data/
├── sql/
│   └── oca_segmentation_query.sql
├── notebooks/
│   └── oca_segmentation_analysis.ipynb
├── visualizations/
├── presentation/
│   └── OCA_VI_Project_2.pdf
└── README.md
```

---

## Disclaimer

The dataset used in this project is a modified representation of the original data and has been adjusted for educational purposes. All analyses, insights, and recommendations are intended solely for academic and portfolio use and do not represent the actual business performance or conditions of OCA Indonesia or Telkom Indonesia.

---

## Author

**Albertus Ariel Renara P**

📧 arielrenara@gmail.com

🔗 LinkedIn: www.linkedin.com/in/ariel-renara

---
⭐ If you find this project interesting, feel free to give it a star!
