# Data Transformation and Cleaning Logic (Power Query / M)

This document outlines the key data cleaning and transformation steps applied directly in the Power Query Editor to satisfy the project's data cleanup requirements and ensure a robust analysis.

## Core Data Integrity Filtering
The following checks were implemented in Power Query to clean the data before loading, ensuring error-free analysis:

⦁	Filtered for Positive Quantity: Applied a filter to the [Quantity] column to keep only values greater than or equal to one ($\ge 1$)

⦁	Rationale: This step removes all rows that represent returns or reversed transactions (negative quantities) and any data errors where quantity was zero, ensuring accurate revenue totals.

⦁	Filtered for Valid Unit Price: Applied a filter to the [UnitPrice] column to keep only values greater than zero ($\ge \$0.01$).

⦁	Rationale: This step removes entries with a unit price of zero or less, which are typically data input errors, as specified in the task.

⦁	Removed Blank Customer IDs: Applied a filter to exclude any rows where the [CustomerID] was blank.

⦁	Rationale: This ensures all transactions used in customer-based analysis (like identifying the Top 10 Customers) are tied to a valid customer, supporting the requirements for Question 3.
	
## Feature Engineering
⦁	Date Conversion: Ensured the [InvoiceDate] column was correctly set as a Date/Time type.

⦁	Numeric Conversion: Confirmed [Quantity] and [UnitPrice] were set to Decimal Number type.





