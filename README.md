E-Commerce Product File Handling System
📌 Overview

This project simulates a real-world e-commerce product management system using Python and file handling.
It demonstrates how product data is stored, processed, updated, and saved using three widely used file formats: CSV, JSON, and TXT.

The system manages:

Sales data for each product (14-day sales history)

Product details such as name, brand, price, and specifications

Product descriptions stored as text files

Each product is identified using a unique SKU (Stock Keeping Unit), which links data across all file types.

The project allows users to:

Load product data from files

Add new products or update existing ones

Save the updated data back into structured files

This reflects how real companies manage product information, sales records, and inventory data in data engineering and analytics workflows.

📂 Data Structure

The dataset is organized in the following format:

mainfolder
│
├── sales_data.csv
├── product_details/
│     ├── details_<SKU>.json
├── product_descriptions/
│     ├── description_<SKU>.txt


Each product is identified using a unique SKU (Stock Keeping Unit).

🧩 File Types Used
File Type	Purpose
CSV	Stores 14 days of sales data for each product
JSON	Stores product details like name, brand, price, and availability
TXT	Stores product descriptions

⚙️ Project Workflow
Stage 1 – Load Data

CSV, JSON, and TXT files are read from the main folder

Data is loaded into Python dictionaries:

sales_data

product_details

product_descriptions

Stage 2 – Update Data

The system allows:

Adding a new product

Updating an existing product

The update() function collects:

SKU

14-day sales data

Product name, brand, model, price, and availability

Product description

All this information is stored in Python dictionaries.

Stage 3 – Save Data

The dump_data() function writes all updated data back into files:

Sales data → sales_data.csv

Product details → JSON files

Product descriptions → TXT files

The original folder structure is maintained.

🛠 Technologies Used

Python

CSV file handling

JSON file handling

Text file handling

OS module for file and folder management

🎯 What This Project Demonstrates

Real-world file handling

Data loading and transformation

ETL-style processing

Structured storage of business data

This project reflects how data is handled in e-commerce platforms and data engineering pipelines.
