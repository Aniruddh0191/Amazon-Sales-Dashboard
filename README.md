# 🛒 Amazon Sales & Prime Movies Dashboard

A Power BI portfolio project for exploring Amazon product sales and an Amazon Prime movie dataset. The repository includes the Power BI report, source Excel workbooks, dashboard background asset, and the original project problem statement.

> **Important:** This repository documents the supplied project files and the analysis requirements. It does not claim that every KPI or visual has been independently validated. Review the measures, relationships, data types, and source data in Power BI before using the report for business decisions.

## 📌 Project Overview

The project brief asks for two analysis areas:

1. **Amazon Products — Sales Analysis**
2. **Amazon Prime — Movie Analysis**

The aim is to organize the supplied data and present relevant metrics and trends through an interactive Power BI report.

## 🎯 Objectives

- Review product sales and product-category performance.
- Track sales and product activity across time.
- Explore review counts as a customer-engagement indicator.
- Analyze movie counts by release year and compare movie-level metrics.
- Document the datasets and the intended dashboard questions.
- Provide a reproducible starting point for reviewing the Power BI report.

## 📊 Dashboard Requirements

### Dashboard 1 — Amazon Products Sales Analysis

**KPIs specified in the project brief**
- Year-to-Date (YTD) Sales
- Quarter-to-Date (QTD) Sales
- YTD Products Sold
- YTD Reviews

**Charts specified in the project brief**
- YTD Sales by Month — line chart
- YTD Sales by Week — column chart
- Sales by Product Category — text or heat-map visual
- Top 5 Products by YTD Sales — bar chart
- Top 5 Products by YTD Reviews — bar chart

### Dashboard 2 — Amazon Prime Movie Analysis

**KPIs specified in the project brief**
- Total Sales
- Total Number of Movies
- Total Number of Reviews

**Charts specified in the project brief**
- Total Movie Counts by Release Year — line chart
- Total Sales by Movie Type
- Top 5 Movies by Total Sales — bar chart
- Top 5 Movies by Total Reviews — bar chart

**Metric definition warning:** Confirm the business meaning of “sales,” “products sold,” and “reviews” from the supplied data before building or interpreting measures. The column names alone do not establish whether a field represents a monetary amount, a count, a rating, or a review total.

## 🗂️ Repository Structure

```text
Amazon-Sales-Dashboard/
├── README.md
├── .gitignore
├── Dashboard/
│   └── Amazon Sales Dashboard.pbix
├── Data/
│   ├── Amazon_Combined_Data.xlsx
│   └── Amazon_Prime_Movies.xlsx
├── Assets/
│   └── Amazon_Dashboard_Background.jpg
└── Documentation/
    └── Amazon_Sales_Dashboard_Problem_Statement.docx
```

## 🧾 Included Files

| File | Purpose |
|---|---|
| `Dashboard/Amazon Sales Dashboard.pbix` | Main Power BI report file supplied for this project |
| `Data/Amazon_Combined_Data.xlsx` | Product dataset workbook supplied for the sales analysis |
| `Data/Amazon_Prime_Movies.xlsx` | Movie dataset workbook supplied for the Prime analysis |
| `Assets/Amazon_Dashboard_Background.jpg` | Background image supplied for dashboard design |
| `Documentation/Amazon_Sales_Dashboard_Problem_Statement.docx` | Original problem statement and required questions |

## 🧱 Source Data Overview

The workbook headers inspected for this project are listed below. This is a schema inventory, not a claim that the data is already cleaned or validated.

### Product workbook — `Amazon_Combined_Data.xlsx`

Worksheet: `Amazon_Data`

| Column | Initial interpretation to verify |
|---|---|
| Product Category | Product grouping/category |
| Product Description | Product description or name |
| Price(Dollar) | Price field in dollars; confirm whether it is unit price or sales amount |
| Number of reviews | Review-count field; confirm aggregation and missing-value handling |
| Shipment | Shipment-related field; confirm values and business meaning |
| Order Date | Order date; verify data type and date range |

