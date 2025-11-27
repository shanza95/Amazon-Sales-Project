# Sales-Project
## Project Overview:
This project involved preparing and analyzing an Amazon Sales dataset to extract meaningful insights by first addressing data quality issues.

### Key Tasks:
## Data Cleaning:
- Identified and handled missing values with appropriate methodology
- Performed string manipulation to fix inconsistencies in text fields
- Handled duplicate entries
- Standardize few feature names, merged multiple name variations into single, consistent values.

## Data Preparation:
- Sorted the dataset to improve readability and analysis
- Ensured all categorical and numerical fields were structured appropriately

## Exploratory Data Analysis (EDA):
- Uncovered sales trends, regional performance, and product-level insights
- Applied conditional formatting to highlight key metrics, anomalies, and patterns in the data.

The dataset contains 128,976 orders with a mix of categorical features such as order status, fulfillment, category, size, and location fields. Below is a structured breakdown of key observations.

**Product Category Distribution**
The dataset is heavily apparel-driven, dominated by *T-shirts* and *Shirts*, jointly contributing ~78% of all orders. Accessories and footwear (Perfume, Wallet, Socks, Shoes, Watch) make up a very small share. *Watch* category has negligible data (3 orders).

**Sales Channel Distribution**
The business is almost entirely dependent on Amazon as a sales channel (99.9%) and within India. Non-amazon is insignificant in volume.

**Shipping Service Level**
Majority of orders use *Expedited shipping*, indicating customer preference for faster delivery, company prioritizing quicker logistics options. Cancellations/ returns are extremely dependent on apparel sizing and fulfillment type. City and state diversity is high, suggesting nationwide coverage.

## Data Visualization:

<img width="1244" height="931" alt="image" src="https://github.com/user-attachments/assets/c00365b5-6c10-47f5-95f0-d4c0941d8a3b" />

**1. Qty (Quantity) Histogram**
This suggests that customers typically purchase small quantities per order, possibly reflecting typical retail or consumer purchasing behavior.

**2. Amount Histogram**
This distribution suggests that most sales are low to mid-value transactions, with few very high-value purchases.

**3. ship_postal_code Histogram**

- The distribution of ship_postal_code values appears multi-modal, with several distinct peaks.
- The gaps between peaks suggest that there are distinct clusters of postal codes, possibly corresponding to geographic areas with different order volumes.
  

<img width="630" height="470" alt="image" src="https://github.com/user-attachments/assets/83ca0fe7-4535-455f-9e2d-f6ed617673e5" />

The order lifecycle is dominated by successful shipments and deliveries, indicating an effective logistics workflow. However:
- The high cancellation volume is a key area that warrants further investigation.
- Return- and rejection-related statuses, while low in count, should be monitored for product quality issues.
- Very rare issues such as lost or damaged shipments show that problems exist but at manageable levels.

  
## Data Filtering 

**- Expedited Shipment by Category**
  
The product distribution is highly concentrated in apparel, specifically *Shirts* and *T-shirts*, followed by *Blazers* and *Trousers*. Accessories abd footwear contribute marginally to total sales volume.

This suggests the business is primarly apparel-focused, and optimization strategies should prioritize inventory, pricing, and promotion of high-volume categories, while reassessing low-volume categories for potential phase-out or targeted improvement.

**- Merchant fulfillments by Courier Status**

Majority of Merchant Orders fall under *Shipped*, followed by 6,870 orders *On the Way*. Only 524 orders remain in *Unshipped* status. From a logistic performance perspective, this is an efficient and well-balanced status distribution, with the vast majority already processed or en-route. 

**- Trousers (clothing category) shipped by Amazon**

The highest number of orders are for the sizes *XXL, XL, M, L*, indicating that large to mid sizes are the most purchased. Smaller sizes (*XS and S*) and extended sizes (*3XL*) have lower but still meaningful demand. 

These inisights can support inventory planning (higher stock levels for L, XL, XXL, M), restocking strategy, promotions tailored to body size distribution, supply chain optimization apparel for Amazon-fulfilled apparel.

**- Orders Status in selected City (AGRA, MUMBAI, PUNE)**

- Mumbai is the dominant city in order volume across all statuses, reflecting a major customer base and high fulfillment activity.
- Pune shows strong performance and medium-scale demand.
- Agra has low order traffic, stable status distribution, and minimal exception cases.

Exception statuses (returns, rejections, out-for-delivery) are very low, suggesting efficient delivery processes in all cities.

Cancellations are proportionate to order volumes and highest in Mumbai.

**- Amazon & Merchant fulfillments by Cancelled Orders for all sizes**

- Amazon fulfillment dominates in volume, which explains the higher cancellation counts across all sizes.
- Mid-range apparel sizes (S to XXL) experience the highest cancellations, likely due to high sales volume and common sizing uncertainties.
- Larger sizes (4XL–6XL) have very low cancellations, reflecting their lower demand.
- Cancellation trends between Amazon and Merchant are very similar in pattern — the only major difference is scale.
- While the demand is low, Amazon still shoes more cancellation than Merchant even in sizes 4XL (35 vs 13), 5XL (38 vs 17), 6XL (50 vs 22). This further reinforces that Amazon handles more overall volume, not that Merchat has fewer cancellation issues.

### Next Steps:
I plan to continue this project in Tableau to enhance insights into regional performance, shipping services, sales trends, products performance, and to build interactive dashboards for more dynamic and accessible business insights.
