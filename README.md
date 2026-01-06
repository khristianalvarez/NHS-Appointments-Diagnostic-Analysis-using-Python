# NHS Appointments Diagnostic Analysis

### Topics Covered:

Data Wrangling, Data Visualisation with Python (Plotly, MatPlotLib, Seaborn), API calling, Web Scraping, Natural Language Processing, and Sentiment Analysis.

#### Grade: *Distinction*

## Executive Summary

This report analyses NHS appointments from January 2020 to June 2022 to answer two operational questions posed by the organization: whether there has been adequate staff and capacity across its networks, and how effectively existing resources have been utilized. Results show a balanced distribution of workload between GPs and other practice staff, a consistently high-capacity utilization, and opportunities to reduce inefficiencies from missed appointments – particularly those booked 2 to 7 days in advance. Public sentiment analysis of healthcare-related commentaries online, particularly Twitter, further provides context on these findings, highlighting prominent discussions on staffing, digital health, and AI in healthcare. 

## Objectives

This analysis was commissioned to deliver data-driven answers to two core NHS operational questions: (1) whether staffing levels and capacity have been sufficient across the networks, and (2) how resources have actually been utilized. The intent aims not only to measure current performance but also generate actionable insights that can strengthen operational resilience and enhance patient care delivery. This report highlights the technical process of the analysis, with emphasis on methodological transparency and the rationale for analytic decisions.


## Data Acquisition and Preparation

Three main data sets formed the backbone of this analysis: the NHS appointment data segmented by healthcare professional type, service setting, and appointment status; the NHS appointment data by context type and national service category; and auxiliary data from Twitter containing healthcare related hashtags that offer an external lens on the public and professional discourse on the matter. Data preparation involved integrating data sets of different granularities (daily and monthly) into a consistent framework, cleaning and standardizing category labels, removing duplicates, handling missing data, and aligning appointment metrics for compatibility across sources.


## Analytical Approach

The analysis applied a structured-multilayered methodology. Trends over time were assessed to observe shifts in workload distribution between GPs and other staff, while monthly capacity utilization was measured to identify sustained pressures or available capacity. Attendance and Did-Not-Attend (DNA) rates were segmented by booking lead time to pinpoint areas of inefficiency, and seasonal and regional variations were assessed to reveal shifts in service demand. Consequently, the frequency of healthcare-related hashtags on Twitter was analyzed to identify public discourse relevant to the NHS operations.


## Insights

### *Adequate Staff and Capacity*

The analysis shows that staffing levels remained largely stable, with a gradual shift in workload balance emerging after mid-2021 as GPs and other practice staff began delivering similar appointment volumes. The “Appointments Over Time by HCP Type” chart below showed a strong recovery from the early pandemic dip, while the “% Share of Monthly Appointments by HCP Type”  demonstrated a consistent division of labor, with GPs handling roughly 37-39% and other staff at 40-42% of appointments.


<img width="468" height="232" alt="image" src="https://github.com/user-attachments/assets/ca369cfa-f7eb-4f77-beb4-e834206b12fe" />

<img width="468" height="231" alt="image" src="https://github.com/user-attachments/assets/b4a20830-b418-4643-aded-63779b1d2ee8" />


The “Appointments per Month by Service Setting” confirmed General Practice (GP) as the main service provider, with Primary Care Networks and Extended Access Provision steadily contributing. 


<img width="468" height="324" alt="image" src="https://github.com/user-attachments/assets/028b1910-dbf6-4434-9377-d7d610b86dee" />


Non-GP settings displayed stable appointment volumes, except for high variability in unmapped data. 


<img width="468" height="231" alt="image" src="https://github.com/user-attachments/assets/24199a32-b28f-4cdb-89b6-3ecddad86768" />


Capacity Utilization also remained high at 94-97% peaking during lockdown, while regional attendance rates were robust at 94% to 96.5%.


<img width="468" height="218" alt="image" src="https://github.com/user-attachments/assets/9aed2668-cd0d-4966-bb86-78fb6e37b801" />



