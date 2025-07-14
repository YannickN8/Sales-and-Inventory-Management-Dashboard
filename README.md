Title:  Furniture Sales and Inventory Management 


Executive Summary

In the dynamic retail landscape, effective inventory management is critical to achieving customer satisfaction and operational efficiency. This project leverages predictive analytics to address key inventory challenges, including overstock and stockouts. By analyzing demand patterns and implementing data-driven forecasting models, the study aims to enhance inventory turnover, optimize stock levels, and improve supply chain efficiency. These efforts have the potential to yield substantial revenue growth, minimize holding costs, and maximize profitability across all product categories.
<img width="1600" height="914" alt="01_Executive Summary" src="https://github.com/user-attachments/assets/8fa3df2d-7ad2-4091-8943-ea8c8db9a08e" />

 
 





Background
Efficient inventory management directly impacts the profitability and sustainability of retail operations. Overstock leads to increased storage costs and wasted resources, while stockouts cause lost sales and diminished customer loyalty. With 43% of small businesses struggling to balance inventory levels, the need for advanced forecasting methods has never been greater. This project addresses these challenges using data-driven techniques to predict demand, optimize inventory levels, and enhance operational efficiency.
<img width="1024" height="585" alt="02_Background" src="https://github.com/user-attachments/assets/0338c4dc-96cc-4e08-939c-936864424a06" />

 

Problem Statement
Retailers face significant challenges in maintaining optimal inventory levels. Overstock results in excessive carrying costs, while stockouts lead to missed revenue opportunities and dissatisfied customers. Addressing these issues requires a predictive approach to understand demand patterns and align inventory management with business needs.
<img width="1600" height="914" alt="03_Problem Statement" src="https://github.com/user-attachments/assets/ce0022fe-5f55-4d42-aafc-0fcbb87e7923" />

 

Objectives
•	Develop predictive models to accurately forecast product demand.
•	Optimize inventory levels to prevent stockouts for high-demand products.
•	Reduce carrying costs for low-demand products by identifying overstock risks.
•	Enhance decision-making through actionable insights derived from analytics.
•	Improve overall supply chain efficiency and profitability.
 <img width="1600" height="914" alt="04_Objectives" src="https://github.com/user-attachments/assets/fc1c7f09-7834-47f2-916b-e7e524abc7f3" />

 

Data Overview

Data Sources
 The data for this study was sourced from multiple channels, including Kaggle for comprehensive datasets, internal inventory management records for detailed operational insights, and external market statistics for benchmarking and validating performance metrics. These diverse sources provided a robust foundation for analyzing and optimizing inventory management practices.
 <img width="1600" height="914" alt="05_Data Source" src="https://github.com/user-attachments/assets/0d393b6e-3a3d-40e5-abb7-b58857a91195" />















System Architecture
The project integrates Microsoft Fabric with Power BI for data visualization and reporting. Predictive models are built using Python and Spark for scalable data processing.
 <img width="1600" height="915" alt="06_System Architecture" src="https://github.com/user-attachments/assets/de4e0608-0430-40c5-92d7-684726339ce1" />



Data Features
The dataset included a variety of features critical for analyzing inventory performance.
•	Independent Variables: Inventory Level, Sales, Cost of Goods Sold
•	Dependent Variables: Inventory Turnover Rate, Stockout Rate
•	Calculated Metrics: Excess Inventory, Sales Growth
 <img width="1600" height="914" alt="07_Data Model" src="https://github.com/user-attachments/assets/a68d8bd8-b2ea-4319-8863-b1af781dad5e" />















Methodology

Data Preparation:
Clean and aggregate inventory and sales data for analysis, ensuring accuracy by removing duplicates and handling missing values.
 <img width="1600" height="915" alt="08_Data Preparation" src="https://github.com/user-attachments/assets/3da6e42b-d3bf-4489-b8b6-7542db372766" />

 





Model Selection:
XGBRegressor was selected as the optimal model for this inventory management project due to its ability to handle complex relationships between variables and its strong predictive performance. This model demonstrated an R² (Coefficient of Determination) value of 0.8, indicating that it explains 80% of the variance in demand, a robust indicator of its effectiveness in capturing the relationships among the independent variables such as Order Date, Sales, and Quantity. 
 
<img width="1600" height="914" alt="09_Model Selection" src="https://github.com/user-attachments/assets/881c0eb4-cf69-4564-a891-217a89d4f791" />



Model Development:
 The XGBRegressor model was trained and fine-tuned using historical inventory and sales data. The model's parameters were optimized to enhance its ability to predict demand while minimizing errors. Key independent variables were carefully selected to ensure a balance between predictive accuracy and computational efficiency. The model's development involved iterative testing to improve its fit to the data, providing a reliable tool for forecasting demand.
<img width="1600" height="915" alt="10_Model Development" src="https://github.com/user-attachments/assets/195e8d0f-ee0e-4cef-9d27-b4d47df15820" />

 


