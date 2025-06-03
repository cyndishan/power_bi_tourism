# ☕ Tourism Report — Power BI Project

Welcome to my Power BI showcase project: **Tourism Report**. This report provides a clear and detailed look at key metrics and visualizations around revenue, visitor numbers, and customer satisfaction, making it an essential resource for stakeholders.

---

## 📊 Report Overview

This interactive Power BI report includes the following visualizations:

1. **Key Metrics Cards**- An overview of total revenue, total visits and average customer satisfactory.
2. **Pie Chart** — Displays the proportion of total revenue contributed by each region.
3. **Line Chart** — Tracks monthly revenue and customer satisfactory trends.
4. **Clustered Column Chart** — Shows distribution of tourist visits within different regions.
5. **Line Chart** — Shows trend of average tourist visits each month.

---

### 🔎 Slicers
- **Region** 
- **Month**

---


## ✅ Problem Solved: Incorrect Weekday Order

Power BI by default sorts month names alphabetically (e.g., Apr before Jan), which can distort trends in several charts.

To solve this, I created a **separate Month Table** with a `MonthSort` column. I then sorted Month names (e.g., "Jan", "Feb") by this numeric column to ensure charts display the **correct calendar order** from Jan to Dec.

```DAX
MonthTable = DATATABLE(
    "Month", STRING,
    "MonthSort", INTEGER,
    {
        {"Jan", 1},
        {"Feb", 2},
        {"Mar", 3},
        {"Apr", 4},
        {"May", 5},
        {"Jun", 6},
        {"Jul", 7},
        {"Aug", 8},
        {"Sep", 9},
        {"Oct", 10},
        {"Nov", 11},
        {"Dec", 12}
    }
)
```

---

## 🖼️ Report Screenshot

Here’s a preview of the full Power BI report:

![image](https://github.com/user-attachments/assets/92ec115f-9280-463e-bf13-bd41a3ba3dc1)


---

## 📈 Key Insights

- 1. In general, tourism generated $2M in revenue from 42K visits, with an average customer satisfaction of 4.22. While visitation and revenue are relatively strong, satisfaction scores indicate opportunities to improve the visitor experience.
- 2. Revenue peaks in July and August, closely followed by a rise in customer satisfaction. However, satisfaction begins to drop in August, while revenue declines sharply from September onward. This lag suggests that during peak months, visitor experience may be strained, possibly due to crowding or overstretched services. The decline in satisfaction could lead to a delayed drop in repeat visits and overall revenue.
- 3. Tourist visits increase steadily from May to a sharp peak in August, then decline. January to April remain the lowest in terms of average visits. The peak aligns with school holidays and seasonal travel trends. However, reliance on a narrow peak season presents operational risks and missed opportunities during off-peak periods.
- 4. West (24.97%), South (23.9%), and North (20.21%) dominate total revenue, while East contributes only 13.32%. The underperformance of the East and Central regions may stem from fewer attractions, weaker branding, or lower visitor satisfaction. 
- 5. South and West lead in average visits, reflecting stronger regional appeal or infrastructure. East trails behind, mirroring its revenue share. There is a direct correlation between tourist visits and revenue. To boost underperforming regions, we should consider improving access, visibility, and offerings.
---

## 💡 Actionable Recommendations

- Boost Low-Performing Regions: Targeted investment in infrastructure, partnerships, and regional branding campaigns is key to unlocking potential in East and Central.
- Monitor and Align Performance: Create an early-warning KPI dashboard to monitor customer satisfaction in real-time during peak months.

---

## 🛠 Tools Used

- **Power BI Desktop**
- **Power Query Editor**
- **DAX (Data Analysis Expressions)**
- **CSV file as data source**

---

## 📂 Files

- `Tourism_report.pbix` — Main Power BI dashboard file
- `Tourism_Data.csv` — Source dataset 

---

## 📌 About This Project

This project was created as part of my data analytics portfolio to demonstrate:

- Data modeling and cleaning in Power BI
- Time-based sorting using custom MonthTable
- Effective use of slicers 
- Extracting actionable business insights from tourism data
- Professional data storytelling for non-technical stakeholders

---

## 🔗 Contact

**Cyndi Li Shan** — Aspiring Data Analyst  
📧 Email: [cyndi.shan0101@gmail.com]  
🌐 Portfolio: [[github]](https://github.com/cyndishan)
💼 LinkedIn: [[LinkedIn]](https://www.linkedin.com/in/cyndi-li-shan/)
