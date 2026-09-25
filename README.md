# 🎯 Kickstarter Crowdfunding Data Analysis (Power BI)

![Power BI](https://img.shields.io/badge/Tool-Power%20BI-yellow?logo=powerbi)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![License](https://img.shields.io/badge/License-MIT-blue)
![GitHub stars](https://img.shields.io/github/stars/your-username/your-repo?style=social)

---

## 📌 Overview
This repository contains a **Power BI dashboard** analyzing Kickstarter crowdfunding trends from **2009–2019**.  
It highlights project outcomes, categories, funding goals, and global participation patterns.

---
## 📂 Data Sets

This project leverages four structured tables to analyze Kickstarter crowdfunding trends:

1. **Crowdfunding Projects (Fact Table)**  
   - **Fields:** ProjectID, ProjectName, CategoryID, CreatorID, LocationID, GoalUSD, USD_Pledged, BackersCount, CreatedDate, DeadlineDate, State  
   - **Purpose:** Central fact table containing project-level details such as funding goals, pledged amounts, backers, and project outcomes.

2. **Category (Dimension Table)**  
   - **Fields:** CategoryID, CategoryName  
   - **Purpose:** Defines project categories (e.g., Product Design, Music, Games, Film). Enables category-wise analysis.

3. **Location (Dimension Table)**  
   - **Fields:** LocationID, Country, Region, City  
   - **Purpose:** Stores geographical information for projects. Supports country-wise and region-wise breakdowns.

4. **Creator (Dimension Table)**  
   - **Fields:** CreatorID, CreatorName, CreatorProfile  
   - **Purpose:** Contains information about project creators. Helps track projects by individual or organization.

---

## 🛠 Data Modeling

The **Crowdfunding Projects** table acts as the **fact table**, while **Category**, **Location**, and **Creator** serve as **dimension tables**. This star schema design ensures efficient slicing and dicing of data in Power BI.

### 🔗 Relationships
- **Crowdfunding Projects → Category**  
  - Relationship: `Projects.CategoryID = Category.CategoryID`  
  - Purpose: Analyze projects by category.

- **Crowdfunding Projects → Location**  
  - Relationship: `Projects.LocationID = Location.LocationID`  
  - Purpose: Map projects by country and region.

- **Crowdfunding Projects → Creator**  
  - Relationship: `Projects.CreatorID = Creator.CreatorID`  
  - Purpose: Track projects by creator.

---

## 🔑 Key Metrics
- 📈 **Total Projects:** 365,892  
- 👥 **Total Backers:** 4,291  
- 🧑‍💻 **Total Creators:** 334,841  
- 💰 **Funding Goal:** $16B+  
- ⏳ **Average Duration:** 34 days  
- 🗂️ **Categories Covered:** 169  

---

## 📈 Insights
- 🚀 Crowdfunding peaked in **2015** with 58K projects.  
- ✅ **Success Rate:** ~38% of projects reached their goal.  
- ❌ **Failure Rate:** ~51% of projects did not succeed.  
- 🎮 **Top Categories:** Product Design, Tabletop Games, Music, Documentaries.  
- 🌍 **Regional Trends:** North America & Europe lead in project density.  

---

## 🛠 Data Modeling
The project uses four core tables:

- **CrowdfundingProjects** → central fact table  
- **Category** → defines project categories  
- **Location** → stores geographical info  
- **Creator** → contains creator details  

---

## 📝 Conclusion
This Power BI project provides a **comprehensive view of Kickstarter crowdfunding trends (2009–2019)**, enabling stakeholders to understand:
- 📊 **Patterns of success and failure** across categories and years  
- 🌍 **Global participation** and regional strengths  
- 🎮 **Emerging categories** like product design and tabletop games  
- 💡 **Key factors** influencing project outcomes  

By combining **data modeling, interactive visuals, and storytelling**, this dashboard transforms raw Kickstarter data into **actionable insights**.  
It serves as a valuable resource for **creators, backers, and analysts** who want to explore the dynamics of crowdfunding platforms.

---

✨ *This project demonstrates the power of data visualization in uncovering trends and guiding decision-making. If you found it useful, please star ⭐ the repository and share your feedback!*

## 📊 Dashboard Preview
![Dashboard Screenshot](https://github.com/vaibhav-vj24/Crowdfunding-Data-Anlyasis/blob/main/Crowdfunding%20Data%20Analysis.png)  
*(Add your dashboard screenshot here for a visual preview)*




