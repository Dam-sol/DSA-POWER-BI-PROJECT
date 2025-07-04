### DSA-POWER-BI-PROJECT

### 📊 PALMORA GROUP HR ANALYSIS – Case Study 3

### 🔍 Case Overview

Palmora Group, a Nigerian manufacturing firm, faces growing scrutiny over **gender inequality** within its workforce, across three regions: Lagos, Abuja, and Kaduna. Negative media coverage has prompted the CHRO to launch an urgent internal investigation. As an HR Analytics consultant, you were brought in to assess the state of gender diversity, pay equity, and performance-based compensation within the company.

---

### 🧹 Data Cleaning & Preprocessing
Following initial inspection of the dataset:
- Replaced missing genders with `"Undisclosed"`.
- Removed employees with:
  - `NULL` departments
  - Missing salaries (assumed no longer employed)
 
  - ###📊 **Dataset summary after cleaning:**
- Total records: **946**
- Gender distribution:
  - Male: 465
  - Female: 441
  - Undisclosed: 40

---

## 📈 Analysis & Insights

### 1. Gender Distribution
- **By Region:**
  - Lagos has the largest and most balanced workforce.
  - Abuja is more male-dominated.
  - Kaduna has fewer employees and higher gender imbalance.
  
![image](https://github.com/user-attachments/assets/bc0b3bf6-5be1-4cc3-b6ee-6aba28997426)

- **By Department:**
  - Engineering and Sales are significantly male-heavy.
  - Support and Legal show more balanced representation.
  - Undisclosed genders appear across multiple departments.

  ### 2. Insight on rating based on gender

  ![image](https://github.com/user-attachments/assets/56461a45-08dc-4289-9a4d-6f13cd56ecfe)

  🗺️ Regional Gender Insights:
Lagos has the largest employee base and a relatively balanced male-female ratio.

Abuja leans more towards male employees.

Kaduna has a slight male dominance, but also shows a visible presence of "Undisclosed" gender entries.

 ### 3. Salary Structure & Pay Gap 
- Will explore average salary by gender across departments and regions.
- Identify departments/regions where the gender pay gap is highest.

-💰 Salary Structure & Gender Pay Gap Analysis

📊 1. Overall Pay by Gender

| Gender          | Avg Salary (\$) | Median Salary (\$) | Employee Count |
| --------------- | --------------- | ------------------ | -------------- |
| **Male**        | 74,790          | 73,360             | 465            |
| **Female**      | 72,136          | 72,500             | 441            |
| **Undisclosed** | 78,368          | 75,305             | 40             |


✅ Observation:

Males earn $2,654 more on average than females.

The median salary is also slightly higher for males, confirming a modest but real pay gap.

Employees with "Undisclosed" gender appear to earn significantly more, which could skew data in some departments.

🏢 2. By Department (Sample)

| Department           | Gender | Avg Salary (\$) |
| -------------------- | ------ | --------------- |
| Accounting           | Female | 72,939          |
| Accounting           | Male   | 77,530          |
| Business Development | Female | 74,628          |
| Business Development | Male   | 82,016          |

✅ Observation:

Departments like Accounting and Business Development show consistent gender-based salary gaps.

Males are paid ~$4,000–$8,000 more on average in these departments.

🌍 3. By Region (Sample)

| Region | Gender | Avg Salary (\$) |
| ------ | ------ | --------------- |
| Abuja  | Female | 70,452          |
| Abuja  | Male   | 73,246          |
| Kaduna | Female | 72,298          |
| Kaduna | Male   | 74,850          |

✅ Observation:

The pay gap persists across all regions, with Abuja showing the widest gap (~$2,800).

Even in Kaduna, males earn notably more than females.

🚨 Focus Areas for Management – Gender Pay Gap

🏢 Departments with the Largest Pay Gaps (Male - Female)

| Department               | Avg Male Salary | Avg Female Salary | Pay Gap (\$) |
| ------------------------ | --------------- | ----------------- | ------------ |
| **Business Development** | \$82,016        | \$74,628          | **\$7,389**  |
| **Human Resources**      | \$73,796        | \$66,579          | **\$7,217**  |
| **Services**             | \$79,456        | \$73,075          | **\$6,381**  |
| **Support**              | \$77,415        | \$72,030          | **\$5,385**  |
| **Product Management**   | \$76,101        | \$70,773          | **\$5,328**  |

🌍 Regions with the Largest Pay Gaps (Male - Female

| Region     | Avg Male Salary | Avg Female Salary | Pay Gap (\$) |
| ---------- | --------------- | ----------------- | ------------ |
| **Abuja**  | \$73,246        | \$70,452          | **\$2,794**  |
| **Kaduna** | \$74,850        | \$72,298          | **\$2,552**  |
| **Lagos**  | \$76,681        | \$74,163          | **\$2,517**  |

### 4. Compliance with $90,000 Minimum Wage
🚨 Conclusion:
Palmora does not meet the minimum wage requirement. Nearly 7 out of 10 employees are earning below the regulatory threshold.

📊 Overall Salary Band Distribution

The chart below shows how many employees fall into each $10,000 salary interval:

Most employees earn between $60,000–$90,000.

Very few are in the $90,000+ range, where regulatory compliance begins.

A significant number of staff are still below $60,000, indicating a large non-compliant population


![image](https://github.com/user-attachments/assets/48811d2c-c19b-4e4a-9249-2c4386d9018c)


![image](https://github.com/user-attachments/assets/82f43340-b0ab-4748-848b-51fec549b70f)

### 5. 🎁 Bonus Calculation – Individual Employees

🧮 Bonus Rule Mapping (from Bonus Rules Dataset):

| Performance Rating | Bonus % |
| ------------------ | ------- |
| **Very Good**      | 20%     |
| **Good**           | 15%     |
| **Average**        | 10%     |
| **Poor**           | 5%      |
| **Very Poor**      | 2%      |
| **Not Rated**      | 0%      |

💡 Sample Output – Top 10 Highest Bonus Recipients:

| Name             | Region | Department           | Rating    | Salary (\$) | Bonus (\$) |
| ---------------- | ------ | -------------------- | --------- | ----------- | ---------- |
| Barnaby Farnall  | Kaduna | Engineering          | Very Good | 118,800     | 23,760     |
| Evangelia Gowers | Kaduna | Business Development | Very Good | 118,450     | 23,690     |
| Hector Isard     | Abuja  | Support              | Very Good | 116,970     | 23,394     |
| Candy Aindrais   | Lagos  | Business Development | Very Good | 116,590     | 23,318     |
| Ashien Gallen    | Abuja  | R\&D                 | Very Good | 115,080     | 23,016     |
| Alexis Gotfrey   | Lagos  | Engineering          | Very Good | 114,470     | 22,894     |
| Cletus McGarahan | Kaduna | Engineering          | Very Good | 114,430     | 22,886     |
| Hogan Iles       | Lagos  | Accounting           | Very Good | 114,180     | 22,836     |
| Michale Rolf     | Lagos  | Services             | Very Good | 111,820     | 22,364     |
| Amery Ofer       | Abuja  | Legal                | Very Good | 111,050     | 22,210     |

💰 Total Amount Paid Per Region:

| Region     | Total Salary (\$) | Total Bonus (\$) | Total Compensation (\$) |
| ---------- | ----------------- | ---------------- | ----------------------- |
| **Abuja**  | 24,116,280        | 2,513,998        | **26,630,278**          |
| **Kaduna** | 26,652,820        | 2,656,528        | **29,309,348**          |
| **Lagos**  | 18,954,570        | 1,811,180        | **20,765,750**          |


🏢 Company-Wide Total:

| Metric                 | Amount (\$)    |
| ---------------------- | -------------- |
| **Total Salary**       | 69,723,670     |
| **Total Bonus**        | 6,981,705      |
| **Total Compensation** | **76,705,375** |