### Movie workbook — `Amazon_Prime_Movies.xlsx`

Worksheet: `Amazon Prime Data`

| Column | Initial interpretation to verify |
|---|---|
| Product Description | Movie title/description |
| Price(Dollar) | Price field in dollars; confirm whether it is a sales amount or another price measure |
| Quality | Quality/rating-related field; verify its definition |
| Release Year | Movie release year |
| Movie type | Movie type/category |
| Actor | Actor information |
| Director | Director information |
| Number of reviews | Review-count field; confirm aggregation and missing-value handling |

## 🚀 How to Open the Project

1. Download or clone this repository.
2. Open `Dashboard/Amazon Sales Dashboard.pbix` in Microsoft Power BI Desktop.
3. If Power BI asks for data-source credentials or cannot locate a workbook, use **Transform data → Data source settings** or edit the source paths in Power Query to point to the files in `Data/`.
4. Refresh the report and inspect the Power Query steps, relationships, measures, and visuals.
5. Validate all KPI definitions and results against the source workbooks before publishing or presenting the report.

Power BI Desktop is required to edit the `.pbix` file. GitHub can store and preview the repository files, but it does not render an interactive Power BI report directly inside the README.

## 🧪 Validation Checklist

Before presenting the project as final, check:

- [ ] Both workbooks load without errors.
- [ ] Column names and data types are correct.
- [ ] Dates are parsed correctly and the calendar table covers the intended period.
- [ ] Duplicate records and missing values are reviewed and documented.
- [ ] The definition of sales/revenue is confirmed rather than assumed from `Price(Dollar)`.
- [ ] Review counts are numeric and are not accidentally summed where a different aggregation is appropriate.
- [ ] Movie counts use a suitable distinct-count or row-count definition.
- [ ] Top 5 visuals use the correct measure and sort order.
- [ ] YTD/QTD measures use a valid date table and appropriate filter context.
- [ ] The report refreshes after the source files are placed in the expected location.
- [ ] Sensitive or personal information is not included in the public repository.

## 🛠️ Tools

- Microsoft Power BI Desktop
- Microsoft Excel / compatible spreadsheet application
- Git and GitHub

## 📤 Upload to GitHub

### Option A — GitHub website

1. Sign in to [GitHub](https://github.com/).
2. Select **New repository**.
3. Set the repository name to `Amazon-Sales-Dashboard`.
4. Add a description such as: `Power BI project for Amazon product sales and Prime movie analysis`.
5. Choose **Public** for a portfolio project only if you have permission to publish all included data and assets; otherwise choose **Private**.
6. Create the repository.
7. Upload the contents of this project folder, preserving the folder structure.
8. Commit the files with a message such as `Add Amazon sales dashboard project`.

### Option B — Git command line

Run these commands from inside the extracted `Amazon-Sales-Dashboard` folder after creating an empty GitHub repository:

```bash
git init
git add README.md .gitignore Dashboard Data Assets Documentation
git status
git commit -m "Add Amazon sales dashboard project"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/Amazon-Sales-Dashboard.git
git push -u origin main
```

Replace `YOUR-USERNAME` with your GitHub username. Do not paste a password or access token into the repository or README.

## ⚠️ Data, Licensing & Privacy

- Confirm that you have permission to publish the supplied Excel data, report, and background image before making the repository public.
- The problem statement highlights data accuracy, integration, and privacy as key challenges.
- Avoid publishing personal, confidential, or restricted business information.
- This repository contains the supplied project files; it does not assert that the data is official Amazon corporate data or that Amazon endorses this project.

## 👤 Author

**Anirudh Kumar Yadav**  
Data Analytics | Power BI | Excel

---

*Built as a data analytics portfolio project. Update this README with verified findings, dashboard screenshots, and validated KPI definitions after reviewing the final report.*
