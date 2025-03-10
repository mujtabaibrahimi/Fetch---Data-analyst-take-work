# Data Cleaning and Analysis with SQLite

## Overview
This project performs data cleaning and analysis on three datasets: Users, Transactions, and Products. The cleaned data is stored in an SQLite database, and multiple SQL queries are executed to extract insights.

## Datasets
The following CSV files are used in this project:
- `USER_TAKEHOME.csv`: Contains user information including birth dates and states.
- `TRANSACTION_TAKEHOME.csv`: Contains transaction details such as purchase dates and final sale amounts.
- `PRODUCTS_TAKEHOME.csv`: Contains product information such as brand and category.

## Data Processing Steps
1. **Load the data**: Read the CSV files into Pandas DataFrames.
2. **Convert date fields**: Convert date columns to proper datetime format.
3. **Convert numeric fields**: Ensure numeric fields are properly formatted.
4. **Handle missing values**: Fill missing categorical values with 'Unknown'.
5. **Save cleaned data**: Store cleaned data in new CSV files.
6. **Store data in SQLite**: Load the cleaned data into an SQLite database.
7. **Execute SQL queries**: Run predefined SQL queries for data analysis.

## SQL Queries Executed
The following queries provide insights into user and transaction behavior:

1. **Top 5 Brands by Receipts Scanned (Users 21+)**
   - Identifies the top 5 brands based on the number of scanned receipts for users aged 21 and above.

2. **Top Brand in 'Dips & Salsa' Category**
   - Determines the most frequently purchased brand in the 'Dips & Salsa' category.

3. **Identifying Fetch’s Power Users**
   - Finds the top 10 users with the highest spending and the most receipts scanned.

4. **Generation-wise Sales Percentage in 'Health & Wellness'**
   - Categorizes users into generations (Gen Z, Millennials, Gen X, Boomers & Older) and calculates the percentage of sales they contribute to the 'Health & Wellness' category.

## How to Run the Project
1. Ensure Python is installed along with the required libraries:
   ```bash
   pip install pandas sqlite3
   ```
2. Place the CSV files inside the `data/` directory.
3. Run the script (`main.ipynb` or `main.py`).
4. View the generated `CLEANED_USERS.csv`, `CLEANED_TRANSACTIONS.csv`, and `CLEANED_PRODUCTS.csv`.
5. Check the SQLite database `mystore.db` for structured data storage.
6. Review the SQL query results printed in the console.

## Output
- Cleaned CSV files: `CLEANED_USERS.csv`, `CLEANED_TRANSACTIONS.csv`, `CLEANED_PRODUCTS.csv`
- SQLite database: `mystore.db`
- SQL query results printed in the terminal

## Author
Developed by Muhammad Mujtaba.

## License
This project is for educational and analytical purposes only.

