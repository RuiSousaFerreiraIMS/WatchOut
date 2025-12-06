# WatchOut

## How to run the WatchOut database in MySQL Workbench

1. **Open MySQL Workbench**  
   Launch MySQL Workbench and connect to your MySQL server (e.g., `Local instance MySQL`).

2. **Open a new SQL editor tab**  
   Go to **File → Open SQL Script…** and select the file `watchout_schema.sql` (this file contains all `CREATE DATABASE`, `CREATE TABLE` and `INSERT` statements).  
   Alternatively, you can open a blank tab with **File → New Query Tab** and paste the contents of the script.

3. **Execute the script**  
   Make sure you are connected to the server, then click the **Execute** button (yellow lightning icon) to run the entire script.  
   The script will:
   - Drop and recreate the `watchout` database (if it already exists)  
   - Create all tables (Customer, Product, OrderHeader, OrderItem, Employee, SalaryHistory, etc.)  
   - Insert sample data for testing

4. **Verify the schema and tables**  
   In the **SCHEMAS** panel on the left:
   - Right-click and choose **Refresh All**  
   - Expand the `watchout` schema  
   - Check that all tables were created successfully

5. **Run custom queries**  
   Open a new query tab, select the `watchout` schema as default (right-click → **Set as Default Schema**), and write your own `SELECT`, `JOIN`, `GROUP BY`, etc., to explore the data.

6. **(Optional) View the ERD**  
   If you are using the MySQL Workbench model file (`.mwb`), you can open it via **File → Open Model…** to see the full ERD with all relationships (PK/FK) between the tables.
