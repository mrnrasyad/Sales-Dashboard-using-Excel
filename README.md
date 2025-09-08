# Sales Dashboard using Excel: A Data Analytics Project

## Brief Description about this Project
The goal of this project is to prepare the data and use pivot tables and charts to analyze customer and product trends within a year, and finally present each chart in an interactive dashboard.

## Data Description
The dataset that used in this project is collected from kaggle - [https://www.kaggle.com/datasets/zahidmughal2343/amazon-sales-2025](https://www.kaggle.com/datasets/zahidmughal2343/amazon-sales-2025)

Below are the descriptions of the variables.

1. Date - Date of the order.
2. Product - Name of the product purchased.
3. Category - Product category (Electronics, Clothing, Home Appliances, etc.).
4. Price - Price of a single unit of the product.
5. Quantity - Number of units purchased in the order.
6. Total Sales - Total revenue from the order (Price × Quantity).
7. Customer Name - Name of the customer.
8. Customer Location - City where the customer is based.
9. Payment Method - Mode of payment (Credit Card, Debit Card, PayPal, etc.).
10. Status - Order status (Completed, Pending, or Cancelled).

## Scope of The Project
1. Data preparation
    - Copy the raw data to a working sheet for preparation while keeping the original data intact.
    - There are two data files: **Sales Transactions** and **Orders Detail**.
    - Created two new columns (**Payment Method** and **Order Status**) in *Sales Transactions*. Then used **XLOOKUP** to match and retrieve the payment method and order status for each *Order ID* from *Orders Detail*.
    - Checking duplicate data.
    - Fixed formatting issues in the **Date** column by trimming unnecessary spaces and replacing:
      - `"-"` with `"/"`
      - `"25"` with `"2025"`
    - Changed the data type of **Price** and **Total Sales** into *Currency*.
    - Added `"pcs"` as a unit label in the **Quantity** column.
    - Finally, converted the data range into an Excel Table for easier handling.
  
  2. Exploratory data analysis (EDA)
     - Created several pivot tables to analyze total orders by payment method, total sales by country, monthly sales by product category, top-selling products, and total orders by status, each visualized with clustered column or bar charts.
    
  3. Creating Sales Dashboard
     - Combining all the charts that were created and using slicers and timelines for filtering to make the dashboard more interactive, a 2025 Sales Dashboard was created.
    
## Results
#### **Total Orders** by **Payment Method**
Most customers prefer PayPal and Card payments, while Amazon Pay and Gift Cards remain less popular. This indicates an opportunity to either promote underused methods or optimize checkout for the most popular ones.

<p align="center">
  <img src=image/1.png />
</p>

#### **Total Sales** by **Cities**
Miami leads sales at $31,700, followed by Denver and Houston, while San Francisco and Los Angeles have the lowest. Overall, sales are strong in a few key cities but weaker in others, showing room for improvement.

<p align="center">
  <img src=image/2.png />
</p>

#### **Total Sales** per **Month**
Sales were really strong in February and March, led by home appliances and electronics, but everything dropped sharply in April. Footwear showed a small boost in March before falling too, while clothing and books stayed low throughout. Overall, sales started strong but couldn’t keep the momentum going.

<p align="center">
  <img src=image/3.png />
</p>

#### **Top Selling Products**
Refrigerators, laptops, and smartphones were the biggest revenue drivers, while clothing items and books barely contributed, showing that sales were heavily dominated by high-value electronics and appliances.

<p align="center">
  <img src=image/4.png />
</p>

#### **Total Ordes** by **Status**
Completed sales totaled 88 orders, while pending sales were 85 orders, and canceled sales were 77 orders.

<p align="center">
  <img src=image/5.png />
</p>

## Dashboard
This dashboard provides an overview of sales performance:
- **Trends over time** (monthly sales).
- **Geographic performance** (by cities).
- **Product insights** (top sellers).
- **Customer behavior** (payment methods).
- **Operational efficiency** (order status).

It also includes **interactive filters** (top section), allowing users to analyze specific conditions:
- **Filter by Month** → Sales data for each month (Feb–Mar 2025).
- **Filter by Product Category** → Books, Clothing, Electronics, Footwear, Home Appliances.
- **Filter by Status** → Cancelled, Completed, Pending.
- **Filter by Payment Method** → Amazon Pay, Credit Card, Debit Card, Gift Card, PayPal.

<p align="center">
  <img src=image/dash.jpg/>
</p>

## Recommendations
- Run promotions in low months (March).
- Focus marketing on Miami & SF, investigate LA & NY.
- Push high-value products, bundle low-sellers.
- Optimize checkout: prioritize PayPal/Cards, review Amazon Pay.
- Fix fulfillment to reduce pending/cancelled orders.
