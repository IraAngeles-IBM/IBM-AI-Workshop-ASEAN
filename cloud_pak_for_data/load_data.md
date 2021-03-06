# DB2 Warehouse

## Load Data 

1. Download the following files from this Github [repository](https://github.com/IraAngeles-IBM/IBM-AI-Workshop-ASEAN/tree/master/cloud_pak_for_data/assets):

    - billing.csv
    - products.csv
    - customer-serivce.csv

2. Select **Load** from File in the Menu:

    ![load from file](images/load_from_file.png)

3. Select source **billing.csv** file

    ![load billing csv](images/load_billing_csv.png)

4. Choose the target, **create a new table and load**, then click **next**

    ![load billing csv](images/create_new_table.png)

5. Define or verify the suggested table definition, then click **Finish**

    ![load billing csv](images/table_definition.png)

6. Load complete for **billing.csv**, click on **Load more Data** to load **products.csv** and **customer-service.csv**, repeating steps 2 to 6.

    ![load billing csv](images/load_billing_complete.png)

7. To run **SQL**, go to menu -> **Run SQL** and type the following SQL command:

    ```
    SELECT CUSTOMERID,CONTRACT,PAPERLESSBILLING,PAYMENTMETHOD,MONTHLYCHARGES,TOTALCHARGES,CHURN
    FROM BLUADMIN.BILLING;
    ```

    ![load billing csv](images/db2_warehouse_sql_loop.gif)

    