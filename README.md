# Unsupervised Learning: Creating Customer Segments

## Project Overview

This project focuses on discovering internal structures, patterns, and knowledge from a dataset containing various customers' annual spending amounts across diverse product categories. The primary objective is to segment customers into distinct groups based on their spending behavior using unsupervised learning techniques.

## Dataset

The dataset comprises customer spending data across multiple product categories. Each entry represents the annual spending (in monetary units) for a particular customer on different products.

## Key Objectives

- **Data Exploration and Preprocessing:** Conducted thorough exploration and preprocessing to clean and normalize the data, ensuring it's suitable for clustering algorithms.
  
- **Dimensionality Reduction:** Employed Principal Component Analysis (PCA) to reduce the dimensionality of the dataset while preserving significant variance, facilitating better visualization and interpretation of customer segments.
  
- **Clustering:** Implemented K-Means clustering to group customers based on their spending patterns, identifying distinct customer segments.

- **Visualization and Insights:** Visualized the clustered data to gain insights into the different customer segments, providing actionable information for targeted marketing strategies.

## Results

- Successfully segmented customers into distinct groups with similar spending patterns.
- Provided a comprehensive analysis of each segment, highlighting key characteristics and potential marketing strategies.

## Conclusion and Implications: How to Use This Knowledge

In this final section, we explore ways to leverage the clustered data effectively. We will first consider how the different groups of customers, or customer segments, may be affected by specific changes, such as a new delivery scheme. Additionally, we will discuss how assigning a label to each customer, based on their segment, can provide valuable features for further analysis and decision-making.

### Using Customer Segments for A/B Testing

Companies often conduct A/B tests when making small changes to their products or services to gauge the impact on customers. For instance, a wholesale distributor is considering reducing its delivery service from 5 days a week to 3 days a week. However, this change will only be implemented for customers who are likely to react positively.

Given that the change would reduce the frequency of deliveries, the distributor can use the identified customer segments to determine which customers might respond favorably. The A/B test should be conducted on one segment at a time, ensuring that both the control and experimental groups come from the same cluster. This approach is crucial because different customer segments have varying needs and may react differently to changes in delivery frequency.

### Engineering Features from Customer Segments

Clustering techniques allow us to derive additional structure from originally unlabeled data. Each customer now has a segment they best identify with, based on the applied clustering algorithm. This 'customer segment' can be considered an engineered feature for the dataset.

For example, if the wholesale distributor recently acquired ten new customers who provided estimates for their anticipated annual spending across different product categories, the distributor can classify each new customer into a segment. This classification can help determine the most appropriate delivery service for these new customers, based on the behavior and needs of similar existing customers.

By leveraging these insights, companies can make more informed decisions, tailor their services to specific customer needs, and enhance overall customer satisfaction.

## Libraries Used

1. **Pandas**  
2. **Numpy**
3. **Scikit-Learn**
