# 📊 Power BI Project Management Dashboard with DAX

_An **interactive Power BI dashboard** for tracking and analyzing projects, built with a strong focus on **DAX (Data Analysis Expressions)**._

This project demonstrates how to transform raw project data into **dynamic KPIs, visual insights, and time-based calculations** using DAX.

---

## 🖼 Dashboard Preview
<img width="1257" height="707" alt="image" src="https://github.com/user-attachments/assets/4d853d65-b201-4270-a02b-5df4589da3be" />

---

## 📌 Project Description
This dashboard is designed to:
- Track **project budgets**, **hours spent**, and **project counts**.
- Provide **status-based analysis** (In Progress, Completed, On Hold).
- Allow interactive filtering by **Project Manager** and **Timeline**.
- Showcase **practical DAX implementations** for business reporting.

The data is fictional but reflects **real-world project tracking scenarios** — making it a great template for learning or professional use.

---

## 📂 Dataset Overview
The dataset (`Sheet1`) contains:
| Column           | Description |
|------------------|-------------|
| **ProjectID**    | Unique identifier for each project |
| **ProjectName**  | Name of the project |
| **ProjectManager** | Person responsible for the project |
| **Status**       | Project status (In Progress, Completed, On Hold) |
| **StartDate**    | Date when the project started |
| **DueDate**      | Project completion or deadline date |
| **Budget**       | Allocated budget for the project |
| **HoursSpent**   | Total hours worked on the project |

---

## 🛠 DAX Measures
This project uses **DAX** to calculate KPIs and time-based metrics.

### 🔹 DAX Measures
```DAX
Total Budget = SUM(Sheet1[Budget])

Total Hours Spent = SUM(Sheet1[HoursSpent])

Average Budget = AVERAGE(Sheet1[Budget])

Total Projects = DISTINCTCOUNT(Sheet1[ProjectID])
