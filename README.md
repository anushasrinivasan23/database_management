
### ** Building a Relational Database for Bird Strike Insights with MySQL and R**

---

### **Overview**
This project involves analyzing bird strikes on aircraft using the FAA dataset. The goal is to build a MySQL relational database, load the data, and perform SQL queries and analysis through R.

---

### **Project Setup**

#### **Prerequisites**
- **Environment**: RStudio with an R Project for this practicum.
- **Dependencies**:
  - R packages: `DBI`, `RMySQL`, `tidyverse`, `ggplot2` (or base R plot functions).
  - MySQL (freemysqlhosting.net).
- **Files**:
  - `BirdStrikesData.csv` (FAA dataset file).
  - `BuildingRDB.Rmd` (R Notebook file).

---

### **How to Run the Project**
1. **Setup Cloud MySQL**:
   - Configure a MySQL database on freemysqlhosting.net.
   - Note the host, username, password, and database name for connection.
   
2. **Open the R Project**:
   - Place all files, including the `.Rmd` and `BirdStrikesData.csv`, in the same folder.
   - Open the `.Rmd` file in RStudio.

3. **Run the Code**:
   - Ensure all code chunks are properly executed in order.
   - Follow the headers and comments in the `.Rmd` file to navigate each task.

4. **Check Results**:
   - Validate the created database schema.
   - Confirm data loading and run the provided SQL queries.
---

### **Key Sections**

#### **Database Configuration**
- A cloud-based MySQL database is set up with required tables (`flights`, `airports`, `strikes`, `conditions`).
- Relational schema implements primary and foreign keys.
- Tables are populated using data from `BirdStrikesData.csv`.

#### **Queries and Analysis**
- **Top Airports with Strikes**: Identifies states with the highest number of bird strikes.
- **Analysis by Airline**: Highlights airlines with above-average bird strike incidents.
- **Analysis by Month**: Summarizes incidents by month, providing insights into seasonal trends.

#### **Visualizations**
- Vertical bar charts or horizontal bar plots for trends.
- Visualization of bird strikes by month or by total birds.

#### **Stored Procedure**
- A MySQL stored procedure removes strikes by their primary key and logs the removal in an audit log.

---

### **Outputs**
1. **Database**:
   - A fully operational relational database with FAA bird strike data.
2. **Queries**:
   - SQL results for airports, airlines, and monthly trends.
3. **Visualizations**:
   - Charts showcasing key trends and insights.
4. **Stored Procedure**:
   - Logs of removed incidents in the audit log table.
