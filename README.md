![image](https://github.com/user-attachments/assets/30791634-c116-47bf-b5c2-548d96b3e6bf)
# Customer-Segmentation-Analysis
This project entails preparing transaction data from an online retail store to segment customers based on their total spending and quantity of products purchased using a K-Means clustering algorithm. 



<h2>Introduction</h2>

<h5>Problem Statement</h5> 

<p>The need for proper and articulate segmentation is on the rise as businesses struggle with understanding and grouping their customer base in a way that unlocks better marketing and engagement strategies. Without efficient segmentation, time and cost are wasted resources because marketing campaigns lack the efficiency and specific highlights needed to drive sales.</p>

<h5>Context</h5>

<p>This project uses transaction data from an online retail store to segment customers based on their total spending and the quantity of products purchased. The dataset source is from a UK-based retailer, containing the following columns: InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country.</p>

<h5>Objectives</h5>

<ul>
<li>To clean and preprocess customer transaction data.</li>
<li>To determine the relevant metrics; Total Amount Spent and Quantity.</li>
<li>To apply K-Means clustering for customer segmentation.</li>
<li>To visualize and interpret the clusters.</li>
</ul>

<h2>Analysis</h2>

<h5>Data Cleaning</h5>

<p>The data cleaning process began with the removal of rows with missing values. After which the transactions were filtered to include only those with positive values in the Quantity and UnitPrice columns. This led to the need to create a new feature called TotalSpend, which is obtained by multiplying quantity by unit price.</p>

<h5>Grouping</h5>

<p>The data was grouped by the CustomerID column, where both the TotalSpend (sum of total quantity multiplied by UnitPrice) 
  and Quantity(sum of quantity purchased) were caculated. </p>
 
<h5>Data Standardization</h5>

<p>Scaled the data using StandardScaler to ensure TotalSpend and Quantity are suitable for a more effective clustering.</p>

<h5>K-Means Clustering</h5>

- Utilised the Elbow Method to determine the optimal number of clusters (K=5).
- Applied K-Means with optimal number of clusters.
- Assigned each customer to a cluster.

<h5>Visualization</h5>
<p>A scatter plot showing clusters with Total Spend vs. Quantity Purchased.</p>

<h2>Key Findings</h2>
- Clear segmentation was identified among customers.
- Some clusters represented high spenders with low quantity, while others represented frequent buyers with lower total spend.
- Identified a group of moderate spenders and quantities.

<h2>Conclusions</h2>

<h5>Insights</h5>

- Cluster 0: Likely occasional bulk buyers with high total spend but low frequency.
- Cluster 1: High frequency, moderate spend – loyal and frequent customers.
- Cluster 2: Low spend, low quantity – likely one-time or discount customers.
- Cluster 3: High quantity, low spend – volume buyers of low-cost goods.
- Cluster 4: Balanced cluster – average spenders with consistent purchases.

<h5>Recommendations</h5>

- Loyalty rewards and early access to new products should be offered to high-value customers.
- Subscriptions or discounts should be made available for frequent buyers.
- A referral-reward system should be made available for frequent buyers.
- Engagement campaigns can be revisited specifically for low spenders.




