# Product Recommendations for Store Expansion
## Project Overview
This project involved making product recommendations for new stores across various states based on historical store performance data. The company currently operates stores in 6 states and is expanding into additional states, with specific locations and store types identified. However, the food and beverage offerings at these new stores needed to be determined.

## Goal: 
To provide data-driven recommendations for the food and beverage offers (Chicken, Adv GnG (Pizza), Bean to Cup (Coffee), Swirl World (Frozen Yogurt), and DoorDash) at new stores based on insights from historical data.

## Tools used:
- **`Microsoft Excel`** (for data cleaning, manipulation, and analysis)
- **`Power BI`** (for data visualization and interactive reporting)
- **`Gamma AI`** (for presenting findings and recommendations)

## Steps Followed in the Project:

### 1. Data Cleaning and Preparation

- Handled missing values by replacing them with `0` from the store `Performance Data` in Excel.
- Replaced `6K` with `5.5K` in the store type column to reflect correct store classifications.
- Stored the clean data in the Clean Table worksheet.

### 2. Sales Per Day Calculation

- Using `Power Query`, calculated the daily sales for each offering by dividing the total sales by the number of days the store had been open (from the `Days Store Open` column).
- Removed redundant columns and saved this table in the `Rate Table` worksheet, which contained normalized sales values on a per-day basis.
  
### 3. Aggregation with Pivot Tables

- Created `Pivot Table` to aggregate sales values by store type.
- Grouped sales figures for relevant products, such as Chicken, Adv GnG (Pizza), Bean to Cup, Frozen Yogurt, and DoorDash, to analyze their daily performance across various store types.
  
### 4. Sales Distribution Analysis

- Calculated the relative sales distribution for each product offering across different store types.
- Unpivoted the sales distribution table to facilitate better chart creation and visualization.
- Visualized sales distribution to understand trends in product performance across store types.

  ![Sales Distribution Chart](https://github.com/codenirmal99/Product_Recommendations_for_Store_Expansion/blob/main/Images/Sales%20Distribution.png)
  
### 5. Recommendations Based on Analysis

After analyzing sales distribution and product performance, specific recommendations were made for each store type:

- ### **5.5K Stores (Urban Focus)**

    - Adv GnG (Pizza): Focus on variety and quality for urban customers.
      
    - Bean to Cup (Coffee): Emphasize convenience for city dwellers.
    - Chicken: Introduce grab-and-go meal options.
    - DoorDash: Partner for increased urban delivery convenience.
    - Swirl World (Frozen Yogurt): Capitalize on trends with diverse flavours.
      
- ### **EDO Stores (Hybrid)**

    - Adv GnG (Pizza): Balance quality and convenience for both locals and travellers.
      
    - Bean to Cup (Coffee): Ensure quick service for both customer groups.
    - Chicken: Offer both snack and meal options.
    - DoorDash: Keep options open for future expansion.
    - Swirl World (Frozen Yogurt): Offer a mix of classic and innovative flavours.

- ### **Travel Centers (Traveller Focus)**

    - Adv GnG (Pizza): Prioritize quick, easy-to-eat options.
      
    - Bean to Cup (Coffee): Provide fast, efficient caffeine fixes.
    - Chicken: Focus on filling meal options for long-distance travellers.
    - DoorDash: Low focus, as travellers prioritize in-store purchases.
    - Swirl World (Frozen Yogurt): Provide refreshing treats for travellers.
      
### 6. Correlation Analysis

- Calculated the correlation coefficient between the `Inside Guest Count Per Day` and the `Sales per day for each product` offering.
- The correlation helped validate recommendations by showing the relationship between foot traffic and product sales.

### 7. Power BI Dashboard

- Built an interactive `Power BI` Dashboard to provide a visual overview of product sales distribution by store type.
- Stakeholders could filter by store type and product to view daily sales averages and recommendations for new stores.
- A `Shape Map` visual allowed stakeholders to see average sales by state for different products.

    ![Dashboard](https://github.com/codenirmal99/Product_Recommendations_for_Store_Expansion/blob/main/Images/Dashboard.png)
  
### 8. Data Transformation and Unpivoting

**`Melted Table`**: Derived from the `Rate Table`, this unpivoted table allowed for easier aggregation and visualization of per-day sales figures.
**`Melted Full Table`**: Derived from the `Clean Table`, this unpivoted table contained overall calculations.

### 9. Data Relationships

Established relationships between various tables (e.g., Store Connector, Offer Connector, Recommendation Table, Melted Table, Melted Full Table ) to enable filtering and dynamic data analysis in Power BI.

### 10. Final Presentation

- Used `Gamma AI` to generate the presentation summarizing the findings and product recommendations for each new store location.
- The presentation included an overview of the current product mix offered at different store types.

    ![Dashboard](https://github.com/codenirmal99/Product_Recommendations_for_Store_Expansion/blob/main/Images/Brief%20Presentation.png)

## Conclusion
- By analyzing past store performance, this project provided targeted recommendations for product offerings in new store locations. The integration of `Excel` for analysis, `Power BI` for visualization, and `Gamma AI` for presentation ensured that the final recommendations were both data-driven and effectively communicated.
  
- This analysis will assist Senior Leadership in making informed decisions about which product offerings to implement in new stores, maximizing both customer satisfaction and profitability.
