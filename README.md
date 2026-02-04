# Driver-Risk-Assessment-using-Big-Data-Analytics
This project analyses truck telematics data to identify risky driving patterns and fuel inefficiencies, and built dashboards to support safer, more cost-effective fleet operations.

Dataset

There are three files in the original dataset:
1. geolocation: This outlines driver details along with geolocation details such as latitude, longitude, state, etc.
2. trucks_mg: This gives information on iles driven and gas consumed by the driver
3. trucks: This gives information on the truck model along with miles and gas consumed every month

Important research questions

Problem 1: We are identifying and analyzing abnormal driving behavior such as unsafe tail distance, lane departure, and idling by using truck event data. The goal is to improve safety and monitor risky driving patterns in real time.

Problem 2: We want to identify which trucks are fuel-inefficient and which trucks are most likely to need maintenance, so we can reduce fuel cost and  avoid breakdowns.

Problem 3: We analyze telematics events to find which drivers show risky behavior.
Goal: identify unsafe patterns, top risky drivers, and behaviors that need coaching.

Problem 4: We calculate how well each driver performs based on safety behavior, fuel efficiency, and total events. The goal is to identify top drivers and those needing coaching.

Tools

1. HDFS – Stored the geographic and truck fleet data for processing in a distributed environment.
2. Hive – Created tables and loaded the truck and geolocation data for querying and analysis.
3. Impala – Ran real-time SQL queries on Hive tables to extract driver risk factors efficiently.
4. PySpark – Processed and enriched truck fleet data, calculated risk factors, and prepared datasets for visualization.
5. Tableau – Built dashboards to visualize driver risk factors and highlight those exceeding the threshold.

Insights

1. The riskiest event type is unsafe following distance. 
Recommendation:  Higher-risk drivers travel during off-peak hours to reduce exposure to dense traffic and lower the likelihood of avoidable collisions.
2. 14 trucks carry an elevated Maintenance Risk Score. 
Recommendation: Prioritize inspections and preventative maintenance for the low MPG, high risk trucks.
3. Identify both top-performing and underperforming drivers. 
Recommendation: Reward high-performing drivers, while implementing structured corrective actions for underperforming drivers to ensure accountability and improvement.
4. By comparing Performance Score with Risk Score, we found that drivers with higher risk scores consistently perform worse overall, reinforcing the connection between unsafe driving behaviors and reduced performance.



