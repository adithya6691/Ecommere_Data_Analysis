
# 🛒 E-Commerce Data Analysis using MySQL & Python

This project demonstrates the end-to-end process of building and analyzing an **E-commerce transactional database**.  
Using **Python (Pandas)** for data preparation and **MySQL** for analytics, it extracts key insights into sales performance, customer behavior, and seller performance.

---

## 🎯 Project Objective

The goal of this project is to analyze a real-world E-commerce dataset to uncover business insights such as:

- Trends in orders and revenue over time  
- Customer purchase behavior and retention  
- Seller performance and revenue contribution  
- Product category analysis and profitability metrics  
- Growth and sales forecasting indicators  

---

## 🧰 Tools & Technologies

- **Programming Language:** Python  
- **Database System:** MySQL  
- **Libraries:** Pandas, MySQL Connector  
- **Environment:** Jupyter Notebook / VS Code  

**##Dataset link**
https://drive.google.com/drive/folders/11B3D7nZDlMpIrautqhB94E5AWz5Q9S_0?usp=drive_link

## 🗄️ Database Design

The relational database was designed to represent a complete E-commerce ecosystem.  
It consists of interconnected tables covering customer, order, product, payment, and seller data.

- **Customers:** Contains customer IDs, location (city, state), and demographic information.  
- **Orders:** Stores details of each purchase including timestamps and order status.  
- **Order_Items:** Captures item-level details such as price, quantity, and freight value.  
- **Products:** Holds product categories and item descriptions.  
- **Payments:** Tracks payment method, installments, and transaction amounts.  
- **Sellers:** Contains information about each seller’s identity and location.  
- **Geolocation:** Maps postal codes to city and state for geographic segmentation.

These tables are connected through primary and foreign key relationships, allowing for seamless analytical queries across multiple dimensions.

---

## ⚙️ Data Integration Workflow

1. **Data Extraction:**  
   CSV files containing raw transactional data were imported using Python.

2. **Data Transformation:**  
   Data was cleaned, column names standardized, and missing values handled using Pandas.

3. **Schema Generation:**  
   The script automatically inferred data types and created SQL tables dynamically in MySQL.

4. **Data Loading:**  
   All cleaned data was inserted into the database for efficient querying and analysis.

---

## 📊 Key SQL Analyses

The project covers a wide range of analytical queries, divided by insight level:

### 🧩 Descriptive Analysis
- Identify all unique cities with active customers.  
- Count total orders placed in a specific year.  
- Measure total and average sales per product category.  
- Analyze installment-based payment behavior.  
- Count customers per geographic region.

### 📈 Diagnostic & Trend Analysis
- Monthly order trends for specific years (e.g., 2018).  
- Average number of items purchased per order by city.  
- Revenue contribution by product category.  
- Seller-wise total revenue and ranking.  
- Correlation between product price and sales frequency.

### 🔍 Predictive & Advanced Insights
- Moving average of customer order values over time.  
- Cumulative sales per month across years.  
- Year-over-year revenue growth rate.  
- Customer retention rate (repurchases within six months).  
- Identification of top three high-value customers each year.

### ⚙ How to Run the Project

1. *Clone this repository:*
   bash
   git clone https://github.com/<your-username>/Ecommerce-Analysis.git
   cd Ecommerce-Analysis

2. **Download the dataset** from the [Google Drive link](https://drive.google.com/drive/folders/129lQLqWlkeAyD1Zr8MXJwohelMQ9UUei?usp=drive_link)
   and place all CSV files in your local project folder.

3. **Edit your MySQL credentials** in `csvtosql.py`:

   python
   conn = mysql.connector.connect(
       host='localhost',
       user='root',
       password='yourpassword',
       database='db_p'
   )
4. **Run the script** to load data into MySQL:

   bash
   python csvtosql.py
   

5. *Open and run the Colab notebook* (ec_analysis_d.ipynb) or refer to the included PDF for all queries and visualizations.

## 💡 Business Insights

- **Sales Trends:** Orders and revenue show seasonal fluctuations, with peak months identified for key campaigns.  
- **Customer Behavior:** Certain states and cities account for a major portion of total purchases.  
- **Payment Insights:** A significant percentage of customers prefer installment-based payments.  
- **Seller Ranking:** Top-performing sellers contribute disproportionately to total sales.  
- **Growth & Retention:** Positive year-over-year growth with measurable repeat purchase rates.  

---

## 🔍 Future Enhancements

- Integration with **Tableau** or **Power BI** for interactive dashboards.  
- Implementation of **predictive analytics** using Python (e.g., purchase forecasting).  
- Addition of **data quality checks** and error logging in the ETL pipeline.  
- Building a **data warehouse model** for advanced business intelligence.

---

## 👤 Author

**Adithya**  
📊 Data Analyst | SQL | Python | Tableau  
🔗 https://www.linkedin.com/in/adithya-senguttuvan-36923863/  



---

⭐ *If this project helped you learn or inspired your work, please give it a star on GitHub!*
