# Repeated Customers Analysis

## Overview

This project focuses on analyzing the behavior of repeated customers by using matrix visualizations to compare spending patterns across different product segments and customer segments over multiple years. The visualization helps highlight differences in customer spending year over year, enabling businesses to derive actionable insights from the data.

## Applicability of Matrix Visualization

### 1. **Flexible Customer and Product Segmentation**
The matrix visualization is highly flexible, allowing for an unlimited number of customer and product segments. These segments can be dynamically defined based on the available data. The typical customer segments could be:
- **Small customers**
- **Medium customers**
- **Large customers**

Similarly, product segments can vary based on the business needs, such as:
- **Product-Segment-1**
- **Product-Segment-2**
- **Product-Segment-3**
  
The visualizations can handle **any number of customer and product segments**, making the code adaptable to various datasets without needing to adjust for specific segment names or structures.

### 2. **Year-over-Year Comparison Across Multiple Years**
The matrix visualization also supports the comparison of data over multiple years. The structure is designed to dynamically compare spending changes between **consecutive years**, regardless of how many years of data are available. This flexibility allows for easy adaptation to datasets with different year ranges.

### 3. **Identification of Patterns and Trends**
With this visualization, businesses can quickly identify important patterns, such as:
- **High-growth segments**: Customer segments with significant increases in spending.
- **Declining segments**: Customer or product combinations that show a significant drop in spending.
  
This enables businesses to spot trends over time across multiple years and make adjustments to their marketing, sales, or product strategies.

### 4. **Actionable Insights for Marketing and Sales**
This matrix visualization helps identify trends and areas that may require action, such as:
- Developing targeted marketing campaigns for high-growth segments.
- Offering promotions to reverse declining trends in certain product segments.
- Shifting resources toward high-performing products or customer groups.

The matrix visualization allows businesses to base decisions on actual data rather than assumptions, resulting in more effective strategies.

## Explanation of `combined_df.csv`

The file `combined_df.csv` is generated as part of the analysis. It provides a combined dataset containing **year-to-year differences** for each customer across different product segments. This dataset enables further external analysis, beyond what is visualized in the matrix.

### Structure of `combined_df.csv`

The `combined_df.csv` file contains the following columns:
- **customer_id**: The unique identifier for each customer.
- **customer_segment**: The segment the customer belongs to (e.g., small, medium, large).
- **year_to_year**: The consecutive years being compared (e.g., 2021_2022, 2022_2023).
- **product-segment-X_previous**: The total spending in the previous year for the specific product segment.
- **product-segment-X_following**: The total spending in the following year for the specific product segment.
- **product-segment-X_diff**: The raw difference in spending between the two years for the product segment.
- **total_value_previous**: The total spending across all product segments in the previous year.
- **total_value_following**: The total spending across all product segments in the following year.
- **total_diff**: The total raw difference in spending between the two years across all product segments.

### Applicability of `combined_df.csv`

This file is extremely useful for researchers and analysts who wish to perform additional external analysis of the year-to-year differences across customer and product segments. With this data, one can:
- Perform custom statistical analysis.
- Run machine learning models to predict future spending behavior.
- Build external visualizations for presentations or reports.
  
The flexibility of this dataset enables deeper exploration of customer behavior, making it suitable for a wide range of business or academic applications.

## Conclusion

The matrix visualization and `combined_df.csv` file provide powerful tools for analyzing customer behavior over time, supporting multiple product and customer segments dynamically. With the ability to handle unlimited segments and years, this project offers a scalable solution for businesses looking to derive insights from their repeated customers' spending behavior.
