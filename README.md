# Procurement Analysis Dashboard with Power BI

## Overview
This project involves creating a comprehensive data warehouse schema for invoice analysis, followed by visualizing the analytical results using Power BI. The data warehouse consists of several dimension tables for detailed categorization and a fact table for transactional data. The Power BI dashboard leverages this structured data to provide insights into invoice metrics, vendor performance, and spending patterns.

## Database Schema

The data warehouse schema includes the following dimension tables and a fact table to support a wide range of analysis and reporting needs:

### Dimension Tables

- **DimCurrency**: Stores currency information.
- **DimLocation**: Contains details about locations including country and region.
- **DimDate**: Holds date-related information, facilitating time-based analysis.
- **DimVendor**: Details of vendors including location, spend, and tier.
- **DimItem**: Information about items including category, sub-category, and commodity details.
- **DimExchangeRate**: Exchange rates between different currencies on different dates.

### Fact Table

- **Fact_Invoice**: Captures invoice transactions, linking to dimensions for detailed analysis.

### Relationships

The schema defines relationships between the fact table and dimension tables, enabling a comprehensive multi-dimensional analysis.

## Power BI Dashboard

The Power BI dashboard is designed to provide actionable insights from the invoice data. It includes various measures, filters, and slicers created using DAX and M language for data manipulation.

### Key Features

- **Dynamic Measures**: Created using DAX to calculate metrics like total spend, savings, and average unit price.
- **Filters and Slicers**: Allow for interactive analysis by vendor, item, location, and time period.
- **Visualization Components**: Includes charts, tables, and graphs that dynamically update based on user selections.

### Development Process

1. **Data Import**: Data is imported into Power BI from the data warehouse using Power Query.
2. **Data Manipulation**: The M language is used within Power Query for cleaning and preparing data.
3. **Measure Creation**: DAX is used to create calculated columns, measures, and business metrics.
4. **Dashboard Design**: Visual components are added and configured to display the desired metrics.
5. **Interactivity**: Slicers and filters are set up to allow users to interact with the dashboard for in-depth analysis.

## Getting Started

To utilize this project:

1. **Setup Database**: Create the database tables as defined in the schema and load your data.
2. **Configure Power BI**: Import the data into Power BI Desktop.
3. **Customize Measures**: Adapt the DAX measures according to your specific analysis needs.
4. **Explore the Data**: Use the dashboard to explore invoice data, identify trends, and make informed decisions.

## Conclusion

This project provides a robust foundation for analyzing invoice data, offering insights into vendor performance, spending patterns, and the impact of currency exchange rates on transactions. The Power BI dashboard enhances the analytical capabilities, making it easier to visualize complex data and uncover actionable insights.
