# 📂 **Data Folder Documentation**

This folder contains the data files and associated details for the **E-commerce Dashboard Project Using Power BI**. The dataset is a combination of multiple CSV files joined and enriched with additional columns to facilitate insightful analysis.

---

## 📄 **Data Files**

### 1. **Original CSV Files**
The following CSV files were used to create the dataset:
- **Customers_Large.csv**: Contains customer information such as Customer ID, , Name and Segment.
- **Orders_Large.csv**: Includes order details like Transaction ID, Product IDs, Order date, and Customer ID.
- **Products_Large.csv**: Provides product details such as Product ID, Name, Category, and Price.
- **Sales_Large.csv**: Contains sales transactions, including order IDs,Tax, Discount, and Revenue.

### 2. **Combined Dataset**
- **Dataset.csv**: This is the final merged dataset created by joining the original CSV files. It includes additional calculated columns for enhanced analysis.

---

## 🆕 **Newly Added Columns**

### **1. `Dataset[Profit]`**
- **Description**: The calculated profit for each transaction.
- **Formula**: `Profit = Revenue - (Cost+Tax)`

### **2. `Dataset[Profit Margin]`**
- **Description**: The profit margin as a ratio of discount and revenue.
- **Formula**: `Profit Margin = Profit / Revenue`

### **3. `Dataset[Discount_Impact]`**
- **Description**: Represents the effect of discounts on sales.
- **Formula**: `Discount Impact = Discount / Revenue`

### **4. `Dataset[Popularity]`**
- **Description**: A custom metric to measure the popularity of products (Low, Medium, High) based on sales volume.

---

## 🔧 **How to Use**

1. **Data Source**:
   - All individual CSV files are available in 📂 Original Data and the combined `Ecommerce_Sales_Data.xlsx` is available in the 📂 Data folder.
   - Use the files as inputs for analysis in Power BI or any other analytics tool.

2. **Integration**:
   - The `Ecommerce_Sales_Data.xlsx` file can be directly imported into Power BI for creating dashboards and reports.
   - Original CSV files are retained for flexibility and data lineage.

---

## 📂 **Folder Structure**
```
├── Ecommerce_Sales_Data.xlsx  # Final combined dataset with new columns
   📂 Original Data/
   ├── Customers_Large.csv     # Original customer data
   ├── Orders_Large.csv        # Original order data
   ├── Products_Large.csv      # Original product data
   ├── Sales_Large.csv         # Original sales data
```
---
