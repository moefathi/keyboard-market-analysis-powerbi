# Keyboard Market Analysis – Power BI

## Project Overview
In this project, I worked on a data science solution for City Center, a computer store in Jordan that wants to introduce three mechanical gaming keyboards into the market: Razer Huntsman, HyperX Alloy, and Redragon K552P.

The main goal was to analyze historical market data to understand customer demand, compare the performance of the three keyboards, study the relationship between price and demand, and predict future demand to support City Center's decision-making process.

I worked on the project as part of NextStep Solutions, where I was responsible for collecting and preprocessing the data, performing analytical and predictive analysis, creating visualizations, and providing recommendations based on the results.

## Project Objectives
The main objectives of this project were:

- Analyze historical demand and performance for the three keyboards.
- Compare the brands based on their sales rank and demand.
- Understand the relationship between prices, discounts, and customer demand.
- Forecast future performance and demand for the next 12 months.
- Identify the most suitable keyboards for market entry.
- Provide recommendations about pricing, stock inventory, and the best time to introduce each keyboard.

## Data Collection
I used Helium, an e-commerce data collection tool, to collect historical Amazon data for the three keyboards. The collected data included:

- Sales Rank
- New Price
- List Price
- Time Records

The original datasets started from different dates and contained some missing values, so I prepared the data before starting the analysis.

## Data Preprocessing and Cleaning
I used Power BI and Power Query Editor to clean and prepare the collected datasets. This included:

- Removing errors from selected columns.
- Removing empty rows and handling missing values.
- Selecting 1 January 2023 as the starting date for the analysis.
- Adding columns and measures required for the analysis.
- Converting prices from USD to JOD because City Center is located in Jordan.

I also created additional columns to make the analysis easier to understand and more useful for business decisions:

| Column | Description |
|---|---|
| Brand | Specifies the keyboard brand. |
| Brand_ID | Unique ID to identify each brand. |
| Demand | Demand level based on sales rank: High, Medium, or Low. |
| Demand Score | Numerical demand level: High = 3, Medium = 2, Low = 1. |
| New Price (JOD) | Selling price converted to Jordanian dinars. |
| List Price (JOD) | Original listed price converted to Jordanian dinars. |
| Discount (JOD) | Difference between the new price and list price. |

I also created measures to calculate the average demand score and rank the keyboards based on their average demand score.

## Data Analysis and Forecasting
After preparing the data, I used Power BI to perform analytical and predictive analysis.

For the predictive analysis, I used the forecasting feature in Power BI to predict future sales rank for each keyboard. I also compared actual sales rank with forecasted sales rank by ignoring the last 11 months to evaluate the forecasting performance.

The analysis focused on historical performance, customer demand, brand strength, pricing, discounts, and future demand.

## Power BI Dashboards
I created interactive dashboards in Power BI to present the results and make the analysis easier to understand for City Center's sales team and decision makers.

The dashboards include:

- Customer demand comparison between the three keyboards.
- Average demand score and keyboard ranking.
- Historical sales rank comparison over time.
- Future sales rank forecasting for each keyboard.
- Average new price by demand score.
- Average new price and sales rank over time.
- Discount effect on customer demand.
- Summary cards showing average sales rank, new price, demand score, and discount.
- Interactive slicers to explore the data.

I also used demand levels and scores to make the results easier to understand, instead of relying only on sales rank.

## Findings and Recommendations
After analyzing the results, I identified the following performance ranking:

1. **Razer Huntsman:** Achieved the strongest demand performance, the lowest average sales rank, and more stable demand compared to the other keyboards.
2. **HyperX Alloy:** Showed moderate performance and demand, ranking second overall.
3. **Redragon K552P:** Showed the weakest historical demand and stability, although its demand showed some improvement during 2025.

Based on the analysis, I recommended that City Center introduce Razer Huntsman first because of its strong and stable demand. HyperX Alloy could be introduced as a second option while monitoring its initial sales. For Redragon K552P, I recommended delaying its introduction until its demand becomes clearer.

I also recommended using discounts mainly during periods of low demand, as the analysis showed that brand strength had a stronger influence on demand than price alone.

For inventory planning, Razer Huntsman should receive a higher stock allocation, while HyperX Alloy and Redragon K552P should initially have lower stock allocations based on their performance and forecasting results.

## Limitations and Future Improvements
Although the solution provided useful insights for City Center, there were some limitations:

- The analysis relied on Amazon data, which may not accurately represent the behaviour of customers in the Jordanian market.
- The forecasting wizard in Power BI was not the most advanced forecasting method and could produce negative predicted values.
- The analysis focused mainly on sales rank and price, while other factors such as customer ratings and seasonal gaming events could also affect demand.

In the future, the solution could be improved by collecting data from the Jordanian market, including additional factors in the dataset, and using stronger forecasting methods with Python or R.


## Technologies and Tools
- Power BI
- Power Query Editor
- DAX
- Helium

## Project Information
- **Project Type:** Academic Project
- **Course:** Business Process Support
- **Semester:** Fall 2025–2026

## License
© 2026 Mohammad Aldeghemat. All rights reserved.

