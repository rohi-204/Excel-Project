# 🎧 **Spotify Social Media Analytics – Strategic Branding with Excel**

---

## 💼 **Recruiter Note**
This project demonstrates my skills in **Excel, Power Query, data cleaning, business analytics, and storytelling with data**.  

I applied advanced Excel formulas, PivotTables, and visualization techniques to transform raw social media data into actionable insights for Spotify’s branding strategy.  

If you’re looking for someone who can combine **technical skills with business thinking**, this project is a strong example of my ability to:  
- Clean and structure large datasets  
- Apply analytics to marketing data  
- Build meaningful KPIs (**Engagement Rate, ROI, Follower Growth**)  
- Deliver clear insights that guide business decisions  

---

## ❓ **Problem Statement**
Spotify runs multiple campaigns across **Instagram, Twitter, Facebook, and YouTube**.  

However, the marketing team struggles to measure:  
- Which **content types, hashtags, and platforms** drive the most engagement  
- How **campaigns impact follower growth**  
- Where **ad budgets** should be allocated most effectively  

---

## 🎯 **Objective**
The objective of this project is to **clean, organize, and analyze Spotify’s social media data using Excel and Power Query** to evaluate:  
- Engagement performance  
- Platform growth  
- Hashtag effectiveness  
- Campaign ROI and uplift  
- Follower retention trends  

and provide **actionable insights for improving branding strategy**.  

---

## 📂 **Dataset & Cleaning (Task 1)**
Data cleaning was performed in **Power Query**:  
- Removed duplicates and standardized column names  
- Fixed inconsistent date formats and changed data types  
- Replaced null/missing values in engagement metrics with **0**  
- Split **Hashtags** column by delimiter → separated multiple hashtags  
- Split **Target Platforms** column by delimiter → handled multi-platform campaigns  
- Loaded clean tables into Excel as:  
  - `tblPosts` → post-level data  
  - `tblWeekly` → weekly metrics  
  - `tblCamps` → campaign metadata  

**Insight:**  
- The dataset was standardized into structured tables, ensuring accuracy and consistency for further analysis.  

---

## 📊 **Analysis & Formulas**

### 📝 **Engagement Analysis (Task 2)**
- Engagement Rate formula:  
  ```excel
  = (Likes + Comments + Shares) / Impressions
- Ranked posts & hashtags:
  ```excel
  =RANK.EQ([@Engagement Rate], [Engagement Rate], 0)

**Insight**
- **Twitter** posts had the highest engagement rate
- Hashtags **#SpotifyWrapped** and **#NowPlaying** were top performers

---

### 📈 **Platform Performance (Task 3)** 
- Weekly growth & engagement rate analyzed using PivotTables
- Correlation between Ad Spend & Net Followers:
  ```excel
  =CORREL(tblWeekly[Ad_Spend], tblWeekly[Net_Followers])

**Insight**
- **Twitter** delivered the highest engagement
- **Instagram** showed consistent follower growth
- **Ad spend had weak correlation** with follower growth → content quality mattered more

---

### 🏷️ **Hashtag & Content Strategy (Task 4)**
- Compared Text, Story, Reel performance across platforms using PivotTables
- Average clicks per hashtag calculated via Pivot

**Insight**
- **Text posts** on Instagram & Twitter performed best for engagement
- **Reels** gained high impressions but lower interaction
- **#SpotifyWrapped** was the most impactful hashtag overall

---

### 📢 **Campaign Effectiveness (Task 5)**
- ROI (Engagements per Spend):
  ```excel
  = [@Total_Engagements] / [@Campaign_Ad_Spend]
- Engagement Uplift:
  ```excel
  = [@During_Eng_Rate] - [@Pre_Eng_Rate]
- Follower Growth during campaign:
  ```excel
  = SUMIFS(New_Followers) - SUMIFS(Unfollows)

**Insights**
- **ChillVibes** → highest follower growth
- **SummerBeats** → largest uplift in engagement
- **Wrapped2024** → strong ROI compared to spend

---

### 👥 **Follower Retention & Loyalty (Task 6)**
- Highest Net Followers Week:
  ```excel
  =MAXIFS(tblWeekly[Net_Followers], tblWeekly[Platform], "Twitter")
- 4-Week Moving Average:
  ```excel
  =AVERAGE(OFFSET([@Total_Followers], -3, 0, 4, 1))

**Insight**
- **Twitter** had the strongest single-week follower gain
- **4-week moving average** showed smoother growth trends
- **Ad spend had little direct impact** on follower growth

---

## 🔎 **Final Key Insights**
- **Twitter** → strongest for engagement
- **Instagram** → best for steady follower growth
- **#SpotifyWrapped** → top-performing hashtag
- **SummerBeats** → highest engagement uplift
- **ChillVibes** → highest follower growth
- **Ad Spend ≠ guaranteed growth** → content quality matters more

---

## 🛠 Tools Used
- **Excel** → PivotTables, PivotCharts, Conditional Formatting
- **Power Query** → Data cleaning & transformation
- **Excel Formulas** → SUMIFS, AVERAGEIFS, RANK.EQ, MAXIFS, OFFSET, CORREL
- **Visualizations** → Line charts, bar charts, moving averages

---

## 🔮 **Future Scope**
- Build **Power BI** dashboards for interactive visualizations
- Apply **predictive modeling** to forecast engagement & growth
- Automate updates with **Power Automate or Python scripts**
#### **📌 This project highlights my ability to turn raw marketing data into actionable insights using Excel and Power Query, demonstrating both technical expertise and business understanding.**
