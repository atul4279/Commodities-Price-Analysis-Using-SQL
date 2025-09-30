# Commodities-Price-Analysis-Using-SQL
This project demonstrates SQL-based data modeling and analysis on commodity price data across regions in India.
It includes:

A database schema with commodity, region, and price details.
Pre-populated datasets for commodities, states, cities, and prices.

Analytical SQL queries answering real-world business questions such as top costly commodities, price variations, and availability trends.

Project Structure
commodity_db.sql
Creates the schema commodity_db.

Defines and populates tables:
commodities_info: Commodity details (Id, Name, Variety, Unit, Category).
region_info: Region-level details (Id, Centre, State).
price_details: Commodity price details (Id, Region_Id, Commodity_Id, Date, Retail_Price).

Commodities+Prices+Solution.sql
Contains SQL queries answering analytical questions:
Common commodities in Top 10 costliest between 2019 and 2020.
Commodity with maximum price difference across regions (Jun 2020).
Commodities ranked by number of available varieties.
Most available commodity in the state with least data points.
Commodity with the highest price variation (Jan 2019 – Dec 2020).

How to Use
Clone the repository:
git clone https://github.com/atul4279/commodities-prices-sql.git

cd commodities-prices-sql

Load the schema and sample data in MySQL:
SOURCE commodity_db.sql;

Run analytical queries:
SOURCE Commodities+Prices+Solution.sql;

Tech Stack
Database: MySQL (compatible with other SQL databases with minor adjustments)
Data Model: Relational (Commodities ↔ Regions ↔ Prices)
SQL Concepts: Joins, Aggregations, Window Functions, CTEs, Views

Example Insights
Identify commodities consistently expensive across years.
Track price fluctuations across states and cities.
Measure availability diversity by commodity.
Spot high variation commodities to study market volatility.

Next Steps
Expand dataset with more years and regions.
Build BI dashboards (Power BI/Tableau) for visualization.
Automate ETL pipeline to refresh data periodically.