<img width="468" height="472" alt="image" src="https://github.com/user-attachments/assets/7dc378ad-67cf-4363-8077-8bca8fbe9c5e" />


Overall, staffing and capacity were sufficient to meet demand but allowed little margin for unplanned and unexpected surges. 


### *Utilization of Resources*

Resource utilization was strong with appointment slots consistently above 94% usage as shown in the following capacity utilization chart above. Therefore, resource use was efficient with most appointment slots filled. 

The “% Share of Appointment Status Over Time” showed over 90% attendance rates, with Did-Not-Attend (DNA)’s averaging only about 5%.


<img width="409" height="291" alt="image" src="https://github.com/user-attachments/assets/2f340e95-00ec-46ef-8abe-d2f3fbbd2d71" />


The “Missed Appointments by Booking Lead Time” chart also highlighted that most missed appointments were booked 2 to 7 days in advance – a key opportunity for intervention.


<img width="431" height="247" alt="image" src="https://github.com/user-attachments/assets/0f04011c-dcd2-4178-a903-80c76139a58c" />


Booking patterns also relied heavily on same-day and short lead times. 


<img width="468" height="232" alt="image" src="https://github.com/user-attachments/assets/fb67ecf1-348a-4cfb-b3cc-467d38341828" />


The “Appointment per Month by Context Type” identified Care Related Encounters as the majority of the activity, with a balanced mixed of routine and urgent care as show in the “Top 5 National Categories” chart.


<img width="417" height="287" alt="image" src="https://github.com/user-attachments/assets/f3bb8055-82e4-4a80-b522-d25148841527" />

<img width="468" height="247" alt="image" src="https://github.com/user-attachments/assets/ac0fe81c-3688-4472-9be8-8d45bc449907" />


Seasonal analysis also revealed General Practice (GP) dominating all year, with slight seasonal shifts but no major underutilization. 


<img width="468" height="231" alt="image" src="https://github.com/user-attachments/assets/c8b67bfa-0e51-46d8-b02d-977527295667" />


Overall capacity remained high, with expected peaks in winter months.


### *Public Sentiment*


Twitter hashtag trends positioned #healthcare as the most prevalent topic, with notable engagement around #AI, #telehealth, and workforce related tags such as #nurses and #hiring. These aligns with operational findings, reflecting public awareness of staffing pressures and the growing interest in digital health solutions.


<img width="468" height="374" alt="image" src="https://github.com/user-attachments/assets/91470ef3-0b70-4313-8886-4ccb479d5fab" />


## Discussion

From a technical perspective, NHS is achieving strong efficiency converting available capacity into delivered care. However, consistently high utilization leaves little margin to absorb sudden increases in demand. The Did-Not-Attend (DNA)  analysis points directly to the 2 to 7 day booking window as a key operational weakness, suggesting scope for improved reminders and simplified cancellation systems. The Public Sentiment analysis also reinforces these operational findings and identifies opportunities for engagement, particularly around digital-first care pathways.


## Recommendations

It is recommended that the NHS should optimize appointment durations  to case complexity, increase seasonal capacity planning, and dynamically allocate workforce to meet regional demand variations. Resilience can be strengthened through rapid-response teams and cross-training staff to manage surges, while patient access should be enhanced by expanding urgent slots, refining referrals, and optimizing online booking. Reserving emergency slots will also help prevent overload, and leveraging public sentiment in promoting telehealth and alternative health care options can further improve efficiency.


## Further Analysis


Future analysis could incorporate predictive modelling to anticipate demand surges, enabling a more proactive resource allocation. A root cause analysis of overutilization will also help identify underlying operational pressures and guide targeted interventions. Consideration of the impact of seasonal trends and external factors could also provide valuable context for capacity planning. Consequently, regional performance benchmarking could highlight best practices, while a more detailed examination of the factors behind missed appointments could inform strategies to improve attendance rates.



### *---Complete diagnostic analysis on Jupyter Notebook attached above---*











