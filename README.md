# E-commerce Data Processing in Databricks with Delta Tables

A PySpark-based data processing pipeline developed in Databricks for handling and managing e-commerce order data. This project utilizes Delta Lake for efficient upsert operations, error handling, and inventory management, offering a scalable ETL solution for e-commerce data stored in Delta tables.

## Project Structure

- **`orders_notebook.ipynb`**: Main Jupyter Notebook containing the full code implementation and results. Check the code here: [`orders_notebook.ipynb`](orders_notebook.ipynb).
- **`data/initial_inventory.json`**: JSON file with the initial inventory setup.  
   https://github.com/rodrigo85/databricks_delta_table/blob/7cbca1b5fa92d38bd8f0a430a053c43b6ca072af/data/initial_inventory.json#L1-L15
  
- **`data/orders.json`**: JSON file containing sample order data.  
   https://github.com/rodrigo85/databricks_delta_table/blob/7cbca1b5fa92d38bd8f0a430a053c43b6ca072af/data/orders.json#L1-L50

## Key Functionalities

1. **Delta Upsert (Merge)**: This function merges source data with existing Delta tables, allowing for incremental data loads.
2. **Order Data Extraction and Flattening**: Extracts and flattens order-related data for streamlined processing.
3. **Inventory Management**: Automatically adjusts inventory levels based on processed order data.
4. **File Handling**: Moves processed files to a different directory, managing processed data and storage efficiently.

## Example Code

Refer to the notebook for code implementation: [`orders_notebook.ipynb`](orders_notebook.ipynb).
