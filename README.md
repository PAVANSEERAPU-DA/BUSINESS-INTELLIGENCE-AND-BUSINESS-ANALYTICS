# Energy Company Cost Optimization BI Project

## 📖 Project Overview

[cite_start]This project provides a comprehensive Business Intelligence solution for a regional energy company to address the challenge of high operational costs and improve profitability[cite: 9, 132]. [cite_start]The company, which provides power generation and distribution services, was facing reduced profit margins due to excessive fuel and maintenance expenses and a lack of visibility into key cost drivers[cite: 4, 9, 12].

[cite_start]This solution leverages Salesforce CRM for automated data management and Power BI for advanced visual analytics, enabling data-driven decision-making to enhance operational efficiency[cite: 7, 52, 53].

## 🎯 Business Goals

The primary objectives of this project were to:
* [cite_start]Reduce operational costs by identifying inefficiencies and cost-heavy regions[cite: 17].
* [cite_start]Improve visibility into fuel, labor, and maintenance spending[cite: 18].
* [cite_start]Automate the flagging of high-risk, low-profit operations[cite: 19].
* [cite_start]Enable data-driven decisions through interactive dashboards and analytics[cite: 20].
* [cite_start]Enhance long-term resource planning and cost efficiency[cite: 21].

## 🛠️ Tech Stack & Tools

* **CRM & Automation:** Salesforce CRM
* **Data Visualization & Analytics:** Microsoft Power BI
* [cite_start]**Data Generation:** Python with the Faker library (for mock data generation) [cite: 111]

## 🏗️ Solution Architecture

The system is designed with a two-part architecture:
1.  [cite_start]**Salesforce CRM:** Acts as the central hub for data management[cite: 56]. [cite_start]It captures and validates operational records related to fuel, labor, and maintenance costs across different regions[cite: 57, 147]. [cite_start]Automation features like validation rules and Apex triggers are used to flag inefficiencies in real-time[cite: 70].
2.  [cite_start]**Microsoft Power BI:** Connects to the Salesforce data to provide rich, interactive dashboards[cite: 56]. [cite_start]These dashboards allow stakeholders to visualize cost trends, compare regional performance, and monitor key performance indicators for strategic decision-making[cite: 151, 152, 153].

## ✨ Key Features & Implementation

### Salesforce CRM Implementation

* [cite_start]**Bulk Data Import:** Utilized Salesforce's Bulk API to efficiently load over 199 operational records, ensuring scalable and accurate data entry[cite: 167, 187].
* [cite_start]**Validation Rule for Loss Detection:** A rule named `High_Cost_Low_Output_Loss_Detection` was created to automatically flag records with high costs (>$60,000), low energy output (<200,000 kWh), and negative profit, enabling rapid identification of underperforming assets[cite: 157, 191, 192].
* [cite_start]**Apex Trigger for Maintenance Flags:** A custom Apex Trigger, `FlagHighCostEnergyRecords`, automatically flags records requiring "Unplanned Maintenance" review based on high-cost and negative-profit conditions, improving responsiveness and aiding in preventive planning[cite: 163, 196, 198].
* [cite_start]**Filtered List Views:** Customized list views allow teams to filter and analyze data by region, helping to localize decision-making and identify area-specific trends[cite: 170, 202].

### Power BI Dashboards & Analysis

Three key dashboards were developed to address business needs:

1.  [cite_start]**Operational Cost Analysis:** Provides a detailed breakdown of expenditures by region and cost type (fuel, labor, maintenance)[cite: 207].
    * [cite_start]**Insights:** The West and South regions have the highest operational costs and a higher average of unplanned maintenance, suggesting an area for focused improvement[cite: 213, 215].
2.  [cite_start]**Consolidated Overview:** Offers a high-level summary of total spending across all categories[cite: 219].
    * [cite_start]**Insights:** Fuel cost is the largest operational expense, totaling **$478.77M**, making fuel efficiency the highest-impact area for cost savings[cite: 225, 229]. [cite_start]The West region accounts for the largest share of total costs (25.56%)[cite: 226].
3.  [cite_start]**Cost Analysis Page:** Focuses on tracking cost trends over time to evaluate the effectiveness of control measures[cite: 231].
    * [cite_start]**Insights:** A gradual downward trend in monthly fuel costs was identified (from $43M to $37M), indicating early signs of successful cost control[cite: 237, 240].

## 📊 Database Design

[cite_start]The system's database schema was designed with five key entities to track operational costs, maintenance, and alerts effectively[cite: 78].

* **Entities:**
    1.  [cite_start]`Region`: Stores details for each operational region (North, South, East, West)[cite: 79].
    2.  [cite_start]`OperationalRecord`: Captures monthly data on energy output and costs[cite: 80].
    3.  [cite_start]`MaintenanceLog`: Tracks planned vs. unplanned maintenance activities[cite: 81].
    4.  [cite_start]`CostAlert`: Flags records with high costs and low output[cite: 82].
    5.  [cite_start]`MonthlyReport`: Aggregates data for monthly dashboard reporting[cite: 83].

## 💡 Conclusion & Impact

[cite_start]This integrated solution successfully equipped the energy company with the tools to gain control over its operational costs[cite: 272]. [cite_start]By combining Salesforce's automation with Power BI's analytics, the company can now identify cost drivers, detect inefficiencies in real-time, and make informed, data-driven decisions to improve profitability and long-term efficiency[cite: 273, 275].

## 🚀 Future Work

To further enhance the system, the following steps are recommended:
* [cite_start]Integrate predictive analytics to forecast cost spikes and maintenance needs[cite: 278].
* [cite_start]Incorporate IoT data from equipment to monitor real-time performance and fuel usage[cite: 279].
* [cite_start]Automate the distribution of scheduled Power BI reports to relevant departments[cite: 280].
* [cite_start]Expand the CRM to track other key metrics such as environmental impact and energy savings[cite: 282].
