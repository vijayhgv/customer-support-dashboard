# 📊 Customer Support Ticket Analysis Dashboard

An interactive **Power BI dashboard** built to analyse 8,469 customer support tickets and uncover key insights around SLA performance, resolution efficiency, and customer satisfaction.

---

## 🖼️ Dashboard Preview

> 📁 Open `Customer_Support_Dashboard_Vijayendra.pbix` in Power BI Desktop to view the full interactive dashboard.

---

## 📌 Project Overview

| Detail | Info |
|---|---|
| **Tool Used** | Microsoft Power BI Desktop |
| **Dataset Size** | 8,469 rows |
| **Total Visuals** | 11 |
| **DAX Measures** | 4 |
| **Project Type** | Data Analytics / Business Intelligence |

---

## 🎯 Key KPIs

| KPI | Value |
|---|---|
| 🎫 Total Tickets | **8,469** |
| 🚨 SLA Breach Rate | **66.71%** |
| ⏱️ Avg Resolution Time | **884.21 days** |
| ⭐ Avg Satisfaction Score | **2.99 / 5** |

---

## 📊 Dashboard Visuals

1. **KPI Card** — Total Tickets
2. **KPI Card** — SLA Breach Rate
3. **KPI Card** — Avg Resolution Days
4. **KPI Card** — Avg Satisfaction Score
5. **Bar Chart** — Tickets by Type
6. **Donut Chart** — Tickets by Status
7. **Bar Chart** — Tickets by SLA Status
8. **Bar Chart** — Tickets by Priority
9. **Bar Chart** — Tickets by Channel
10. **Column Chart** — Avg Satisfaction by Ticket Type
11. **Slicer** — Filter by Ticket Priority

---

## 🔧 DAX Measures Created

```dax
-- 1. Total Tickets
Total Tickets = COUNTROWS('customer_support_tickets')

-- 2. SLA Breach Rate
SLA Breach Rate =
DIVIDE(
    COUNTROWS(FILTER('customer_support_tickets',
    'customer_support_tickets'[SLA Status] = "SLA Breached")),
    [Total Tickets]
) * 100

-- 3. Avg Resolution Days
Avg Resolution Days = AVERAGE('customer_support_tickets'[Resolution Time (Days)])

-- 4. Avg Satisfaction Score
Avg Satisfaction Score = AVERAGE('customer_support_tickets'[Customer Satisfaction Rating])
```

---

## 📁 Files in This Repository

---

## 🚀 How to Open This Dashboard

1. Download **[Power BI Desktop](https://powerbi.microsoft.com/desktop/)** (free)
2. Download this repository
3. Open `Customer_Support_Dashboard_Vijayendra.pbix`
4. Explore the interactive dashboard!

---

## 💡 Key Insights

- **66.71%** of tickets breached SLA — major service delivery issue
- Avg resolution time of **884 days** — process improvement needed
- Satisfaction score of **2.99/5** reflects impact of slow resolution
- Priority and channel analysis shows where most tickets originate

---

## 👨‍💻 About Me

**Vijayendra** — Aspiring Data Analyst from Anantapur, Andhra Pradesh
🔗 [GitHub](https://github.com/vijayendra) | [LinkedIn](https://linkedin.com/in/vijayendra)

---

⭐ *If you found this helpful, please give it a star!*
