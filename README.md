# Breast-Cancer-Referral-Network-Analyis

## Overview

This report examines the network of healthcare facilities that provide breast cancer care across the United States. Using IQVIA Claims, geospatial and capacity data, the analysis focuses on the structure and robustness of the referral system, encompassing primary care providers, cancer centers, and specialized hospitals. The study evaluates connectivity, shortest path lengths, and resilience under stress scenarios to identify gaps and opportunities for improvement.

## Key Findings

Network Characterization

1. Degree Distribution

	•	Cancer Centers:
	•	Highest Degree: Urban regions, such as New York and California, have the highest mean degrees due to centralized care networks.
	•	Outliers: Regions with centralized hubs like MD Anderson in Texas or Sloan Kettering in New York show significantly higher degrees.
	•	Primary Care Providers (PCPs):
	•	PCPs in rural areas often rely on a limited number of referral centers, resulting in lower mean degrees compared to urban counterparts.

2. Shortest Path Analysis

	•	PCPs → Cancer Centers:
	•	Shortest paths are lowest in densely populated areas like the Northeast and urban West Coast.
	•	Longest paths are found in rural Midwest and Southern regions.
	•	Cancer Centers → Specialized Hospitals:
	•	Urban hubs have shorter paths (e.g., New York, California) compared to regions with sparse specialized facilities, like the Mountain West.

Simulated Stress Scenarios

Simulation Details:
- Modeled the impact of increased patient volumes (0.001% to 1% of the population) on the referral network, simulating breast cancer diagnosis surges.
- Assessed isolated PCPs and overloaded cancer centers under different stress levels.

Results:
**Remaining Operational Cancer Centers:**
- Urban areas show higher resilience, with hubs like California and New York retaining 30% of operational cancer centers at 0.5% patient load.
- Rural regions such as the Midwest see sharp declines, retaining less than 10%.

**Isolated PCPs:**
- At 0.05% population load, rural states like Montana and Wyoming see up to 70% of PCPs isolated due to limited referral options.
- By 0.5%, nearly all PCPs in rural areas lose connectivity.

## Summaries

Degree Distribution by Region

- Urban hubs (e.g., New York, California, Texas):
- Cancer centers show high connectivity with a large number of PCPs referring patients to them.
- Rural regions (e.g., Midwest, Appalachia):
- PCPs have limited connections, leading to low redundancy in the referral network.

Shortest Path Analysis

**Urban regions:**
- Shortest paths highlight efficient access to specialized care due to higher facility density.
**Rural regions:**
- Longer paths reflect challenges in accessing cancer care, exacerbating treatment delays.

Impact of Stress on Network

- Regions like New York and California exhibit resilience under stress, retaining significant portions of operational cancer centers.
- Rural areas like the Midwest and Mountain West experience rapid degradation in network functionality under stress.

Recommendations

1. Expand Rural Access:
   Invest in more cancer centers or satellite facilities in rural regions to improve connectivity and reduce reliance on urban hubs.
2. Enhance Referral Efficiency:
   Develop telehealth and centralized referral systems to streamline patient transfers and ensure optimal use of available facilities.
3. Simulate Regional Stress:
   Employ simulation models to identify specific vulnerabilities in underserved areas and proactively mitigate risks.
4. Improve Rural-Urban Referral Networks:
   Strengthen rural-urban partnerships by increasing capacity at rural PCPs and streamlining transport to urban hubs.

Summary Data

| Region       | Max Cancer Center Degree | Mean Path (PCP → Center) | % Remaining Centers (0.5% pop) | % Isolated PCPs (0.5% pop) |
|--------------|---------------------------|---------------------------|--------------------------------|----------------------------|
| New York     | 85                        | 12.34                    | 35.00                         | 15.00                     |
| California   | 90                        | 10.45                    | 40.00                         | 10.00                     |
| Midwest      | 25                        | 25.67                    | 10.00                         | 75.00                     |
| Appalachia   | 20                        | 20.45                    | 5.00                          | 90.00                     |

# Conclusion

This report underscores the disparities in access to breast cancer care across the United States. While urban hubs demonstrate resilience and high connectivity, rural areas face significant challenges, with limited facilities leading to higher isolation rates and longer paths to specialized care. Strategic investments in infrastructure and referral efficiency are critical to improving outcomes and ensuring equitable healthcare access.