Results

Model Performance
The XGBRegressor achieved strong performance metrics, affirming its reliability for this project. The Mean Squared Error (MSE) of 1.1 reflects a low average squared difference between predicted and actual values, while the Mean Absolute Error (MAE) of 0.8 indicates the model's predictions are, on average, 0.8 units away from the actual demand. Additionally, the Median Absolute Error of 0.6 highlights the model's robustness, showing that half of the errors fall below this value. These metrics, coupled with a variance of 0.8, underscore the model’s accuracy and consistency in forecasting demand.

The adoption of the XGBRegressor model equips supply chain and operations teams with actionable insights for demand forecasting, helping to reduce stockouts and excess inventory. This predictive capability supports better decision-making, optimized stock levels, and enhanced fulfillment of customer demand, leading to reduced costs and improved operational efficiency.
<img width="1600" height="914" alt="11_Model Performance" src="https://github.com/user-attachments/assets/8d379d58-2a4a-45c4-953f-2a5ddc99a211" />


 
 
Visualizations

The Power BI dashboard provides a comprehensive overview of furniture sales and inventory performance between 2014 and 2017. Key metrics such as total sales, inventory turnover rate, stockout risk, and excess inventory are highlighted, offering actionable insights. Visualizations include trends in total quantity sold over time, profit analysis by sub-category, and regional forecast accuracy. The dashboard also emphasizes inventory efficiency, showcasing relationships between turnover rates, days of inventory, and quantity sold across segments and sub-categories, enabling better inventory optimization strategies.
<img width="1600" height="914" alt="12_DASHBOARD" src="https://github.com/user-attachments/assets/74e030db-1f98-41ba-897c-1112635e9e80" />

  ![13_DASHBOARD_Gif](https://github.com/user-attachments/assets/90c3fb84-badd-4e83-91ba-5164202211aa)


Case 1 Objective: Optimizing high-sales products by preventing stockouts.

Positive Insight:
•	The Table sub-category has high-sales products with low inventory, averaging $1,764.35 in sales. This indicates their popularity and highlights the risk of stockouts. 
 <img width="1600" height="914" alt="14_Case 1_ Optimizing High Sales Prducts by Preventing Stockouts (Positive Insight)" src="https://github.com/user-attachments/assets/16c2dc2d-0948-4dc7-8466-e3511cf667da" />

 

Negative Insight:
•	The Furnishings sub-category has 38 products at risk of stockout with inventory levels below 100 units. This vulnerability to stockouts could lead to potential revenue loss and disrupt customer loyalty. 
 <img width="635" height="356" alt="15_Case 1_Negative Insight" src="https://github.com/user-attachments/assets/e098eac6-793a-49ec-a390-aa35e333f374" />

Internet Stat
This chart is a visual representation of how stockouts can drastically impact inventory metrics, highlighting the need for proactive stock management to prevent these challenges.
https://www.eazystock.com/blog/avoid-stockouts-better-inventory-management-how-to/
 
This graph shows the potential projected sales growth when a 15% improvement in demand forecasting accuracy is achieved.
 <img width="1600" height="914" alt="16_Case 1_ Internet Stat" src="https://github.com/user-attachments/assets/5dfd2bad-9dee-4707-ba11-3a88da4a9d64" />

 

Return on Investment:
A 15% improvement in demand forecasting is expected to yield an additional $7,104.65 in revenue. In the Tables sub-category, improved forecasting could increase revenue by $264.65, while in Furnishings, 38 items at risk of stockout could contribute $6,840 with improved forecasting. This demonstrates the revenue potential of proactive inventory management for high-demand products. 
<img width="1600" height="914" alt="17_Case 1_ Return on Investment" src="https://github.com/user-attachments/assets/11f84b9c-e85f-448f-9600-0c358e18103b" />

Case 2 Objective: Reducing excess inventory for low-demand products.

Positive Insight:
•	 The Bookcases sub-category has low sales and high inventory, averaging $183.37 in sales, indicating potential overstock. Adjusting stock levels could free up space and resources for higher-demand items, improving inventory efficiency.
 <img width="1600" height="914" alt="18_Case 2_Reducing excess inventory for low-demand products (Positive Insight)" src="https://github.com/user-attachments/assets/2fdc2eb3-3ec4-4e1b-88e8-469281ec815e" />


Negative Insight 
•	 The Chairs sub-category has 8 products holding in excess of inventory above 400 units, indicating a supply-demand imbalance. This surplus can lead to higher storage costs and markdowns. . 
 <img width="1600" height="914" alt="19_Case 2_Negative Insight" src="https://github.com/user-attachments/assets/dbd49e90-a485-42ba-a3f3-d8d1beecef44" />

internet stat
This bar chart visually represents how implementing targeted strategies to reduce excess and obsolete inventory can positively impact sales. https://nventic.com/insights/ultimate-guide-to-reducing-excess-and-obsolete-inventory/
<img width="470" height="296" alt="20_Case 2 Internet Stat" src="https://github.com/user-attachments/assets/ad04cf79-0042-496a-8b63-2d8c60eacc1e" />

 

Return on Investment:
By reducing 10% of excess inventory holding costs, the company could save an estimated $12,458.43. Savings for bookcases would be around $458.43, while the chairs sub-category could reduce costs by $12,000 due to surplus inventory. This adjustment frees up capital for higher-demand products, improving cash flow and inventory efficiency. 

Case 1 and Case 2 Comparison
 <img width="454" height="272" alt="21_Cases Comparison" src="https://github.com/user-attachments/assets/22d33292-c2d9-48e7-8e23-aec875b5ad98" />

 
Summary:
The graph illustrates two key inventory optimization strategies with significant potential for both revenue growth and cost efficiency. Case 1 focuses on preventing stockouts for high-demand items, projecting a 15% increase in forecasting accuracy that could translate into a substantial revenue boost, potentially enhancing overall sales by a similar percentage across popular product lines. Case 2 addresses low-demand products with excess inventory, achieving a 10% reduction in holding costs, which not only saves storage expenses but also frees up capital to invest in high-demand products.

Together, these strategies present a holistic approach to inventory management by maximizing sales opportunities while minimizing carrying costs. 

Impact

Solution Impact
By implementing a comprehensive inventory optimization strategy, organizations can significantly enhance their financial performance. This approach involves preventing stockouts of high-demand products to maximize sales and reducing excess inventory of low-demand items to minimize carrying costs. This balanced strategy optimizes resource allocation, improves cash flow, and ultimately strengthens the organization's market position.
 <img width="1600" height="915" alt="22_Solution Impact" src="https://github.com/user-attachments/assets/73bfd1f8-77a6-4805-9d5f-2f758d43bba6" />

 
Business Outcomes
•	Increased revenue opportunities for high-demand products.
•	Significant savings from reduced carrying costs for low-demand items.
•	Improved cash flow and inventory efficiency.
•	Improved inventory turnover rate across all categories.
•	Reduced stockout risks for high-demand items.
•	Freed up capital by addressing overstock in low-demand products.
<img width="1600" height="915" alt="23_Business Outcome" src="https://github.com/user-attachments/assets/0c306fd9-7a25-45be-a610-a3c702d32986" />

 
Key Achievements
 
<img width="1600" height="915" alt="24_Key achievements" src="https://github.com/user-attachments/assets/ebd52584-33c9-4790-9bf6-22fb787ded9f" />



Lessons Learned and Future Work

Challenges and Solutions:
•	Data Quality Issues: The initial dataset required significant cleaning and validation to address redundancy, inconsistencies, and incompleteness.
•	Data Acquisition: Additional data was necessary to obtain a comprehensive understanding of the inventory.
•	DAX Formula Refinement: Certain DAX formulas required adjustment to ensure accurate results.
•	Visualization:  Some visualizations were not suitable for conveying insights.  Appropriate visualizations were crucial for effective communication of insights 
 <img width="1600" height="914" alt="25_Challenges and Solutions" src="https://github.com/user-attachments/assets/5a90265f-0d18-4cf8-abe0-b25f815a6983" />

 
Lessons Learned:
•	Data Quality: We encountered initial challenges with data redundancy, inconsistencies, and incompleteness. These were overcome through a rigorous cleaning and validation process.
Data Acquisition: The initial dataset was insufficient for a comprehensive understanding. We addressed this by acquiring supplementary data from various sources.
Model Optimization: Certain DAX formulas needed refinement to guarantee accurate results. We achieved this through iterative testing and adjustments.
Visualization Clarity: Effective communication of insights hinged on appropriate visualizations. Refining these visuals ensured clear understanding of the data.
 <img width="1600" height="915" alt="26_Lessons Learned" src="https://github.com/user-attachments/assets/4b13c133-8a2f-41ac-a924-7ec79d3419db" />



Future Capabilities:
•	Advanced Forecasting: Implementing more advanced forecasting techniques, such as machine learning algorithms, can further enhance the accuracy of demand predictions.   
•	Real-Time Integration: Integrating real-time data sources, like sales trends and market fluctuations, will enable more dynamic and responsive inventory management.
•	Vendor Collaboration: Collaboration with key vendors can optimize lead times and lead to more efficient inventory planning.   
•	Automation: Automating routine tasks such as data cleaning and reporting can free up resources for more strategic analysis.   
 <img width="1600" height="915" alt="27_Future Capabilities" src="https://github.com/user-attachments/assets/bfc70b11-c17b-4395-8b0d-db3278b0f02a" />

 
References
•	https://www.kaggle.com/datasets/tanayatipre/store-sales-forecasting-dataset?resource=download
•	www.google.com
•	https://learn.microsoft.com/en-us/fabric/
•	https://nexusmax.io
•	External insights: EazyStock Blog
•	Industry benchmarks: Nventic Insights


