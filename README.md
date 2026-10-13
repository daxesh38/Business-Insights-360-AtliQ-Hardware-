# Business Insights 360 (BI 360) – Power BI & MySQL Enterprise Analytics Dashboard

[![Live Dashboard](https://img.shields.io/badge/Power_BI-Live_Interactive_Report-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://app.powerbi.com/view?r=eyJrIjoiNDQ5ZWEzMDYtMjE1NS00NzVhLWIyNzctNTEwNzk2Y2Y2ZWQ5IiwidCI6IjY2ZGNhNGQyLTU0ZDktNDhiOC1hZDFhLTliOWUwNmRiMGQ5MCJ9)
[![Download PBIX](https://img.shields.io/badge/Google_Drive-Download_.pbix-4285F4?style=for-the-badge&logo=googledrive&logoColor=white)](https://drive.google.com/file/d/1_4XIt_YLY6jvAv6pWnoONbNhaKcb9nhM/view?usp=sharing)
[![MySQL](https://img.shields.io/badge/MySQL-Database_Connected-4479A1?style=for-the-badge&logo=mysql&logoColor=white)](https://www.mysql.com/)

---

## 🔗 Quick Project Links
* 🌐 **Live Interactive Report:** [Open Dashboard in Power BI Service](https://app.powerbi.com/view?r=eyJrIjoiNDQ5ZWEzMDYtMjE1NS00NzVhLWIyNzctNTEwNzk2Y2Y2ZWQ5IiwidCI6IjY2ZGNhNGQyLTU0ZDktNDhiOC1hZDFhLTliOWUwNmRiMGQ5MCJ9)
* 📥 **Download .PBIX File:** [Download from Google Drive](https://drive.google.com/file/d/1_4XIt_YLY6jvAv6pWnoONbNhaKcb9nhM/view?usp=sharing)

---

## 🏢 Business Problems Faced by AtliQ Hardware
Before this Business Intelligence solution was implemented, AtliQ Hardware faced several operational and analytical bottlenecks:

1. **Spreadsheet Dependency & Data Silos:** Departments (Finance, Sales, Marketing, Supply Chain) relied on manual, disconnected Excel sheets, leading to version control issues and data mismatches.
2. **Lack of 360° Visibility:** Leadership lacked a single source of truth to view company-wide performance across regions, markets, and segments.
3. **Unexpected Profit Loss:** Despite healthy top-line gross sales, heavy post-invoice discounts, shipping costs, and operational expenses led to unexpected negative net profit margins.
4. **Supply Chain Inaccuracies:** Inaccurate demand forecasting led to excessive inventory carrying costs in some regions and frequent stockouts in others.
5. **Slow Decision-Making:** Static monthly reports made it impossible for regional directors and sales managers to track targets vs. actuals dynamically in real-time.
6. **No Clear Customer/Product Profitability Matrix:** Sales teams couldn't quickly identify which customers and products drove true profit margins versus those eating into margins with heavy discounts.

---

## 💡 How BI 360 Solves These Problems
* **Single Source of Truth:** Direct integration with an enterprise **MySQL database** and **Star Schema** data modeling unifies transactions, targets, and operational metrics into one automated system.
* **Transparent Unit Economics & P&L:** Built an interactive P&L breakdown to track value leakage at every step—from Gross Sales through Deductions, COGS, and Operational Expenses down to Net Profit.
* **Proactive Inventory Risk Classification:** Automated demand forecasting metrics classify products and customers into **Out-Of-Stock (OOS)** and **Excess Inventory (EI)**, allowing the supply chain team to mitigate risks before stockouts occur.
* **Dynamic Benchmarking:** Instant slicing across **YTD, YTG, vs Last Year (vs LY), and vs Target** across all organizational tiers.

---

## 🖥️ Dashboard Pages & Detailed Walkthrough

### 1. Home Page (Navigation Hub)
The landing page serves as the user-friendly entry point, providing seamless navigation to each dedicated functional view alongside report refresh details and quick user guide resources.

![Home Page](Images/Home%20Page.png)

---

### 2. Executive View
* **What Problem It Solved:** Eliminated the need for executives to read multiple departmental reports by providing a consolidated, high-level summary of company health.
* **Key Insights:**
  * Displays top-level KPIs: **$3.74B Net Sales**, **38.08% Gross Margin**, **-13.98% Net Profit**, and an overall **81.17% Forecast Accuracy**.
  * Highlights revenue distribution by division (**PC: 61.33%**, **P & A: 36.18%**, **N & S: 2.49%**) and channel (**Retailer: 71.53%**, **Direct: 17.8%**, **Distributor: 10.67%**).
  * Pinpoints regional performance across sub-zones with market share tracking against competitors.

![Executive View](Images/Executive%20View%20Page.png)

---

### 3. Finance View
* **What Problem It Solved:** Uncovered hidden cost drivers and margin leakages across pre-invoice deductions, post-invoice discounts, freight, and operating expenses.
* **Key Insights:**
  * Houses a complete **Profit and Loss (P&L) Statement** dynamically comparable against benchmarks and previous years.
  * Reveals that out of **$7,370M Gross Sales**, deductions and COGS leave **$1,422.88M Gross Margin (38.08%)**, while operational expenses of **$1,945.30M** result in a net profit deficit of **-$522.42M**.
  * Slices P&L figures across segments, regions, and monthly time-trend curves.

![Finance View](Images/Finance%20View%20Page.png)

---

### 4. Marketing View
* **What Problem It Solved:** Solved ambiguity regarding which product segments and geographic markets drive sustainable profit versus those with unsustainable operating costs.
* **Key Insights:**
  * Breaks down performance across Notebooks, Desktops, Peripherals, Accessories, Storage, and Networking.
  * Shows that **Notebooks** lead total Net Sales (**$1,580.43M**), followed by **Peripherals** (**$897.54M**).
  * Features an interactive **Performance Matrix** and **Unit Economics Waterfall Chart** illustrating the transition from Gross Margin to Net Profit across product categories.

![Marketing View](Images/Marketing%20View%20Page.png)

---

### 5. Sales View
* **What Problem It Solved:** Helped sales managers stop giving excessive discounts by evaluating customer revenue directly against Gross Margin percentage.
* **Key Insights:**
  * Tracks performance across top key accounts including **Amazon ($496.88M Net Sales)**, **AtliQ Exclusive ($361.12M)**, and **Flipkart ($138.49M)**.
  * Scatter plot matrix maps customer volume against Net Profit %, identifying high-margin versus high-volume clients.
  * Unit economics split details pre-invoice and post-invoice deduction impacts per customer segment.

![Sales View](Images/Sales%20View%20Page.png)

---

### 6. Supply Chain View
* **What Problem It Solved:** Replaced manual inventory guesswork with data-driven demand planning, directly addressing excess warehouse storage costs and product stockouts.
* **Key Insights:**
  * Monitors **Forecast Accuracy (81.17%)**, **Net Error (-3.47M units)**, and **Absolute (ABS) Error (6.89M units)**.
  * Classifies customer and product-level fulfillment risk into **OOS (Out of Stock)** and **EI (Excess Inventory)**.
  * Shows **Networking** achieves the highest forecast accuracy (**93.06%**), while **Peripherals (68.17%)** and **Storage (71.50%)** present significant out-of-stock risk requiring operational adjustments.

![Supply Chain View](Images/Supply%20Chain%20View%20Page.png)

---

## 🎓 Course Certification & Acknowledgments
A heartfelt thank you to **Codebasics**, **Dhaval Patel** sir, and **Hemanand Vadivel** sir for creating the industry-grade *"Get Job Ready: Power BI Data Analytics for All Levels 4.0"* program. 

The practical, business-centric approach of this course provided me with end-to-end expertise in relational data modeling, advanced DAX, and stakeholder-driven dashboard design.

### 📜 Certificate of Completion
*(GUID: CB-49-300709)*

You can view the full certificate document in the repository:
📄 [Download Certificate PDF](Certificate/CB-49-300709.pdf)

---

## 📬 Connect With Me
* 💼 **LinkedIn:** [daxesh-patel-0a451a294](https://www.linkedin.com/in/daxesh-patel-0a451a294/)
* 🐙 **GitHub:** [daxesh38](https://github.com/daxesh38)
