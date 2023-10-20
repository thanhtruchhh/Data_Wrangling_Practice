# Data Wrangling Practice

## Overview
This project calculates the total revenue of each product from separate pieces of data by using pandas package in Python. The project's objective is to provide a data wrangling solution applicable to datasets with a large number of records.

## Data Dictionary
The project includes two datasets:

### prices.csv
Records of product's history price changes in Sep 2018:

- `product_id`: Unique identifier for each product.
- `old_price`: Previous price of the product.
- `new_price`: Updated price of the product.
- `updated_at`: When the price was updated.

### sales.csv
Records of product's sales in Sep 2018:

- `product_id`: Unique identifier for each product.
- `ordered_at`: When the product was ordered.
- `quantity_ordered`: The quantity of the product ordered.

## Project Workflow
- **Data Processing**: Loading and cleaning the data.
- **Merging Data**: Combining the two datasets using the `merge_asof` function. Two approaches were applied for merging:
  - Direction = nearest.
  - Direction = backward (combine with direction = forward).
- **Total Revenue Calculation**: Calculating the total revenue for each product.
