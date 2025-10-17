# State-Level-Analysis-of-Health-Issues-Hospital-Availability-and-Healthcare-Quality-in-the-U.S.
All team members: Suji Kim, Anna Baldzikowski, Linh Le, Shi Qiu, Tianqi Sun, Xiaoyan Wang.

Overview

This project examines state-level healthcare for older adults by linking three sources: CDC Healthy Aging indicators, the U.S. Hospital Directory, and CMS Nursing Home Ratings. We measure access, quality, and outcomes, then visualize regional patterns and priority issues to support practical policy and operations decisions.

Data

CDC Healthy Aging: state indicators including physical and mental health and screenings.
U.S. Hospital Directory: hospital counts, types, and beds.
CMS Nursing Home Ratings: Overall, Quality Measure, and Staffing.

All datasets were cleaned and merged on StateCode; basic missing value handling and column standardization are documented in the notebook.

Methods

Descriptive EDA and schema profiling.
Access metrics such as hospitals and beds per 1,000 older adults.
Ranked “top issue by state” and topic mapping across conditions.
Regional analysis of screenings with choropleth maps.
Scatter and box plots to relate ratings to outcomes.
Simple regressions to test relationships between access, quality, and outcomes.

Highlights from Results

Access: Long-term care availability varies widely; Texas ranks high, while several western and rural states are lower.
Quality vs outcomes: Higher quality and staffing ratings align with better self-reported health.
Weak access–outcome linkage: Simple regressions show very low explained variance when using facility quantity alone, indicating that capacity by itself does not predict outcomes.
Preventive care: Cholesterol screening is the most frequent issue flagged under Physical Health and Medical Conditions. Screening levels remain high overall but differ by region, with noticeable drops in specific time windows in the Northeast and persistently lower rates in parts of the West.
Regional distributions: Box plots show WEST and NRE with higher shares of good to very good physical health, MDW in the middle, and SOU more mixed.

Implications

Improve workforce quality and staffing to raise overall performance.
Target outreach where screenings lag and support with practical access options such as telehealth.
Address low-access states with selective capacity investments and regional partnerships.
Monitor quality and access together rather than relying on facility counts alone.

How to Reproduce

1. Open the notebook in Jupyter or Google Colab.
2. Run all cells in order. No local dataset upload is required. The notebook pulls:

· Health.csv from Health.csv.zip
· Hospitals.csv
· Ratings.csv
  via GitHub raw links defined at the top of the notebook.

If you fork this repo or move files, update the three URL constants (HEALTH_URL, HOSP_URL, RATINGS_URL) in the first data import cell.

Limitations and Next Steps

Add socioeconomic controls to reduce omitted variable bias.
Extend the time horizon to study trends and shocks more precisely.
Validate with additional provider-level and rural–urban breakdowns.

Team
Suji Kim, Anna Baldzikowski, Linh Le, Shi Qiu, Tianqi Sun, Xiaoyan Wang
