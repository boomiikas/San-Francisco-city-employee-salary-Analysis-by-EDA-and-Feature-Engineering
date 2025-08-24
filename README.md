# 📊 San Francisco City Employee Salaries Analysis

## 📌 Overview
This project explores the **San Francisco City Employee Salaries dataset** (`salaries.csv`).  
The dataset contains employee compensation records including **base pay, overtime pay, benefits, and total pay**.  
The goal is to perform **Exploratory Data Analysis (EDA)** to uncover trends, salary distribution, and pay disparities.

---

## 📂 Dataset Description
The dataset includes the following columns:

- **Id** → Unique identifier for each record  
- **EmployeeName** → Name of the employee  
- **JobTitle** → Job title/designation  
- **BasePay** → Base salary of the employee  
- **OvertimePay** → Overtime compensation  
- **OtherPay** → Additional allowances/pay  
- **Benefits** → Benefits (insurance, pension, etc.)  
- **TotalPay** → BasePay + OvertimePay + OtherPay  
- **TotalPayBenefits** → TotalPay + Benefits  
- **Year** → Year of the salary record  
- **Agency** → Agency/department of employment  
- **Status** → Employment status (active/inactive, may contain nulls)

---

## 🎯 Objectives
- Perform **automated EDA** to visualize trends in pay components.  
- Identify **top-paying job titles** and their compensation.  
- Analyze **overtime vs. base pay** patterns.  
- Detect **outliers and anomalies** in salaries.  
- Examine **yearly trends** in employee compensation.

---

## 🛠️ Tech Stack
- **Python** (Pandas, NumPy)  
- **Matplotlib & Seaborn** for visualizations  
- **AutoViz / SweetViz / Pandas Profiling** for automated EDA  
- **Jupyter Notebook** for analysis  

---
## 📈 Analyses

Analyses on San Francisco City Employee Salaries 

-Benefits : 36163 rows has nan out of 148654 =24% --> so I used median to fill the nan values
-BasePay : 605 has null values, = 0.4% -->here , i dropped rows , doesnt make significant changes

1. **Distribution of Total Pay**
   - Most employees earn within lower pay ranges, creating a right-skewed distribution.
   - A few outliers with very high pay stretch the tail, indicating income disparity.
   - The gap between median salaries and extreme values highlights inequality in compensation.
   <img width="589" height="453" alt="image" src="https://github.com/user-attachments/assets/546f3872-a216-49c5-8ef7-13fe60d5fba6" />

2. **Average Salary Trend by Year**
   - The line plot shows how average salaries change over time.
   - Some years indicate steady growth, while others show dips, reflecting economic or policy shifts.
   - Overall, the trend highlights periods of salary rise and stagnation, capturing long-term pay dynamics.
<img width="591" height="453" alt="image" src="https://github.com/user-attachments/assets/dba235f3-2558-416e-bcbe-28a2b8421f2d" />

3. **Total Pay Outliers**
   - The boxplot reveals a wide range of salaries with several extreme outliers.
   - Most employees cluster in lower pay brackets, while a few exceptionally high earners pull the distribution upward.
   - These outliers highlight significant income inequality within the dataset.
<img width="578" height="453" alt="image" src="https://github.com/user-attachments/assets/3aee6f92-24a1-4827-8072-ff65a493afde" />

4. **Correlation between Pay Components**
   - BasePay shows a strong positive correlation with TotalPay, confirming it as the main salary driver.
   - OvertimePay and OtherPay contribute moderately, but with weaker correlations.
   - This indicates that while extra pay elements matter, core salary dominates total compensation.
<img width="515" height="433" alt="image" src="https://github.com/user-attachments/assets/bb533f35-e2d4-4277-aaf4-93557762851e" />

5. **Top 10 Highest Paying Job Titles**
   - The bar chart highlights job titles with the highest average pay.
   - Executive and specialized roles dominate the list, reflecting the premium placed on expertise and leadership.
   - The steep gap between top roles and others underlines salary concentration in select positions.
     <img width="950" height="453" alt="image" src="https://github.com/user-attachments/assets/80c9be01-5399-4449-b5e4-045179540db0" />
     
6. **Top 10 Highest Paying Agencies**
   - The bar chart shows agencies with the highest average pay.
   - Specialized agencies and departments with technical or leadership roles dominate the top ranks.
   - The pay gap across agencies highlights how institutional focus and funding drive compensation differences.
<img width="640" height="453" alt="image" src="https://github.com/user-attachments/assets/61cdb7f9-ed25-4ff5-b6bf-f6227a20c1b7" />

7. **Average Total Pay by Year**
   - The line plot shows fluctuations in salaries across years.
   - Some periods reflect steady growth, while others dip, likely due to budget or economic changes.
   - Overall, the trend captures long-term variations in employee compensation.
<img width="713" height="468" alt="image" src="https://github.com/user-attachments/assets/8407e29f-148b-43b8-bcbd-300f40e1c336" />
   
6. **Contribution of Pay Components**
   - BasePay forms the largest share of compensation, dominating overall pay.
   - OvertimePay and OtherPay contribute smaller portions, showing limited impact compared to base salaries.
   - This confirms that salary structure is heavily anchored in fixed pay rather than variable components.
<img width="589" height="509" alt="image" src="https://github.com/user-attachments/assets/4476e4ac-ffae-428a-9b75-885b78e77a20" />

---

## 📊 Results & Findings (Sample Insights)
- **Highest paid job title**: Chief of Police  
- **Maximum Total Pay (with benefits)**: $567,595  
- **Overtime pay contributes significantly** in certain public safety roles.  
- Some columns (`Benefits`, `Status`) contain many missing values.  
- **Outliers** exist in BasePay and OtherPay (e.g., negative/zero values).  

---

## 🚀 Future Work
- Build **salary prediction models** (Regression, ML).  
- Compare salaries **across years** to detect growth patterns.  
- Investigate **gender-based or role-based pay disparities** (if demographic data is available).  
- Create an **interactive dashboard** (Plotly/Power BI/Tableau).  

---
