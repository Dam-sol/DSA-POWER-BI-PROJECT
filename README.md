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
  - Kaduna has the largest and more male-dominated 
  - Abuja is most balanced workforce.
  - Lagos has fewer employees.

- **By Department:**
  - Engineering and Sales are significantly male-heavy.
  - Support and Legal show more balanced representation.
  - Undisclosed genders appear across multiple departments.

 ### 2. Insight on rating based on gender

<img width="194" alt="image" src="https://github.com/user-attachments/assets/ecd3f72a-188e-43fb-a07d-65961896c522" />




  🗺️ Regional Gender Insights:

  
  

  <img width="191" alt="total emplloyee by location and gender" src="https://github.com/user-attachments/assets/0f8a9b15-4086-4602-b33b-93677080e6d0" />
  
Kaduna has the largest employee base and lean more towards male employees

Abuja has a larger employees and a relatively balanced male-female ratio.

Lagos has a slight male dominance, but also shows a visible presence of "Undisclosed" gender entries.

 ### 3. Salary Structure 
- Will explore average salary by gender across departments and regions.
- Identify departments/regions where the gender pay gap is highest.

-💰 Salary Structure & Gender Pay Gap Analysis

📊 1. Total Pay by Gender


<img width="165" alt="image" src="https://github.com/user-attachments/assets/4efc3157-fca2-4a22-b28c-e84d18b45406" />


🏢 2. By Department (Sample)



<img width="215" alt="image" src="https://github.com/user-attachments/assets/3622d0fa-22d3-40e1-9370-57908b51e51f" />



🌍 3. By Region (Sample)



<img width="200" alt="image" src="https://github.com/user-attachments/assets/4f23d70e-b01a-4811-afa6-95fd75b2efc6" />


🏢 Departments with the Largest Pay Gaps (Male - Female)

| Department               |  Male Salary    | Female Salary     | Pay Gap (\%) |
| ------------------------ | --------------- | ----------------- | ------------ |
| **Account**              | 55.85%          | 40.11%            | **10%**      |
| **Product Management**   | 54.83%          | 44.61%            | **10%**      |
| **Support**              | 53.32%          | 41.71%            | **12%**      |
| **Sales**                | 49.99%          | 43.88%            | **6%**       |


### 4. Compliance with $90,000 Minimum Wage
🚨 Conclusion:
Palmora does not meet the minimum wage requirement. Nearly 7 out of 10 employees are earning below the regulatory threshold.

📊 Overall Salary Band Distribution

The chart below shows how many employees fall into a band of $10,000 – $20,000, $20,000 – $30,000 interval:

<img width="302" alt="image" src="https://github.com/user-attachments/assets/e2625e99-14c5-4498-8f92-a33652ac4e77" />

📊 The visual by Region


<img width="276" alt="image" src="https://github.com/user-attachments/assets/632061fb-3856-4b06-a587-61e6fb2ce36e" />

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


