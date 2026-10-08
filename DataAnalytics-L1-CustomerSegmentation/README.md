# Customer Segmentation Analysis

## Objective

The objective of this project is to segment customers based on their purchasing behavior using RFM (Recency, Frequency, Monetary) analysis and K-Means clustering.

## Dataset

The Online Retail dataset from the UCI Machine Learning Repository was used for this analysis.

The dataset contains retail transactions with information such as:
- Invoice Number
- Stock Code
- Product Description
- Quantity
- Invoice Date
- Unit Price
- Customer ID
- Country

## Data Cleaning

The following preprocessing steps were performed:

- Removed transactions with missing Customer IDs.
- Removed duplicate transactions.
- Removed transactions with negative or zero quantities.
- Removed transactions with zero or negative prices.

After cleaning, the dataset contained 392,692 valid transactions.

## RFM Analysis

Three customer behavior metrics were calculated:

- **Recency:** Number of days since the customer's last purchase.
- **Frequency:** Number of unique invoices/orders made by the customer.
- **Monetary:** Total amount spent by the customer.

The analysis identified 4,338 unique customers.

## Customer Segmentation

K-Means clustering was applied to the standardized RFM data.

The Elbow Method was used to determine the optimal number of clusters. Based on the elbow curve, 4 clusters were selected.

### Customer Segments

| Cluster | Segment | Customers |
|---|---|---:|
| 0 | Regular / Potential Customers | 3,054 |
| 1 | At-Risk / Inactive Customers | 1,067 |
| 2 | VIP / High-Value Customers | 13 |
| 3 | Loyal Customers | 204 |

## Segment Recommendations

### VIP / High-Value Customers
Provide VIP benefits, exclusive offers, early access to new products, and personalized rewards.

### Loyal Customers
Use loyalty programs, personalized recommendations, and cross-selling offers to increase customer lifetime value.

### Regular / Potential Customers
Use targeted promotions and incentives to encourage repeat purchases and move customers toward the loyal segment.

### At-Risk / Inactive Customers
Use re-engagement campaigns, discounts, reminders, and personalized offers to encourage customers to return.

## Visualizations

The project includes:

- Elbow Method plot
- Customer count by segment
- Recency vs Frequency scatter plot
- Frequency vs Monetary Value scatter plot
- Customer segment profiling

## Conclusion

The customer segmentation analysis grouped 4,338 customers into four distinct segments based on their purchasing behavior.

The segmentation provides useful insights for targeted marketing, customer retention, loyalty programs, and identifying high-value customers.
