# Power BI Data Modeling Project  

- Built a **star-schema data model** by transforming complex source tables into fact and dimension tables.  
- Analyzed **table grain, relationships, and data requirements** to structure the model for reliable reporting.  
- Applied **data modeling standards,** including naming conventions, surrogate keys, and removal of unnecessary columns.  
- Created a **Date dimension and core DAX measures** for the business, and validated key figures to ensure data accuracy.  
- Applied **Row-Level Security (RLS)** and performed final model validation.  

## Starting Point: Chaotic Data Model  
 
- Many to many relationships 
- Filters going to both directions
- No star-schema
- No sense

### [Download the dataset](./dataset.xlsx)

![Chaotic Data Model](/Images/0_chaos.png)  

## Final output: Clean Data Model  

- Star-schema  
- Facts surrounded by dimensions  
- Right relationships  
- Filters going to the right direction  
- Numbers are protected  
- Everything is friendly and easy to read  

### [Download the Power BI file with clean data model](./data_model_project.pbix)  

![Clean Data Model](/Images/Clean_Data_Model.png)  

## Data Modeling Process  

![Data Modeling Process](/Images/1_Process.jpg)  

## Rules  
1. **Build a star schema:** A **fact** in the middle, dimensions around it
2. **Understand before you change:** Always read the **grain** first
3. **Every column earns its place:** If it doesn't help the report, **drop it**
4. **Protect the numbers:** Know your totals, **re-check** after every change

## Standards
- **Language:** English 
- **Naming:** snake_case (customer_name, order_date)
- **Tables:** fact_ dim_ (fact_sales, dim_products)
- **Keys:** _key _id (customer_key, customer_id)  

## Polish  
- **Connect dim_date:** Almost every fact needs a date
- **Measures:** The obvious ones every model needs
- **Secure the model:** Apply row-level security
- **Check the big numbers:** The ones you already know by heart
- **Hand it over:** Give them the guide, and let them run it
