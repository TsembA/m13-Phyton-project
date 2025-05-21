# Inventory Data Automation with Python & Excel

## Overview

This project utilizes Python and the `openpyxl` library to automate inventory analysis in an Excel spreadsheet. It processes product data, calculates summary statistics per supplier, identifies products with low stock, and adds a column for the total value of the inventory per product. The resulting updated file is saved as a new Excel sheet.

## Key Features

- **Data Input**: Reads product data from an Excel file (`inventory.xlsx`) in `Sheet1`.
- **Supplier Analysis**:
  - Counts the number of products each supplier provides.
  - Calculates the total inventory value per supplier (inventory × price).
- **Low Stock Detection**:
  - Identifies and lists products with inventory less than 10 units.
- **Data Augmentation**:
  - Adds a new column for the total value per product (inventory × price) in the Excel sheet.
- **Output File**: Saves the updated data to a new Excel file named `inventory_with_total_value.xlsx`.

## Technologies Used

- **Programming Language**: Python 3
- **Libraries**: `openpyxl` for reading and writing Excel files.
- **File Type**: Excel `.xlsx`

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/inventory-data-automation.git
    ```

2. **Navigate to the project directory**:
    ```bash
    cd inventory-data-automation
    ```

3. **Install dependencies**:
    Ensure you have Python 3 installed, and then install the required libraries:
    ```bash
    pip install -r requirements.txt
    ```

    If you don't have `requirements.txt`, you can manually install `openpyxl` with:
    ```bash
    pip install openpyxl
    ```

## Usage

1. Ensure your Excel file (`inventory.xlsx`) is in the same directory as the script.
2. Run the Python script:
    ```bash
    python inventory_data_automation.py
    ```

3. After running the script, a new Excel file (`inventory_with_total_value.xlsx`) will be generated with:
    - Total inventory value per product.
    - Supplier product count.
    - List of products with less than 10 units in stock.

## Sample Data

### Input Example (`inventory.xlsx`)

| Product ID | Inventory | Price | Supplier Name | Total Value |
|------------|-----------|-------|---------------|-------------|
| 1          | 15        | 25.00 | Supplier A    |             |
| 2          | 8         | 40.00 | Supplier B    |             |
| 3          | 25        | 10.00 | Supplier A    |             |

### Output Example (`inventory_with_total_value.xlsx`)

| Product ID | Inventory | Price | Supplier Name | Total Value |
|------------|-----------|-------|---------------|-------------|
| 1          | 15        | 25.00 | Supplier A    | 375.00      |
| 2          | 8         | 40.00 | Supplier B    | 320.00      |
| 3          | 25        | 10.00 | Supplier A    | 250.00      |


## Benefits

- **Efficiency**: Automates repetitive calculations, saving time.
- **Financial Tracking**: Easily tracks inventory value and total stock by supplier.
- **Low Stock Monitoring**: Flags products with low stock levels to facilitate reordering.
- **Business Optimization**: Helps businesses make informed decisions about inventory management.

