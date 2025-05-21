# 📊 Inventory Data Automation with Python & Excel

## 🧾 Overview

This project uses Python and the `openpyxl` library to automate inventory analysis in an Excel spreadsheet. It processes product data, calculates supplier statistics, identifies low-stock items, and adds a total value column for each product.

✅ Reads Excel data  
✅ Computes inventory value per supplier  
✅ Detects products with low inventory  
✅ Saves enriched data to a new Excel file

---

## 🛠️ Key Features

- 📥 **Reads from** `inventory.xlsx` (Sheet1)
- 📦 **Counts products per supplier**
- 💰 **Calculates total inventory value** per supplier
- ⚠️ **Flags low stock** items (< 10 units)
- 💾 **Writes total value** per product into Excel
- 🗂 **Saves results to** `inventory_with_total_value.xlsx`

---

## 🧰 Technologies Used

- 🐍 Python 3
- 📘 `openpyxl` library
- 📁 Excel `.xlsx` format

---

## 🚀 Getting Started

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/inventory-data-automation.git
    cd inventory-data-automation
    ```

2. **Install dependencies**:
    ```bash
    pip install openpyxl
    ```

3. **Run the script**:
    ```bash
    python inventory_data_automation.py
    ```

---

## 📄 Sample Data

### Input (`inventory.xlsx`)

| Product ID | Inventory | Price | Supplier Name | Total Value |
|------------|-----------|-------|---------------|-------------|
| 1          | 15        | 25.00 | Supplier A    |             |
| 2          | 8         | 40.00 | Supplier B    |             |
| 3          | 25        | 10.00 | Supplier A    |             |

### Output (`inventory_with_total_value.xlsx`)

| Product ID | Inventory | Price | Supplier Name | Total Value |
|------------|-----------|-------|---------------|-------------|
| 1          | 15        | 25.00 | Supplier A    | 375.00      |
| 2          | 8         | 40.00 | Supplier B    | 320.00      |
| 3          | 25        | 10.00 | Supplier A    | 250.00      |

---

## 💡 Benefits

- ⏱ **Saves time** by automating repetitive Excel calculations
- 📈 **Tracks inventory value** for each supplier
- 🛎 **Alerts on low stock** to prevent supply chain delays
- 🧹 **Cleans up your workflow** with a single script
