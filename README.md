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
