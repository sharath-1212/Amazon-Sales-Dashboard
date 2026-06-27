# Amazon Sales Dashboard

A comprehensive sales analytics dashboard for Amazon sales data, featuring both Power BI visualization and Python-based data analysis.

## Project Overview

This project provides tools to analyze and visualize Amazon sales data through two complementary approaches:
- **Power BI Dashboard** (`amazon.pbix`) - Interactive visual analytics
- **Python Analysis Script** (`main.py`) - Programmatic data analysis and visualization

## Dataset

The project uses a sales dataset (`Dataset/powerbi_sales_data.csv`) containing the following columns:
- `Order_ID` - Unique order identifier
- `Date` - Transaction date
- `Region` - Sales region (North, South, East, West)
- `Category` - Product category (Accessories, Electronics)
- `Product` - Product name (Monitor, Tablet, Phone, Headphones, Laptop)
- `Sales` - Sales amount
- `Profit` - Profit amount
- `Quantity` - Quantity sold

## Components

### 1. Power BI Dashboard (`amazon.pbix`)
Interactive Power BI dashboard for visual exploration of sales data. Open this file in Power BI Desktop to access:
- Interactive charts and graphs
- Region-based analysis
- Product performance metrics
- Time-based trend analysis

### 2. Python Analysis Script (`main.py`)
Python script that performs automated data analysis and generates visualizations.

#### Features:
- **Data Loading**: Reads the CSV dataset using pandas
- **Summary Statistics**: Calculates total sales and profit
- **Regional Analysis**: Aggregates sales by region
- **Product Analysis**: Identifies top 5 performing products
- **Trend Analysis**: Computes monthly sales trends
- **Visualizations**: Generates bar charts and line plots

#### Outputs:
- Console output with key metrics
- Bar chart: Sales by Region
- Line chart: Monthly Sales Trend

## Requirements

### Python Dependencies
```bash
pandas
matplotlib
```

Install dependencies:
```bash
pip install pandas matplotlib
```

### Power BI
- Power BI Desktop (for opening `.pbix` file)

## Usage

### Running the Python Analysis

Run the analysis script:
```bash
python main.py
```

The script will:
- Display sample data from the dataset
- Show total sales and profit figures
- Print sales breakdown by region
- List top 5 products by sales
- Generate and display two visualization charts

### Using the Power BI Dashboard

1. Open `amazon.pbix` in Power BI Desktop
2. Explore the interactive visualizations
3. Filter and analyze data as needed

## Project Structure

```
Amazon Sales Dashboard/
├── Dataset/
│   └── powerbi_sales_data.csv    # Sales dataset
├── amazon.pbix                   # Power BI dashboard
├── main.py                       # Python analysis script
└── README.md                     # This file
```

## Key Metrics Analyzed

- **Total Sales**: Sum of all sales transactions
- **Total Profit**: Sum of all profit values
- **Regional Performance**: Sales distribution across North, South, East, and West regions
- **Product Performance**: Top-selling products ranked by revenue
- **Monthly Trends**: Sales patterns over time

## Example Output

When running `main.py`, you will see:
```
Sample Data:
[First 5 rows of dataset]

Total Sales: [total amount]
Total Profit: [total amount]

Sales by Region:
Region
North    [amount]
South    [amount]
East     [amount]
West     [amount]

Top 5 Products:
Product
[Product names with sales amounts]
```

## Notes

- The Python script expects the CSV file to be in the `Dataset/` subdirectory
- Ensure the script is run from the project root directory
- The Power BI file can be customized with additional visualizations as needed
