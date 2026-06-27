# Business Data Cleaning, Validation and Excel Reporting

## Problem Summary

The objective of this project is to clean, validate, and prepare a retail order dataset for business analysis using Microsoft Excel. The raw dataset contains duplicate records, missing values, inconsistent formatting, invalid discounts, date issues, and order status inconsistencies.

# Dataset Description

The dataset contains order-level retail sales information, including:

* Order ID
* Customer Name
* Customer Segment
* Region
* State
* City
* Category
* Sub Category
* Ship Mode
* Quantity
* Unit Price
* Discount
* Sales
* Cost
* Payment Status
* Order Status
* Order Date
* Ship Date

# Tools Used

* Microsoft Excel
* Excel Formulas
* Pivot Tables
* Conditional Formatting
* Find & Replace
* Flash Fill
* Sorting and Filtering

# Cleaning Steps Performed

* Preserved the original dataset
* Removed extra spaces using TRIM()
* Removed unwanted characters using SUBSTITUTE()
* Standardized text formatting
* Converted date fields into a consistent format
* Calculated Shipping Delay
* Identified and removed exact duplicate records
* Flagged conflicting duplicate Order IDs
* Filled missing Region values with "Unknown"
* Filled missing Ship Mode values with "Unknown"
* Validated discount values
* Applied business validation rules
* Created calculated columns
* Generated data quality reports
* Created Pivot Table summaries

# Business Rules Applied

* Missing Region → Unknown
* Missing Ship Mode → Unknown
* Missing Discount → 0 (only if other sales fields were valid)
* Negative Discount → Invalid
* Discount above the allowed limit → Invalid
* Cancelled Orders excluded from completed sales analysis
* Failed Payments excluded from completed sales analysis
* Refunded Orders summarized separately
* Ship Date before Order Date marked as Invalid

# Summary of Data Quality Issues Found

The following issues were identified during data cleaning:

* Missing values
* Duplicate records
* Duplicate Order IDs
* Invalid Discounts
* Date inconsistencies
* Invalid Shipping records
* Cancelled Orders
* Failed Payments
* Refunded Orders
* Sales calculation mismatches

# Summary of Final Pivot Reports

The following Pivot Tables were created:

1. Sales and Profit by Region
2. Sales and Profit by Category and Sub Category
3. Order Count by Ship Mode
4. Profit Margin by Customer Segment
5. Refunded, Cancelled and Failed Orders by Region
6. Monthly Sales Trend

# Key Business Insights

* Some regions generated higher sales and profit than others.
* Certain product categories contributed significantly more profit.
* Standard Class was the most frequently used shipping method.
* Profit margin varied across customer segments.
* Refunded, Cancelled, and Failed Orders affected completed sales performance.
* Monthly sales trends highlighted seasonal business patterns.

# Assumptions and Limitations

## Assumptions

* Maximum discount allowed = 50%
* Missing Discount treated as 0 when appropriate
* Missing Region and Ship Mode replaced with "Unknown"

## Limitations

* Conflicting duplicate records require manual verification.
* Unknown values may affect detailed regional analysis.
* Results depend on the quality of the original source data.

# Screenshots Included

The repository contains screenshots of:

* Raw Data Preview
* Cleaned Data Preview
* Pivot Summary 1
* Pivot Summary 2

These screenshots demonstrate the successful completion of the data cleaning and reporting process.

