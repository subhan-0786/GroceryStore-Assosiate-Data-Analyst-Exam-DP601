# Grocery Store Sales Analysis - FoodYum

This repository contains code and solutions for a practical exam focused on analyzing grocery store sales data for FoodYum, a U.S.-based grocery store chain. The goal is to ensure data cleanliness, analyze product pricing, and identify trends in sales to support stocking decisions across various product categories.

## Dataset Description

The dataset contains records of grocery store products from FoodYum, including details about the product types, brands, weight, price, and sales performance. Data cleaning is essential to handle missing values, ensure standard formats, and prepare the dataset for sales analysis.

### Table: `products`

| Column Name          | Description                                                                                           |
|----------------------|-------------------------------------------------------------------------------------------------------|
| product_id           | Unique identifier for the product. Missing values not possible.                                        |
| product_type         | The category of the product, such as Produce, Meat, Dairy, Bakery, Snacks. Missing values replaced with "Unknown". |
| brand                | The brand of the product. One of 7 possible values. Missing values replaced with "Unknown".            |
| weight               | The weight of the product in grams. Missing values replaced with the median weight of the dataset.     |
| price                | The price of the product in US dollars. Missing values replaced with the median price of the dataset.  |
| average_units_sold   | The average number of units sold per month. Missing values replaced with 0.                            |
| year_added           | The year the product was added to FoodYum’s stock. Missing values replaced with 2022.                 |
| stock_location       | The warehouse location where the stock is stored. Missing values replaced with "Unknown".             |

## Tasks

- **Task 1: Count Missing Year Added**  
Identify how many products have missing values in the `year_added` column.

- **Task 2: Data Cleaning**  
Clean the dataset by replacing missing values as per the specified criteria.

- **Task 3: Price Range by Product Type**  
Determine the minimum and maximum prices for each product category.

- **Task 4: Meat and Dairy Products with High Sales**  
Filter and return Meat and Dairy products with over 10 units sold per month on average.

## File Structure

- `grocery_data.csv`: The original dataset containing product details and sales data.
- `task1.sql`: SQL query for counting missing year_added values.
- `task2.sql`: SQL query for cleaning the product data.
- `task3.sql`: SQL query for analyzing the price range by product type.
- `task4.sql`: SQL query for filtering Meat and Dairy products with high sales.

## How to Use

1. Clone the repository:

    ```bash
    git clone https://github.com/subhan-0786/grocery-store-sales-analysis.git
    ```

2. Use a database client like PostgreSQL or MySQL to execute the SQL scripts provided for each task. For example:

    ```bash
    psql -U username -d grocerydb -f task1.sql
    ```

3. Follow the instructions for each task to explore the dataset and gain insights.

## Results

- The data cleaning task ensured that missing values were handled, and the dataset was prepared for further analysis.
- An analysis of price ranges by product type showed the variation in pricing across different categories.
- The investigation into Meat and Dairy products with high average units sold highlighted key products contributing to high sales.

## License

This project is licensed under the MIT License.
