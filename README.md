# NHS Cancer Waiting Times Dashboard (July 2021–2024)

This Power BI project analyses NHS cancer treatment wait times across Integrated Care Boards (ICBs), using commissioner-based data from July 2021 to July 2024. It looks at how performance changed over time, particularly around the introduction of ICBs in July 2022. The dashboard highlights national trends, regional variation, and the ICBs showing the most improvement.

---

## Project Goals

- Track changes in the % of patients treated within 62 days of urgent GP referral
- Compare performance across ICBs and years
- Highlight best and worst performers
- Present insights clearly using interactive dashboards


---

## 📊 Dashboard Overview

The report contains five interactive pages:

### 1. Summary

Provides a national overview of treatment performance between July 2021 and July 2024:

- **KPI cards**:
  - Absolute change in % treated within 62 days (2021–2024)
  - Relative % change in % treated (2021–2024)
  - % treated in July 2021
  - % treated in July 2024
- **Line charts**:
  - National average % treated across all ICBs per year
  - Total number of cancer patients treated in July of each year
- **Bar charts**:
  - Top 5 ICBs by absolute improvement (change) (2021–2024)
  - Top 5 ICBs by relative % improvement (change) (2021–2024)
  - Top 5 ICBs by % treated in July 2021
  - Top 5 ICBs by % treated in July 2024
- **Matrix**:  
  Ranks the top 5 ICBs by % treated in July 2024 and displays their actual values

---

### 2. Dive Into ICBs

Explores trends at an individual ICB level. This dashboard shows that a higher number of treated patients doesn’t necessarily reduce performance. Notably, July 2024 saw a sharp rise in patients treated (due to increased screening), yet performance improved:


- **Line graphs**:
  - % of patients treated within 62 days by ICB (2021–2024)
  - Total number of patients treated by ICB (2021–2024)
- **Slicers**:
  - Year selector
  - ICB selector
- **KPI cards** (interactive):
  - Average % treated within 62 days
  - Number treated within 62 days
  - Number treated after 62 days
  - Total number of patients treated

---

### 3. Percentage Matrix

Compares all ICBs side by side across the 4 years, showcasing how most tend to drop from 2021 to 2022 and then improve over 2022 to 2024. Sliders placed to be able to interact with dashboard and see which ICB's performed best each year, exploring how that stood up over other years:

- **Clustered bar chart**:  
  Displays % treated within 62 days for each ICB by year
- **Matrix**:  
  Lists each ICB's % performance per year plus an overall average
- **Slicers**:
  - Select year to focus on
  - Sort matrix and chart by year or overall average

---

### 4. Absolute Percentage Change 

Highlights how ICBs changed in terms of raw percentage points. Showcases which ICB's saw the most improvement from year to year, further steps would be to research what these ICB's did that showed improvement:

- **Clustered bar chart**:
  - Change from 2021–2022
  - Change from 2022–2023
  - Change from 2023–2024
  - Total change from 2021–2024
- **Matrix**:  
  Shows exact % point changes by ICB
- **Slicer**:
  - Sort by absolte change across any year, total absolute change or by the average percentage of patients treated withing 62 days across July of all years

---

### 5. Relative Percentage Change

Similar to the previous page, but based on proportional changes:

- **Clustered bar chart** and **matrix**:
  - Shows % change relative to previous performance
- Helps highlight ICBs that made strong progress even from a low starting point
- **Slicer**:
  - Sort by any year, total relative change or by the average percentage of patients treated withing 62 days across July of all years

---

## File Structure
-📂 Dashboard PDF/ → PDF report

-📂 data/

 - clean/ → Cleaned & Dombined Data
 - raw/ → Original NHS Excel files

-📂 Images/ → Screenshots and dashboard GIFs

-📄 nhs_dashboard.pbix

-📄 README.md


---

## Screenshots & GIFs

### 1. Summary
![Summary](Images/01_NHS_Cancer_Wait_Times_Analysis_Summary.png)

---

### 2. Dive into ICBs
![Dive into ICBs](Images/02_Dive_into_ICB's.gif)

---

### 3. Percentage Matrix
![Percentage Matrix](Images/03_Percentage_Matrix.gif)

---

### 4. Absolute Improvement
![Absolute Change](Images/04_Absolute_Percentage_Change_Visual.gif)

---

### 5. Relative Percentage Improvement
![Percentage Change](Images/05_Relative_Percentage_Change_Visual.gif)


---

## Notes

- **Why July only?**  
  July was one of the only months consistently available across all four years. Using the same month each year avoids seasonal bias and allows a fair comparison.

- **ICB policy context:**  
  ICBs replaced CCGs in July 2022, so this project looks at performance before and after that change.

- **Most improved ICB's:**  
  ICBs that showed improvement in percentage of patients treated within the 62 day limit were also shown to be the worst performers overall, this is most likely due to them having more room for improvement and pushes to try and make them perform better. Interestingly one of the top performers overall in NHS Suffolk and North East Essex Integrated Care Board did see improvement from July 2021 to 2024 (albeit small). An interesting next step would be to see what they have done to try and find this improvement when already acting at one of the hightest national averages.

- **Limitations:**  
  Only July data is included. A follow-up project will bring in all months via SQL for a full trend analysis.

---

## Tools Used
- Power BI (DAX, KPIs, slicers, custom visuals)
- Excel (data cleaning, mapping CCGs to ICBs)
- Google Colab (data cleaning, mapping CCGs to ICBs)
- GitHub (version control and presentation)

---

## Download PDF Report

[Click here to view the dashboard PDF](Dashboard_PDF/NHS%20cancer%20wait%20times%20analysis%20pdf.pdf)

---
## Download Dashboard (Interactive)

[Click here to view the dashboard in PowerBI](NHS%20Cancer%20Wait%20Times%20Analysis%20Dashboard.pbix)

---
## Data Source

[NHS Cancer Waiting Times – NHS England](https://www.england.nhs.uk/statistics/statistical-work-areas/cancer-waiting-times/)

---

This project was created for portfolio purposes and to demonstrate relevant skills for NHS data roles.
