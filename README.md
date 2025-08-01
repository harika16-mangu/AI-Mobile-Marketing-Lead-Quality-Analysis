# AI-Mobile-Marketing-Lead-Quality-Analysis

## Data Analyst Case Study: Aarki Lead Quality Analysis
## Overview
This repository contains my solution to a data analyst case study provided by Aarki AI enabled mobile marketing company. 

The project involved analyzing a confidential dataset to understand trends in lead quality and identify opportunities for improvement. The analysis was conducted using Python in Jupyter Notebooks, with findings summarized in a presentation and dashboard.

The primary goal of this case study was to demonstrate a structured approach to a business problem by transforming raw data into actionable insights for various stakeholders, including the CEO, product, and sales teams.

## The Problem: Understanding and Improving Lead Quality

The case study provided a simplified dataset of approximately 3,000 leads sold to an advertiser. Each lead was associated with a specific ad creative and a final CallStatus. The core objective was to analyze the data to answer three key business questions:

Lead Quality Trends: Are there any statistically significant trends in lead quality over time (improving or declining)?

Drivers of Quality: What factors within the dataset (e.g., ad creative, user segments) are the primary drivers of differing lead quality rates?

Strategic Opportunities: Given a hypothetical scenario where the advertiser offers a 20% CPL increase for a 20% improvement in lead quality, what specific opportunities exist within the data to achieve this goal?

## Dataset Description
The dataset, a confidential subset of real-world data, contained information about each lead. Due to its proprietary nature, the raw data is not included in this public repository.

The key fields analyzed were:

Lead Created Date: The date the lead was generated.

CallStatus: The ultimate disposition of the lead, categorized into "good," "bad," and "unknown" quality segments as defined by the advertiser.

Good Quality: Closed, EP Sent, EP Received, EP Confirmed

Bad Quality: Unable to Contact, Contacted - Invalid Profile, Contacted - Doesn't Qualify

Unknown Quality: All other statuses

WidgetName: An internal name for the ad creative that includes details about the ad size, form page layout, design, and color.

## Methodology
My analysis followed a multi-step process to ensure a robust and comprehensive solution:

Data Cleaning & Preparation: The initial step involved loading the dataset into a pandas DataFrame, handling data types, and creating new features to facilitate analysis. This included creating a LeadQuality column based on the CallStatus categories defined in the case study.

Exploratory Data Analysis (EDA): I performed initial high-level analysis to get familiar with the data, identify potential issues, and check for any immediate trends. This step included visualizing the overall distribution of lead quality.

Trend Analysis: To address the first key question, I analyzed the lead quality rates over time, using statistical tests to determine if any observed trends were statistically significant.

Segment Analysis: I segmented the data based on various attributes derived from the WidgetName and other fields to identify drivers of lead quality. For example, I compared lead quality rates across different ad sizes, design variations, and colors to isolate the most impactful factors.

Opportunity Identification: Based on the findings from the segment analysis, I identified specific ad creative segments that demonstrated above-average lead quality. This information was then used to propose a strategy for increasing the overall lead quality by 20%, as requested in the case.

## Key Findings & Recommendations
The analysis led to several key findings and actionable recommendations for the Aarki team:

Time-Based Trends: "Analysis revealed that lead quality has shown a slight upward trend over the observed period, with noticeable peaks in even-numbered months (April, June, August), suggesting cyclical performance patterns, with a close rate of ~11%"

** Primary Quality Drivers: ** 
1. "Partners like Advertise.com and AdKnowledge deliver superior conversion rates (30–35% and 12%+ respectively), highlighting
opportunities for reallocation"
2. "Users with declared debts in the $70K–90K range are the most likely to convert, making them prime candidates for audience targeting
and tailored messaging."​

Strategic Path to Improvement:
1. If we increase the share of leads from high-performing widgets (currently 18% of volume, converting at ~12–15%),​ And scale up lead flow from top partners such as
2. Advertise.com (30–35% quality rate) and AdKnowledge (12%+),​While reducing volume from low-performing creatives and campaigns (under 5% close rate), increases the quality leads ​And concentrating on debt ranges between $70K–90K and high-performing states (OK, HI, CT, MT, AK)​

## Repository Contents

notebooks/Lead Qulaity Analysis: Contains the Jupyter Notebooks used for the data analysis.

presentation/lead_quality_analysis: Includes the slides and notes from the presentation.

README.md: This file, outlining the project.

Technologies Used
Python 3.x

Jupyter Notebook: For interactive data analysis.

pandas: For data manipulation and analysis.

NumPy: For numerical operations.

Matplotlib / seaborn: For data visualization.

SciPy: For statistical analysis.
