
 E-Commerce Sales & Analytics Dataset

#Project Overview
This dataset contains transactional data for a retail e-commerce platform, covering the period from *January 2023 to June 2025*. It is designed for performing exploratory data analysis (EDA), identifying sales trends, and detecting statistical outliers in purchasing behavior.

# Dataset Summary
- Total Records: 1,200 Orders
- Total Revenue: $1,264,761.96
- Average Order Value: $1,053.97
- Key Categories: Technology, Office Supplies, and Furniture

# Data Dictionary

| Column Name | Data Type | Description |

| *OrderID* | String | Unique identifier for each transaction. |
| *Date* | Date | The date the order was placed (YYYY-MM-DD). |
| *CustomerID* | String | Unique identifier for the customer. |
| *Product* | String | Name of the item purchased (e.g., Laptop, Monitor, Chair). |
| *Quantity* | Integer | Number of units purchased (Range: 1 to 5). |
| *UnitPrice* | Float | Price per single unit of the product. |
| *ShippingAddress*| String | Customer's delivery location. |
| *PaymentMethod* | String | Method used (Cash, Online, Credit Card, etc.). |
| *OrderStatus* | String | Status of the order (Delivered, Shipped, Pending, Cancelled, Returned). |
| *ItemsInCart* | Integer | Total items in the user's cart at checkout. |
| *CouponCode* | String | Promotional code applied (if any). |
| *ReferralSource* | String | Marketing channel (Instagram, Google, Facebook, etc.). |
| *TotalPrice* | Float | Final transaction amount (Quantity × UnitPrice). |

# Key Insights & Observations
1. Outlier Detection:0.67% of orders are classified as high-value outliers (TotalPrice > $3,330), primarily involving Laptops and Tablets.
2. Sales Channels: Instagram is the leading referral source for revenue.
3. Operational Risk: Approximately *41%* of orders are either *Cancelled or Returned*, indicating a significant area for operational improvement.
4. Product Demand:Chairs and Printers are the most frequently sold items by total volume.

# Usage Instructions
- Power BI: Use a Scatter Chart with OrderID in the Details bucket to visualize outliers.
- Python/Excel: Apply the IQR (Interquartile Range) method on the TotalPrice column to filter statistical anomalies.
