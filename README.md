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

## Data Visualization:

<img width="1244" height="931" alt="image" src="https://github.com/user-attachments/assets/c00365b5-6c10-47f5-95f0-d4c0941d8a3b" />

**1. Qty (Quantity) Histogram**

- The distribution is highly right-skewed.
- Most of the transactions have a quantity close to 1 or 2 units.
- There is a very sharp peak at 1, indicating that the majority of orders consist of a single item.
- Quantities greater than 3 are extremely rare.

This suggests that customers typically purchase small quantities per order, possibly reflecting typical retail or consumer purchasing behavior.

**2. Amount Histogram**

- The amount feature is also right-skewed, with the bulk of transaction amounts concentrated between approximately 0 and 1500.
- There is a peak around the 500 to 800 range, indicating many transactions fall into moderate spending amounts.
- There are a few outliers or transactions with amounts extending beyond 2000, but these are rare.

This distribution suggests that most sales are low to mid-value transactions, with few very high-value purchases.

**3. ship_postal_code Histogram**

- The distribution of ship_postal_code values appears multi-modal, with several distinct peaks.
- Values are spread between roughly 100,000 to 900,000, with clear concentration points around 200,000, 400,000, 550,000, 700,000, etc.
- This pattern indicates that shipments are coming from a few dominant postal regions or zones.
- The gaps between peaks suggest that there are distinct clusters of postal codes, possibly corresponding to geographic areas with different order volumes.
  

<img width="630" height="470" alt="image" src="https://github.com/user-attachments/assets/83ca0fe7-4535-455f-9e2d-f6ed617673e5" />

The order lifecycle is dominated by successful shipments and deliveries, indicating an effective logistics workflow. However:
- The high cancellation volume is a key area that warrants further investigation.
- Return- and rejection-related statuses, while low in count, should be monitored for product quality issues.
- Very rare issues such as lost or damaged shipments show that problems exist but at manageable levels.

  
## Data Filtering 
- Expedited Shipment by Category
- Merchant fulfillments by Courier Status
- Trousers (clothing category) shipped by Amazon
- Orders Status in selected City
- Amazon & Merchant fulfillments by Cancelled Orders


### Next Steps:
I plan to continue this project in Tableau to enhance insights into regional performance, shipping services, sales trends, products performance, and to build interactive dashboards for more dynamic and accessible business insights.
