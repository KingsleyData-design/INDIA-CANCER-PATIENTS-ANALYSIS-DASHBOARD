# INDIA CANCER PATIENTS ANALYSIS (2022-2025)

## KEY METRICS

| METRIC | VALUE |
|---|---|
| TOTAL PATIENTS | 100,000 |
| % ALIVE | 36.42% |
| % DECEASED | 63.58% |
| AVERAGE SURVIVAL MONTHS | 20.33 |
| MOST COMMON CANCER TYPE | Breast Cancer |
| CANCER TYPE COVERED | 9 |
| TOTAL HOSPITALS | 10 |


## PROJECT OVERVIEW
  This Analysis looks at 100,000 cancer patient records across India from 2022 to 2025, looking at which cancer shows up the most, who's actually surviving, and where treatment seems to be making the biggest difference. Covering the same dataset across Excel, Power BI, Python and SQL. The analysis explores patient demographics, cancer types, disease staging, treatment approaches / type and survival outcomes.

## KEY INSIGHTS — THE DATA STORY 

- **Breast cancer is by far the most common diagnosis** in this dataset — its bar is roughly double the next highest (Oral Cancer), and the drop-off continues steadily down through Cervical, Lung, Colorectal, Stomach, Prostate, Leukemia, and Ovarian.
- **63.58% of patients in this dataset are deceased, 36.42% are alive.** That's a heavy number, and it's the headline stat the rest of the dashboard is really explaining.
- **Adults make up the overwhelming majority of cases**, followed by Seniors, then Young Adults, with Pediatric cases barely registering — cancer in this dataset is overwhelmingly an adult and senior condition, not a pediatric one.
- **Stage III is the most common stage at diagnosis**, followed by Stage II and Stage IV, with Stage I being the smallest slice. Most patients aren't being caught early — they're showing up once the disease has already progressed.
- **Survival months don't vary hugely by treatment type** — surgery, radiation, chemo, targeted therapy, and combinations all sit in a fairly similar range, suggesting no single treatment is a dramatic outlier compared to the others in this dataset.

## RECOMMENDATIONS — SO WHAT WOULD THIS ACTUALLY MEAN FOR A HEALTH SYSTEM?

- **Push harder on early detection, specifically for breast cancer.** Since it's both the most common diagnosis and Stage III is the most common stage at diagnosis, a lot of these cases are likely being caught later than they could be. Earlier screening could shift that stage distribution meaningfully.
- **Pediatric cancer being such a small slice doesn't mean it should be ignored** — it likely means pediatric cases need entirely separate protocols and resourcing rather than being folded into general adult treatment planning.
- **Since treatment type isn't showing huge survival differences on its own, stage at diagnosis is probably the bigger lever.** Resources might do more good going toward catching cancer earlier (screening access, awareness) than toward debating which treatment protocol is marginally better.
- **The regional spread (visible on the state map) is worth investigating further** — if certain states show heavier patient concentration, that could point to either higher incidence or just better access to diagnosis and reporting in those areas, which are two very different problems.

## WHAT I BUILT IT IN AND WHY FOUR TIMES?

- **Excel** — cleaned and explored the data, first pass at survival and outcome breakdowns.
- **Power BI** — the main dashboard. Cancer Type and Gender as slicers, with charts covering survival by cancer type, survival months by treatment, age group, outcomes by stage, and a map of patients across Indian states.
- **SQL** — same KPIs rebuilt as queries against the dataset.
- **Python** — same analysis again in a notebook, pandas and matplotlib doing the work.

Same reasoning as the rest of the portfolio — four tools, same questions, because the point isn't the dashboard, it's proving the logic holds up across all of them.

## DATASET
- **Source:** Kaggle
- **Records:** 100,000 rows
- **Timeframe:** 2022–2025
- **Columns:** Patient_ID, Age, Gender, State, City, Hospital_Name, Cancer_Type, Stage, Treatment_Type, Diagnosis_Date, Survival_Months, Status, Age_Group


## FILES IN THIS REPOSITORY
- `india_cancer_patients_cleaned.csv` — Cleaned dataset
- `india_cancer_patients_dashboard.xlsx` — Excel dashboard
-` Power BI dashboard`
- `indian_patients_SQL.sql` — SQL queries
- `india_cancer_patients_analysis.ipynb` — Python notebook
